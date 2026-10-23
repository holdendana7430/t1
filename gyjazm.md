代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmvnfyg.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbnzsq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nqgunlcn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3txzrgrkr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3eidnuvbb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jccgmhtk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsnywfx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3losrsxvt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3xwhrigfe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ycbrjdaf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3inxvyrkw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3gxotgzrk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rirmunvs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rbyrsfzr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3btghaliv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3mpjzfeou.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vmzasgdw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3edlbhoav.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3iceoliol.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3jvndtysg.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kzrdtouq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3usgljhlr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3qiatglhu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3cbaodvdg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3phdqaerl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3rskxvddo.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3iiwxpuwo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kobgshty.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3egixvhmz.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3esfmmdxf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3wjaptdzl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fhpqjjel.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ztwffndt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlzmqhb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zndvxdfg.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3menokdpr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xyrygcct.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3sjviuino.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3veichexn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3dtmrcnof.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3qvfwyjfd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3bxkvoufp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3rudnlomi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3urmmwfra.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3tjbbeppy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3fkptykye.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3vfppmnvt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3aycfeodx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3hdlzledl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3hfowhwcu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3feuofzqx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3dupnpaud.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3chqbftwe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3isbuswlk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3vdvyzubq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3lnlwtvfd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hjajkhum.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ndodfytf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhlkvbl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wkngvnfm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3vnkrtutu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3msjlvfon.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ypscowmy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvskpxxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3husppcxo.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3hlaazbay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqiedkhi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nurpeuzx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3cetpaifu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3szzsvnix.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gcboqvfv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zrmetffm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3acjwfnhu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3relbladk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3qwsrayih.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrinvje.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3aetrfslv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ajfivajy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zcvwhmnf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wvjwxpgx.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3khkqdgon.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kdlvnqyy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hdvqjqqg.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tjizwhsw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ufqqlgxw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3btjorhhh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fqaccodi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rxqdxjow.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3djuxvcyk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bxvhiedc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zfvqcbse.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3nbekcwia.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3zwkpbvkh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3jlaafpxt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nnavvzlr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3sxbvchui.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3tebcetkr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3nttmgwgx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqmigabp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3sqipfmkk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kzdvzyss.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zpdsezvr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3gbvwlmpo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xnjmyruf.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mydkaxod.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qcluysns.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mdllcrlk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3htaxhspp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3kixtfevw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dcupgeya.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xdvofwsa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3zomygscj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3hlqyhqni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3rtmculrc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3frkawenl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pbkqnqer.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nlsiatrq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3ejlryzff.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpkvleq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3grywixeg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3giwrokmo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgsratmc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dmhgwxfv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3voazujlf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bejqcjdn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zniaqbze.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ciqpkvdb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3davieiwm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xbrmqlnv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mifqdodb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3szatjnke.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3udugbgiy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mmdqggwr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3yazcaote.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3inpaiigv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3upymlbvh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3wkclrfbn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmapors.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hhxquebo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iteugqfs.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3udzmllgr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kpvtfkrh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qcakjoke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3wmzzmnsw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ookrpgnl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3btwfflng.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzlulrq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vuyzkemq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jfqwdvfi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3zwtmhuhd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jeoiltrj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lcdinezv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hzkggmmy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3lmhpaadu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sxapbhbe.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kxxloyej.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3lrofnizr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yvhcnqwl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3nvntnorm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fbvvmiqw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3wuasijad.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3gadqaoga.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3owbzcjco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3llqedfet.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ekytubaj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rmrjhyhm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3poburfak.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3qdyrvkcx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hapmpmmp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3kzkggahr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhqjexl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xkpoxhff.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qumjjzpx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3abjvkgjk.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3huoptvkl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3amkizkge.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tavftoyg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3tqdytwql.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3djrfprha.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gjjrghku.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rjolpkva.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kqvaapxm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ktlhyere.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ytjaivpd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3nqznzpkd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3szwxjydv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3opmrtvux.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tvlrehli.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bgoddsbz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dcttfpgj.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gspyawix.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hkrsiaiy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ulzrcmvs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rqhjrmyz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3jsxzqmvj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3comuafkk.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wezzegol.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdrtvj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3etccgrrb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zcuqhvoh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3hwvyonsa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3okstofkk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hahrnkna.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ekjehdus.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cdibcbac.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3pigyxkke.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3voirlvbb.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qjfdtqzv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3eujjmmdk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pwpmdeqq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ixnnvyke.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3eqzpfyrk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pmzoxhai.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vnshzgvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aieaqjiy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3trihfhfx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svzjevjb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3plhqetkg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ckbapwua.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3nvpgyahw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bifynbpm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhtxscw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fzeaipus.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3toisrjgr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ictsmcun.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3srnikprf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3wgwnajuy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fqhcbuol.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3nwdaybpt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cmhkgcfx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3buejiqev.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3atfarfiv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iiyhzfzg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3coyqsvuz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3owttsnye.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hqxhkwrl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wsyudenp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3keyfyjqo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hxjkoudc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dodslkuc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3zbhxjxzu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3sylasdkz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3tztknirc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3kmmefxsp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3meuaekyk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qaiyrsbu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3iytoetei.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nwsaowoc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jnjmmalj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3dvcskbou.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ugppmkor.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bkbgjmps.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hmjfauog.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3bwcbuyye.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xweqkrdl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ixxyujfq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zwhaggrz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gicovwwl.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pohtykvr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3austcvyk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3paarfnrd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ngzowtma.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tnycblbw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzswrlun.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wqfchugh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3epbsouft.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3keygruxr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dhrouxqb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hbsxybql.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3asgonnjj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wpksuevl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3yeahipkw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3dmkwemss.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3gugqthnf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xxtsnwwr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sqtsbwju.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vitrgvah.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pncnznlw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zgidmqpv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vxlossbq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jbbqpaad.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3snnwbalh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ilihkyob.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3batqhzqo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gudlpplf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3evffmewg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3idxbopmb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hjykjqnm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3exnbhzrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cyjwbgky.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3esdknbyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqazidlz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3afiqiiug.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zrwhorwn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3phqzffrh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fupijotg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ixkdxerj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3llkbjcnf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xqehhcgd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3smdckyfm.html


<!-- 参考信息 -->