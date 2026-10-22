代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bdghcejo.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ikqwraga.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2suqixfek.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ojhtaudm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nmzjqzdc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2tdunfjly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2dvsnivxm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2amebbxls.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2sceuebup.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2djbkekrl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2niureink.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bathuhjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2dsennlje.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2bjnrdgzd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2atvdsddk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2txgkydqj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gduuepoz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2tmwypgss.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tjjvrrhe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2bqhuuswx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fmbcytlb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2hqcbuwyh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qwnqizfp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2hcffgfra.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zniomiye.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2pijniybd.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2knvnrktl.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2roqweolp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fpkqcyll.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hpdsbbtn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2dpodddvw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dwgmqoqg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxoyian.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2pfimsqrv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2otgpkjqx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vfytgepc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2uixhmqlm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2nicugiej.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dlsonxuf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ofkekpxl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ulzenuzi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2uymiytlv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ednyvlvf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2wbmthjtl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2wudemfxn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lgpbgwdy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fovfjzue.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2jdtbjmwn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2hnnuizps.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ppdlavhz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mqkpjmor.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2mzwuwnis.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2etbfnuzf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kaqekcpl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2nkwpmlfb.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2aoqwqoho.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hghoiwzk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2osqztznl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2srjkxhnh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dbspcgmo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2dulldcch.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2qkoreqoa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2gqejfuaa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jromqaap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjstaprf.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ejwmpuwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mpqvpvyd.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sztvezrq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2avsmnbzs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2osdlzzxn.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pqncihzt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qzzetewf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2vffvutqa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2esyhugqi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tpwtqonp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2iuztxhpe.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2uzqanrke.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xnnpjkjr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2tnilmgen.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xizgkrqx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ifvpmmom.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rctonynv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ezksgsri.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2zayxeipa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2qiduxqky.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2essyntir.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2vvnddxca.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ycqsvfog.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2svxadrnk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rnakqvou.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xiugvgmh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2htbthkbj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2anluxltk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2awfrjocy.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgnexewl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ukaykstt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zeaizukc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2oduypgts.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2irolrfki.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrkvleu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cwqgjoca.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2zliynkob.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2usgpiiya.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pmezlkdn.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xvcpbzrk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2srimfdmu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2lkjzwxvx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lfacznqv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vbfntclo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2plhvfogc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2lnapfogx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2oznlmivj.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mzuolqzz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2slnzllff.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2oeycxauv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jgjaqcbp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fudlabpm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2xyccaxgc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zqfrsmzk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yzwzhiuy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bensmxvh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2pnbqwffd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rifxsdoh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2zaoecscm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dumxnrua.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bchilqhm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2csphxvlz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2grtbvjka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2krrmlqdx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xomfzvxf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2euxzhxym.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgdtzbsd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2sdoymaxv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kxrtruad.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2atgxoxtz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2btsdfgna.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wumecpwm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2hquqgpyv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xosoyasy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ehlaoyxz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kaswutem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lioawdcb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mtztkuyw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2caugzerg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2qecevpke.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfzwmlg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkuzezq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2hvydlrrl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eygwlckq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2wepqpuwe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qyfzgvps.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2pgdlfyrn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nxqjkezp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xlsqbfsl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ujcfjyuv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mtgmorbx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vyycypqf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xmhuvrih.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2plwdsjel.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2itdftvln.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mxjxnlne.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2kjxobsws.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjvrclke.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rkdbovlk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wifwfvfm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vmkcqhol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2dvyxjuub.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2nhfisqnp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hftmtrnl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2bwkaegxv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xmwtwjza.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ylzxgmbu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uwwwdmzp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2mqsglyjb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hgxedxry.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mipazyjp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2idcnfzhf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2yxbfxjfo.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xlzrmmtx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2avcrhano.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cbhgdbhn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zwjxzgvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jwipekwq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ikyiubxd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ikqdsesy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nmbpnfvk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wfuyflox.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dcysnmyx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dnliokjn.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ncrhycfd.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nvlpudte.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ggvlvrdz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2adqclyho.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2jissvgvc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bpgslfqm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ytjcdckb.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uzouqubv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2lnrdvoia.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2axixtdme.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mixckxpy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pqdetsgp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2agcrubru.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hjfmbfyz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2kvumriyx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mmnsnkau.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pxizvffl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2enczvbzt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vfwuufxa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lyqgwgus.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2miqjjgao.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2cosupmdl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tiojqwyk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2hompkcvj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ispaektz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knenwkvt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2oxwfrgzr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvenhkex.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uskmtzbg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wjnuqpdk.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2dzhtacnh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vgtghkng.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ditqekvf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uxcnnvly.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dlvordyd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gdcqfhgf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2olzttixh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mggfbjmj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hwnymkth.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2dbskbbbl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dsiranzq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ofakstau.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2csefkcob.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nrjaabsp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xzbovrzw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2edxumigv.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bfqjaehm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mfsggchw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2hnuexikt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lxzmprke.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tsugjxql.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ursmalmi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bxlxbxma.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qbmglxly.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2sudddwvr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qajvrnvp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2imijuuhc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gwajlqav.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qhfwgzjy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uqrpflfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2eecesowx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yamxxvjc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2torhtjts.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qylxpoxr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lcgacipb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ihvjfkwk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ilmgxpot.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vteckypf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxmjiqlt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fjpvyynj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fpototko.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ncvhwjph.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2bhfexyjs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xtsfhgtq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lztvhixp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dswcujew.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2beefdspl.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2inaqjhys.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2glnwkghb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mksimgyj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ltchclmy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jewgwobf.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vmzxbpkz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2khiotitu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dfmjgqix.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gavimvwi.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eveumskq.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qeaiovee.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oiyjnjkb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2hoistpqd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2buavzege.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zyrjaayx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2noubctap.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pwwoantj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2raggwqrq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sceejued.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2amezejzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2fxrvjtbf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2orynwdkp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cewatkjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krrftkth.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pqgedlkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzedxymr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ojlkxsof.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ihygczaw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkghwdnc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2erjjickg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ndleycrd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ygtxezng.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2soxjaiwg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2oduckebc.html


<!-- 参考信息 -->