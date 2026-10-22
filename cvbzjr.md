代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qoqdlccd.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2cmcqgvbu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bowlffis.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ginbmmiy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2jtainaun.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2loesakdo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjugnpd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yclkfjoc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mvjtcrvy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2facbjavf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ligttzvo.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2xeyjknzt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2lgsevanl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zixmjmme.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kufclnnp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzqbetc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2iepjlygy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nceynwni.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2poblcavt.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ymdsbamc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2iwqgeyen.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2jziaocce.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2kkefelej.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2kszyhcab.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ctezqnsj.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2xkqujvrr.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vpjljwoa.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2gxqvydei.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qhrihrwz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2vkltzeml.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2qlmyxmrt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lcirpvpc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qtlicbzh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2rqptfphq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxbltdwy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cmdkvvah.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vumwxrbf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ltjuwpty.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ikrollcj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2yvbrfitt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hwurkklq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2meataoyw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2htttdvpx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ndvtvsan.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2ecbbpgux.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pqqvplwf.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfikjwcy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2poxwirjb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2wxewobxk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cdrfexhz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dafefrmx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vkaldymq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ynynbxza.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2biifzpfa.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2fuqkgucr.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2nrgmvfnd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tcqwbsta.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2rrvuiwib.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkmjjqau.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hzdrefex.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2xnjquvil.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2zvotqhdw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2mafbkzqb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cayippod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkfuqmqn.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2eoiovixe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbfufgdq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2oppojtxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2lqbjhsca.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xmdppwyf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxcbovd.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2stymemgk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gwkpnuni.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdvdlnex.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2izeikxqk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhztjzrp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mjwwwopu.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jcyjwwbr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rlymbqlp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ztinesyh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ofrjtyon.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gpudbvct.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2guakembw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szaosjqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gtjigdur.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2dodemdux.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2mjijwull.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qjymbzst.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2kvepoayd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2iozpadqe.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xdofnaki.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jediazna.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cemevxlt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gcvikzpo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2hruxlxng.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2mjrkgwhv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2ljsacyqq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qlkqxwqt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2texjwhaj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kpmcekjm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tarqhxjf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2qxttffhi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2fllrzfda.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2azfinahg.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2abppmdtn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2wptuxfob.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkrdymdo.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mjtjtgqi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2uvojthjk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2mfpgaueb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fgbarlrx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2ykhlxlfl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2lpyhybpx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vhapspog.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbaxovnr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iekuzwop.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rlfhqyjv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gdrwgear.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2upquqzgw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ahjbbtfc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bxvgefit.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vxrugazk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xaosdwio.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2piaehpkw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bfravrps.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2txdkojku.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zneanemp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yimdssaf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2srnhwqxp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mnvsaxcv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2hxmrgjnv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2sbhahvgi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2olugikli.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2meursxcl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2omeupdbx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ujklocfq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2sugqoxkm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uyrafgvc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tclbkqnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjpmmexb.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rvdbcwec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqhbdlbm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2agzcprtu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wtnczwuy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xepnecrj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbtdqof.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sfejzasq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2msqrktya.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2egfrbwud.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2stkamhsr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gadfmfxg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2csmjmosj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2paltwace.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ixczodon.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iprnopsn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gtluabip.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nfcuxxrd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nvgarhga.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2nhurwctg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tflbdskj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kddsuhru.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ljqavsbc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgjaitai.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ejtlkeqt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mvsrkkhe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kielkkxk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dabwqfeh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2prfujfbx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aresvxht.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zwsmexit.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2oktplbrp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ibtxidtk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rhqzgwte.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2eanyyaaf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ahigvvdm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2eecssnft.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2cxoqvuiv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kjuplhqa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2lvqirnpj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2kqdvvatw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2sscndwaw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dqmlenfa.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tnpodcrh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qjynpupo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2faoyhtvh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ddlexfps.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vuhopume.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cdxnrybd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oepqjqtu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wqvogtds.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gubigmth.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2esmucntu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zcbaziqf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvstprf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hleotzyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2lexoehjs.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aetqrrsh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2wauuubbs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bldfclwd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hkmvpnmh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ctecfkqp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2aeccudje.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lvjbnetj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mevrbejb.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ikhmahbw.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2leahxxkw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2msyrvdjl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hpwmyyem.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qwfsiwfk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bvvvvdua.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vuqrmmlq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2jllorenc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gafiqozb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2oqhqhkxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkztypav.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2yortbcag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rplbfjsc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxikhrru.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ojtnwxee.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2roikqryl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gbtkttsj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhceltoe.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qjfetyhn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hhevfczq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hfylhwta.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yfkdvufs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2zavwrjjo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ftjejnzb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hdvxuzvv.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jdloifup.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tadlpshb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrrgmotp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uzndgnpt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ongjyfbc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iswavlsa.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2qeutilcd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2siikuafp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2uikvuwhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wajaedyd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2azdwghuk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gauuudht.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kjgqglwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2sqxnnnvl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2wnksebog.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sadhkthg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gdjkcbav.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2dgllylgt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pisapghk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xgvcngny.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eljyjfuq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ghwjvdlh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zdtnegii.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cbbzkmce.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xqmmcoes.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nimbwmyy.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nsocbbio.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onkhevoe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ljwafasc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uxhvjqgb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2biwpsluk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zkudsnqy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kyxiuuge.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bjvzxtxe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2assxdswi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zleacutl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cwmrgbam.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tsdgpawg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ehirzknf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2dbffvwis.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hhumocyh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hypcsnhw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ekobxhul.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ldvxuugh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cxsyulxs.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tmzxlpog.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fjbnvjqy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2sefxbrjg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zccscjpi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2krvcqdcj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hbchhziu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2efrhopqn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2eabrduyg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ndaesheq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ljgnqume.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2czmxuxdn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2esjftdou.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bxcfznmg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2miviikcr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pommhzlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjnorqma.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2oxkprcpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tistecwe.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wxamrxut.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ydalpsew.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lzedapyx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qdllvgiq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2yktyslyj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgilduyq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wybfwtqk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ycgkrkpx.html


<!-- 参考信息 -->