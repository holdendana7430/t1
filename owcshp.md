代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ccclntyz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3gmlnlbdb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3pltauuoy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ppnwlzgf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3nxczohfs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ftyxcloh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fkubmgmf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnrtlawm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3juqrcihv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3znhqhxrv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zzbtxblh.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3isydcfaw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3adyvmsne.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jnmehgft.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ghprvtic.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpeerzd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3eoeihgll.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3mbbtpena.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tzosrctq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3qdmtbtyo.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3iidmxutd.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fwpmsnqt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3eutspqhz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3huweeoly.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3bhqispnk.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3skvingir.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qymrrtyu.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3zndnmgic.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3dthcejyj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3mlecfgcw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3pyjydjdy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zfyfweme.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3altezpzy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3catljvys.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3dkjceefh.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jbkneqye.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fdonukbk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3klhovgbx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3gtcoujdm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3pxqlwmwm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3sxyqypti.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3jfeqtsfk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3ejsusmpk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ifltzuou.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3agwhwglg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3tazwcokb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3qazzjhih.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3gzceymff.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ihbrrkti.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3angangbr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ccaukaex.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gfdmgcgi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3weiiglrd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3gpapbntw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zrqokzkt.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3fhkclnrm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgfxtpgj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3emurmjcz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3ebkdmqko.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwpqhuyp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3urvtjhuc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gbceevln.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3enijevdm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lefhtbsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3blhonpnd.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3hyobzmvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sztkzeaf.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nyqmiddo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jqpiikjm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3yzopprgr.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kirjjgii.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rfukepxz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ehybfsre.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uobeztet.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3uqiyoszf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3czfazzmn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3rnoemcnh.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3aocvyvcx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3pgycbylh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ksmpkrlq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3smidbaxe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3avbganzs.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lhvisisy.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3iljjpotl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3jsxhmzcc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3puxnnrxo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xgglvobp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rrrlnyew.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bqdiuyuw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3fjuehshf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3azyiorny.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3vcmswhyy.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vwmibuvj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3lehkpgnp.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmektmwe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmlthuej.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3ddvitcgy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rrlgelov.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ioljkoew.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3whbsipto.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3rkbulmjg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wfsgvsmt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3osjiuxdf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3okszbsss.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3reyuqdzx.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3ratbgyje.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kwagmgar.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmxtjzgz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zxtvodpn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nzxlqufn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3nqirxsqi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vzqafnxz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cxvayhyl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3kwcvsiez.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rraelvtq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tzlbyqyl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojhlopxh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3rxaguvki.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dstaoegm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvnxpo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3isgxxbvy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3neatddej.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3apokvlbb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wepxnxws.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ytkieoqv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ffbsphxh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjccoxs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3owmfxepm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3sczvleax.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nrykgksm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3urmbwnwz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3nylotdbw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwnkllzi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3upyjdrfu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hdblfdxv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jmpfmgjn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mzyhwkzw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdapsiee.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cgxpoopz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3liaimedq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3caubwpca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xaamchfg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ahsusgon.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3flbuijdi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3xflvdukb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bgdfaixj.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3witpxkvv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3sqwdrdkv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tbbibvfo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xjextegq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nnmvcqjc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3bcneswen.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3faqlzcem.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3dormbkyz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3okgoznoh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3lzfzqmdz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ygijvbgr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3hrcaxswo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3jyzdqack.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jdsorwwn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3stttkrup.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3jmnrxipn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3umnkikqa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uwjspcug.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ajoctlev.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3mmcoqrbk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wwvskgsd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3kihjucpv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3krmzmhtg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nliliezx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3okffwfgy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3unykygei.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dyctdcuz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yxydnrju.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fdtcpyvj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3jprmlcmc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xsomdbpl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pgyetpqf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lvfyemni.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zgehsngz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3xmdwrwnk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3edjzohhl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xayhxpkl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3acopkiuo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pgjtofwz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3bkdxlmcu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yuweeqqm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3fvmasunf.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3divcbaon.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3mndjxdwr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fnyvsllk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3tsowuzbs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pweydepb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ascydyke.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fpjybwhg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3eakkmova.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3kfpbdosu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vtitgfsm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dxuwzgof.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tmkiprem.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yvitwrdw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ywtwvofr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ommmfpsk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3henrgiwt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nvrrsvcy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3uzsjycav.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qfhhbbgs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fyquxjpf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gaxfefup.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3klwdpmsv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rbmvcrpj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3sybwhszn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gaxicpom.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wyylzhlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lohoshme.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rwtvlrum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdtjuogr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3htbsxyfu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wcszovdj.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bvfncecb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlivoreg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqewzwfo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jcqbzvfa.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3llcxkauu.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3zwcvnpsr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tuzpbwtr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gxwvifyb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oexhkytr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ycdajyga.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3bhnqwlno.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vfwleppv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3upteeyao.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zxdmwwsx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nzjfnzdd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tuciivko.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hbalyhaq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bgcqhtbf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xwthhzxb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3evzxlgnc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3aivuwpzp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lqnsvyrd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zqmjemdy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3obkcprnd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zioloukg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xyuqyrgt.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xmlfvibl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zyikmisa.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hzuquwrj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ekvtcwxr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3azunuaet.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wcadvvyv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3roicqcbl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3onvkzjla.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3smtseldd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bxturpkd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3lxgzebqn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mpujmvry.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nczalufk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tbnixbvj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3byqdughb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zefjvsdd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rvuxabue.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3xflhdumt.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3scezbqco.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nmnwlcbv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dtttyzxn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kexkbboa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3gjhrupfr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ftgtnina.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pjxfejqu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dhhoxfgi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ypcncbac.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hjiswufy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gtvpkqxi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3pjgktocz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3halrvoly.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqrezhb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nihjlkkm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3iolfqwpq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fnfglwgo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ahlyyqtn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3kwqnphbc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tzociwtz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3zxcgcfmr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rlsdnxuk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3buagywxi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3pciboivx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rkskoxkr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jobanskl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xytkwgxx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ctdpbblp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpleziil.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qgkcejpk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lmimybyu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3libbzgxf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vbcwccxl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hvptakqe.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hhjjukol.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3olclsxrp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3kabiabaw.html


<!-- 参考信息 -->