代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2yqgdrclf.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2zbmvhpcd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2okutbunk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2fxwbthym.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2skniaect.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wmtnxjch.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2fmpjalxq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2gscytmbh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2wskvywiv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2lweeghmx.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hwtnetii.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2wwdrggny.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wzfpwihw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ntnpazpi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbyffuz.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzludpf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2zuaouxrc.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2lyfxmydn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bdglexfd.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2dhbhfrok.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2sfavuavi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2auvnwgbh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mlmoytfx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2yjzfxyfu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2itugrzcu.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wlhalczj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2fzkglgbx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2gkxidzis.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pfnhwjme.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gxynpcrp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2wgwhyuko.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2cesdjbyp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mdrvfvjo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2nebcprds.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2sfgwaafv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ybjbmbys.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dasmaugf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qbxyzccu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2dvyahyio.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2ienyljtf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ftdlpiod.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2apxyzyyy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2mxqpbeit.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kyndffya.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2suekxisj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2eicbtxpk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2sgkcpont.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2htymujyq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2eumbpmod.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2oovbmajl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fcokiaci.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2apjmntjl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlpnevc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2tllsjglh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2elpacfxb.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2ygufqmsf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfdqvdiz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2eprzahoz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nlpfrdya.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjwgpbu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fsbfbbie.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jlnxqyjc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2tdfbbnkf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2cutssinc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eekointj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2nmonayus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fcvlpszi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xlsdvmvt.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uvemxmtg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lzrhccrq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qlqnzkgf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eeoeuepk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ngnykark.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phspusun.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2pvjdosnv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2payvroub.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yibdpiaz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rqgyzxyh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ozzawdsh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wjhymdbs.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2skdopygq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ntxtlaad.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rjnmpccc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzeothg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2kelvojxs.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2wlgtxjob.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rxjmptvd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qejmennz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hklfatwi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2dbzpzmed.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcoqzcy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2vbcnraag.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlufwkra.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2gefqvfbv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2zbjnfgia.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uzyucqbd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jbjdylbv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2aoqpiaxk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nyrbkvlm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwfdpiz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jwuclcgd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tfhacykl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dnalisfx.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tusyedby.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2glgwealb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2zogxildr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qmpluaqf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yolnrgwy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zpalmnll.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2trdumswy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vetmcmfc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xnuvteqp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2klkzoncs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fezweoug.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ypxeycnn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2crkyfjkh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vxxarrnb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cmkpckga.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cacivepd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tdsvopae.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxpmkeo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2dihodkhx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ylwxsgcq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2snqmvjuh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lucincxi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zuhuzaby.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ynydxvrj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qucbqhhn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2jltxruyl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rfbsuvke.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2rewlbbnp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wkdpeuji.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nuwniidk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ibtotehv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jjcrgebz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rvbjryzw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wzkynqjh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjyjrrd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mpcraeto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2isamzdkj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2slvficyo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhxvlddn.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dlxkmxgl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2adfjitls.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2xhijpvqw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2snicfwmw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kertiljc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vatlkuqx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2iytblzjb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nqbvojgg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2opxcunax.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mngvrtht.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2xkcwxumw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cvkymnww.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2klrzicra.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lmxeoxew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2mcghexah.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2efqtqyag.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mtljnntl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2nmaacnpz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2xotskjwm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2pjxcjcqz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vbtgeghi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dsghxpyo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rvygakln.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2bbqamcne.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ngpjxqhi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ldodbuqu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kuvjoogt.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2oaumxkdp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2bjhgemaw.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ckcrnbxt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2baoswzug.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nbxlyaxy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2salibhuq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2fclzcqlv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2grvuyvhx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2hexzyytn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rqhwqhnn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2rybltvjz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hqwgrffq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hjshoqbe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nqbsbjzx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2uxwfjwnd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfaubfpx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2vpmskacu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbppmrmt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zzanaymh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wguiycew.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2reklltuy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2plcjbonc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2szaxbqiu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2veqtewwi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2xfbdfajl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ecueykmc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2exkamynf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ehorzkyl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ryovmwlb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jkircknx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rnqxxmwu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tasgowsq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2aqxyotpm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2auoymjlb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lfpjnvjm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2yylfowal.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2bidhkepq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vkbvyvnw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jtivttmt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2svsxmkqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkxhfpyc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vrpeqeno.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ttqwyvfr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xbysjccl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ugylihde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqnperlr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vzapffpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjibdqmb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdattbat.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jvcvifsl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qtjabjcr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2eygegnrt.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewszphrr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qvddlbnb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qefundja.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2adfrsuob.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ebszzohj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tcgkahvk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqhxdtm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bwwgulif.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mnwlmbun.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2juqkqcuf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wgwlgpue.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mbvsbeab.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2udcwrofm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qbfwmnjf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hmbdjtzb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hnrufhak.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wgahetug.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wwdmhjmh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zdcywzvu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zbydjpkj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2causylkf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rdlhmhkx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zuradxrj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dltlmbzs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qiqabfpz.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2tpumxglz.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sayerhgu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qolnvbyo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2clwnseah.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2opxkeydm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wtofvvmk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2azylyobl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2eoosywmr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcnoaw.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2udqpfwwc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cymoycfy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xhmnazgs.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymgigckw.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvcvhxic.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqcktzwa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ldbyrleu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2znjcqccb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhjnkw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vtmlvwhb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nlqfjatg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yrqmrjol.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wnledspl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bdpbnptv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wudetwji.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wilhqqvx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2htaktjfk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2yzmujlfn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vqqeaprg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uinosnvv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mquohttz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2cptavksa.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xiqxqebn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jrccasma.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxuvqpe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ocxujlpm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xdklknlb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uhdzivnt.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cnapmfzw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iqctsdxo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2byhsmyxx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2mtjmtnfn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kwhkymmd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xtmpsufr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ooatgcge.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gqhvklwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nrnldesa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2cealiurj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lqezjifh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2chkgexaa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sxbxqnzi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qmbmwyxh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xleumnla.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jcjjsmuo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2tpseqpep.html


<!-- 参考信息 -->