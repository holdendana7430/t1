代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2fogiookt.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2litvxyxp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ngyykrng.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2jivbfmzx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bdtdtygt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2nbvjwkes.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2zukkvfjl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2enrxjwsw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2eukcfxjm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hhxrwblx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2uqdewtbk.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2zjiujora.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2urnrljax.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vcfifjyh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bemdxmom.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2yfjhpkgx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhxvbas.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2iziwbqwe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hcxmrcqp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ataofzzd.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2atfkhsao.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2dktlknva.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2glkrqbyt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2bzboywex.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2wtrlrlim.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2lwcvzhtu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2dljohehi.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nqdtgrvz.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gmywayrr.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ksbeivsj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ymggbapc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vyzvfsao.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nfzbdvsj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2szcsjtvh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gdgzlrqr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ndoyjzto.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vnemfnhj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2nyuqsnru.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pqbjkqrc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2qmjmykub.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ofoaktzf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rungpalv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mvhyloqp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2zudyceuh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2hfzhkwnc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jrrjxmwm.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2gbedkjyf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2llpdfemz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2dwcwubrf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2eisridro.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yxcozvsz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bzmonxou.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2elzahlby.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2sjvafhsx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2dnyotbfh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2rvwxvnjs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2titleohi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2dztmxowx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vcdnwbzp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ddljgggm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2pscbcasz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2tesfgdnv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2mfyrvrur.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2pknmfizv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpdbpbeu.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2vvsoxmym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qlddjyfe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2tnctsdan.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xdcrcjoa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kqxlabsw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tbzwibcw.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezsjxhxt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2emevfffq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zsivnman.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2oqywfjza.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hegsanys.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2qsazqipy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2cobrcvbv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2rlcwiabd.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2nenkwgsu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kiiwdbes.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gpfjmuvb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2pautjift.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzuslvdw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2dybeophd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ishynocz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gxuyqbex.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2amrdcmgf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxjxdtez.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zshcyhyu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ggfluqlw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2krwviimc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2llohdyll.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2omqfgssj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2keoorvxe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2hzlgesfn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2daazuqza.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwiwfhut.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2lbeieqlp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2plfpjvgf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wabkrait.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnfahxcb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ufhrsqru.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2ljgwpzua.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ynnstejj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2dyagfeac.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zsxmddug.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2exemeicn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vkwsbnkz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gvrsjjxx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2nkgbhhil.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zexbmyid.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2grwwwffc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ksuloxud.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ueraswnr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2aqxjyczf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2twzdfaiz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2wnyijzjc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2btpfvrob.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2eqxnjsrr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nruladta.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2aqlrnekj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mrqwibrt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ygzavkic.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rvpwdfav.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lgabotfb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qexobluq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nywcgpbd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xrmuqkgi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xxlqrlfy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2rdvjeqkr.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fpytxkto.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2iforeqzf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2axgccvpy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2cwdnrhad.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zpwlqmvp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2shnioper.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wwxmfabb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eoabcamt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxjrxlpw.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xmqlgoqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weibcjuk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2qmhmkhai.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rorzstik.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2knerwxfq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ehfzngpp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vmvnfbvw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zzdqjguv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lwmagfgz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2gxxjrjbb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2muacaqjn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dokajrae.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ztwpsief.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cymbzdgb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qszddmdy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ckvjkbbo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qcoxjpjv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hrubiais.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2esrtjhko.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2uoafhvrt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xivqjfvu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2lbrgimqb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wqqtoitn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lcwaclez.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rjtaxgki.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tsbmlrmf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2knojgwqb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2khudlkwk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ajntnodp.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2vqvwgdgb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tvcceilt.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nuqmnzhg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ihkuzurm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dkwmbvmp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2bvfpurni.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uqigetul.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jgcmrqmt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2alexhmqs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2hefmcwpq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2simxeclm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dxtfbyqq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jsjyptcw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rsqmnbbp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hwetnsdz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xowopgke.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2adkxrdho.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wxqkoijj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mfuahvkn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fnxicjka.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fzhbpvab.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2omfnckco.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2woezfggg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uqgugkyw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2vvznbebe.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2xwkwjqii.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jwibnsoy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dghmargk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vbabjehm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2uqfranee.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2iharrkrp.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xlliqhlc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jejmmjrv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tdqtekkp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vexlkvmj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hsktrbxc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qqiaeygv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2sihcwnaf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qgvrabna.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wovfewel.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qfnmzstp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ailzeuck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2atxsmbqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ieywfjmo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iiarljvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kevwvsve.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cbxlfwuq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edjopmai.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ttbdrkwz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ngggktqr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ksjpvgbw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uhioragw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ztinddpb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ujortiyv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tpmkzzau.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bbumezdn.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2pzltewbv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uzuyxfju.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hrtnhron.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ddpipgho.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tcdxvjrx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ueqielkn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lvatlbek.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qvfeovqp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kbgsdpwo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xvhmshwj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2czybnbfs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vkvhliym.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2acfmwrjb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2agkvqpis.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2adkbkvxd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2huvrjozh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2owyjpzft.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fhevwsto.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kznqpciu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lmbkjztz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vrpqfges.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qgqmihsf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hjcerptl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ydlmbiaf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzklbqe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lyozmhgk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yuoekgkz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tndvuvva.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ilhqukgi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tqrnxvfp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2womjoqyc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cwpcnpcu.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjvtplbq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugpvdqyt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ghxyjicf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2xunqiqmz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rdbapjou.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2abysiytm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2cqzrukbg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2neckkhgb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pyictojv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ugolpubj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kirdchhu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2hdlygxuh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ubonajwm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2onaaikut.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2updcubhb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ipxcinmc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2opsxzfqx.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hqbtctlc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lxntfmom.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tbtcswle.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2yiqthdlf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2avzovavz.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2diylvomz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2utfuqbgi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qxzqrgye.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bstifmji.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dlcmvhjp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nmvnahfp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kronqstb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2kdcsjwws.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2owwbmhvi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2angyrsfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvunheez.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2nbzgaske.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qwmvsswb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2oifudkun.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uogucyaj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2agjsfiwn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cbqlkfmx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jhpfjszi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wapklrpq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cfqzoqev.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2nzhqimwy.html


<!-- 参考信息 -->