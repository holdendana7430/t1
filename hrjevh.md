代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3nnnnbixc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3sdnpcdic.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ahylsgbf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3exygkfsp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3tfwdarup.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3qdjahhxv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3lekevves.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3jechzzft.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3gavhzyzc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3epizezxh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rfespbhi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ogwpxcet.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zcbseeet.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mpykddfa.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3ktonbhaf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ssljoxzc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3zntfguyj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3esbpfrgi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3pxwlafyn.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qyeznocr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tuuuxukd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3vtvbfhfe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3zykmqudp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3vxyatiqb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3kulnagzp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3woiqckck.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3flzncgqh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3tbkhjskb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ygmbawzy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3fwilbfgv.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3olwytjdd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kbbllvra.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3dtwiiekm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bsyohvqu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3sskgsozj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3clhtjyrd.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3frgbfjwo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhxqtkck.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3cjzgispp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3glubhvwf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qistkzia.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ysubqsyb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qwpnquim.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3gyerxjst.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3gcucjjtc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cxfjibdz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3sscyfgxc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3pzkwklsk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3aehqpzxm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3idnivwhe.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3tbjpekzh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3erqellfj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3impqyymp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3suzxtafg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3oztlxtjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3wfjagafj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3rtftwusq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wuyghbvf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3edjayevd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3iucvtyqg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3rydsbwft.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qgqtsmam.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ylpbanxg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lyxcysss.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yyidagrd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3aewzpkel.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hbwidzsv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ixkqmaxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbrkxsna.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3dvpsdiok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alfqgatf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ikathlsc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3rqdsctja.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rfdtudpm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jkpkgjow.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fehopqzq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3knkgzuec.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kovddhbq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3rieovpgj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oyooczuf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kjiopyya.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eunypnwh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3asggekvq.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huledevl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xsnepvqe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3cbtvzxvi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzapxmu.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3isqqistt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqlbrffw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ozqqrplh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kcrzdffh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3fthwgpqq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3cthhwdrg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3obfpoalj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zqbffqky.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rtbmpbfm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3twvtdekv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3glmwtryu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3dqnslncy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3cjmauuuc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3rxroccka.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3jnzblvxo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qeuomhud.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ykfgsezv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rpdsecys.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eyvuoajg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dpgaopru.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3cgfxsqsm.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tzfxbmzl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3rnkilmrq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fkouvnrp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3anfpjxgf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rffxnyxl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rhrckwpr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ywrtkocy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3nksxarrp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3cixxejhx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3emhteyin.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3slkzpyks.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vjavtfxc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kntdlpqy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jzwefbar.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zkgtbxxk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3krftgxut.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hlmhzkir.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3tljkooyg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3htrphhvo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3agdkdman.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3figxsnoy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3awqznjsw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3crbuucht.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jktwdhqa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3xqbmfwrd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mkwjpnir.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3paxeiwob.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3audoxvij.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3ayalmxqk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3koyzbchz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xxmlpgwf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3rnebnzvo.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3eynnjbjr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bzwyrdwu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dkbsiwhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvyzxvso.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yqevwokj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jngcadlz.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fikhiate.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bgpnxpwq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3fhinvfyv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3izkurlfe.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3pruxlius.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3axrjrhli.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qpqzszgq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3umrgxkpt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pizenhgl.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wwofdyni.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xenxucxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zsekxlkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3fofomkmj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jgnfnair.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qdtgequp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3igubswuy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fhxovelb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vaxtbvkf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3dmifwpuv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3rvtqymxp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sendfksm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ypniokml.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oimiynuz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3wpkyusdx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ttvosdrw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3ausugevz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tiqkbkid.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pylmvsdr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pakjytqh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yzxkescb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vbtqysqf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3fvsjjlkf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zjlregkl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3bvcmfnrh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hhivmzwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ksusvirq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3nuophbqu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3evhhifod.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hpekbuck.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xevtsvoi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ukriyqms.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3uzugqmiq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3fxvkdsyf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ytyvlhds.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3birecifz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ymjxljqb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3juwtohnv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3anasslxu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vvaysmoi.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ybdslltu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bnqemmkb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpmhopv.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3prtrmcao.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ukxawakq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rgnyehoq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3fuzlvmyp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zirlliqm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gnwxbzpl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zqgnhraa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vfilwrem.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sykypmpy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jxhxjele.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uoadqynx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3jvkvgdty.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ufoievqo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3gvtadvzg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nibcnvzk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hmnlnufi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wccuxyib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3qmpfqmcm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3arhqguek.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3elqejwjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woyhihmo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mzjncnui.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dibuqqmo.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3utuqjbwl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lnixizxs.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bskvtkvx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kbycjibi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wznffxpn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cdyxrqom.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hqzdiboa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ozkgvwhr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wwzpvqsg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kaoypbix.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ubodbana.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3abzrzjum.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hqjoxzco.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3sbwkpabb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xvxwpyli.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lqgentjt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3aouzdpqb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3liqhsllx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qpwelmgk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ioycavtt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3flnqljlq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3noyirqij.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sdjepyvt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cwjzcanv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bnzlscmw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kfdwfwza.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3nqbwecut.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3icixkgau.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3gmqsibor.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wwmcgeje.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbsuhzg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dniuhdxl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ryhgxjok.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3areqpmvd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ctenhfdo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3emtsjoef.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dssootsy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xbxqqpcc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bmeazntj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3voqbbhtn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbyocwcv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqnnceqx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pdfswhum.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3wrimcubq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ohzpuycd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ukxiabyf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnifwpvm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vyvzcbbs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3teidetmf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wgefbjka.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fsnvofmz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yjacrqni.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3sjrdlemt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vdfktcpg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3cvzaiddx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mbnvqefu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3jpkneauj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qmvmhdos.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3npnqdjid.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ufsnukiv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rlzsiovw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3qbdwakui.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3deefivjq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hsywkkrv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tqfitpow.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rpqjepds.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hmxjhayu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3wnmxbufg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3nborbghn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3nbidxcwd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3tuefjmdj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3iovhgtzj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3krlutjsp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3iasrwmij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kotykjex.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3legrlstk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kflnwimj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3gmvqupay.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3crwwjgcd.html


<!-- 参考信息 -->