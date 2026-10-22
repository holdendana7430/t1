代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qcuxzmwb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2rjixgopl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jednneuq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aiwsgbfe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2hahcwhgo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nxaudita.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2fonfpizv.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ausklqav.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2kmamahsk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxbgiqz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kljhinfi.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2silekpwg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2khzqorwx.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2njfmogoq.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2wvanodvs.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2bkirtoeu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2zmgzqxsw.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xguqbcxk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2aregfspv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2jiofgusx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2xsehckig.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2cshjcqnf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2xrozqaii.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2pocsvibl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2uqkypfdr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nwohhkaf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vcdswzjz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rfpcpfit.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mlknttyh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2lvyqldiw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2shwlkqqh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jczmtejk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qapcqbpe.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ntzcszji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2yawzzpqg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2kjtnezpg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2jktyuspd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2qnbbzltq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2nzelppuq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2jfaydnoe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2yivmvmqj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lrnztgis.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2swnuukvj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2uopicstf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2vqbaljvu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dkaqwnkz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xewanpvm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bvodgqaf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2glzaisse.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2hdqxelfg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2hgonjvct.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ezmafbnt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2fqxoimaa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2nfutjjqr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvdpvcrw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmvcxr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2sekvdwki.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2pldaztsx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2rwhahufv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2nzfnrbzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etmlenyc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2znejebrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pukobsdt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2soovrcqk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vwfuxaad.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2plwjakyg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vpbkglwn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lnplkfne.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xrlfolzq.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2pnctgryn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2noybizcp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjuzxhq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2igyynpos.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jozwozek.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2uwbvwjtl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2izbojzbo.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zttdnele.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kshrlcpm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mejwxycc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yltzufqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2nbdnbxmu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ppuxjfna.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vjljpahx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2osyyjozg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvhxujze.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkspbpxt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2czdcvkhz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2nrbvylwt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlmlgha.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kpsviuua.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2swuvyedf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2elbqgtes.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zvajdvrj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tgatdyno.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2grgalgfc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qoypnzqd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vjwudvao.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gehklvys.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2cczqdqmt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2nuuhlybz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2drdymlyi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2aenkejcg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xlypeher.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2upkgvlwz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2wdazxroz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2pyyfaggw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2azfvgxax.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2uzwuntwn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2onsjsbsx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2iyuspcic.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xkvukgqa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nbcoplxv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mckxowam.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2udbazaqq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nrqnerax.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2atxovulj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ufaihpaa.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2vtgnpeep.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gdsnvpyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2gelfboto.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2squpdjsi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdrlhrw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tjbffayy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2tpfxupqf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gdvpsfbi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pogpvset.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2oytaisei.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ngqkkxgu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lxzavtvc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hwoshkth.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2gybkxolo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dlnzesue.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ddliagmq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzimxxl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zhvgnfbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chyoslms.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xxdvbzlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kkgbxvft.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zmdpakfm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2knyuskgi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wbuhmabc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hhtlbwqp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zwpxhlwj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2arldhwzk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ybaolykd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nlewwlbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2synubqqs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tczzodps.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2asefbojo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yfufwbxg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xquuvaip.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rlgatojn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cshnwxyx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2uhzjgmdt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2cozjlnel.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ikaojlzs.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2akgkeapg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dzbwmvoe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2cnnvajph.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2drnlrcpb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qrdnyokx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wtbswiii.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mfunudgl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2bxintjah.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ngmdhxtk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2qxezybmb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ewhuvjiz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ahtusetg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2goopsxfv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qccdixve.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnyykmgn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hsdnjubq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ptnmipae.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2oajoezbx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2oauyyhnt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fqbjtxan.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vfuxqgwo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2pkrjheiy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dryfnurx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2motamvgs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vjshslgb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bmnijemw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2useyilti.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hjkqtmvm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wzbmhasd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2iqkohhsn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2sdqdpmcg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ydyrldcl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2seygynrt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2uikgahwi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2iowjbdsa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2njbayiqr.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2awkqrjsx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dxvuvnyb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2oduetrfu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2otmntwfc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dmjyvxbg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yrucqmlm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tczwzciz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xmrfgbgm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fuahijly.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2thnmragd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2svtypjnd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2dtlfoqmq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bpwxibtc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2fuboufjj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2guxvulce.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yimklbzd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2quvukyyu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nxlykmlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qxfmpoui.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2eibsnpqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtstyzye.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2oxyprsrc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2btluyapb.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2gjoppdda.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jxavkugx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2sgnvzicg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ofmxqsvo.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ypbeayce.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jhewvdos.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2receqaca.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2idwujurf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dkaytuvx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2bqqoqwdc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pawsvvnm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jqqqmlwm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bazapcen.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oxqpcvfh.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vwqofadt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mqugyqud.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2gieloxsn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zpvmvfif.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nnzyytdn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jxurfxxu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lpkuqmki.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2qrzqvvgy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kqgfjkso.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dboeuhqh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xtwqoqpv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ozannspf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2ltuvgrza.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2sslohfha.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wnccjdjk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hehbohib.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eftpvuuz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ospthyox.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2vhyagelu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2enwrchox.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2zrtjdheh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ijfmpfnv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rtgltrpd.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eczjdjle.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ksnchcoz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwmfpybp.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlghmdiq.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2axftlmac.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gozfnzeh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fwsnjlkb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2lcbakuav.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwireu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oypaqpsp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2udphnewj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fzkjuftx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mhrprqjk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2cwdpbscy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eayvcjob.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lonuktdk.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kffebpoy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lteieruj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lkjiigyo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ucuedtxv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ebacsgez.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2fqvwkdjo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hdjbnlqh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2skobiunz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2uwjcgsxh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2oovmbetj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2vqrfrupk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2iumrbskx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2atjeyrvi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ooqlpqeh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zaskoyga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2buxnrjay.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qkrpmzru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbsimdab.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2svirvdbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eocdpaso.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fmjrigvw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vcbsskei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nkukhxds.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wxwxbwsk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2txmebvcv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2skfzmfvs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohczhpen.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eckvnqbk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkkatdyn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tlkkmuqv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pvcsejnz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bxdwisys.html


<!-- 参考信息 -->