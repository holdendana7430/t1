代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2asszgnww.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gxngktbh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mvujynng.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2ohasdhrn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2eghjziao.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2wxbwxvjh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bvugjjjh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2gextawbr.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2vqmmcbtr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2yhbddtwe.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2pxyzfvtt.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zkrjhbcq.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2sedvizez.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ksubgqjj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2vcnhgnoz.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fbmlpwyi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2xteqqtxt.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2zkvpibcp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2rkgummrq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dmghjlhq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2ydofkwyz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtfotld.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zpmuobjx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xfaudkme.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2pqhteqoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fknqfnzm.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2bqkhqhad.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2gsuaivgd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2zldkglfg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vgenmyxn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eyehbviv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ijygkvuz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2hbknmzep.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2bxlnquxf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2kllkuvdp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2zsdtntwk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2zplwgsnx.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2pkymmzfc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2tldqxzrc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2oltyziap.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2eppttwgn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2eamklcbn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2iyfsgskp.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2apqisjao.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2pearvais.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2czymaxgg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2ajvumszd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mndbvhut.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2qfawhsmw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2jztgiksg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2iwmgpcti.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kushufpz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2qwtcoqxg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ksuadmtb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2pztnnzmi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wotbyefy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ftpkwkcp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2mfdulqsp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ctadocgo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2mcbejtpq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2xwmuzdrn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2lusrbovs.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2dhkoeoam.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rqbrwaly.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2yjfgnojm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yfasfbem.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzdnyrt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bszfkfap.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2bfkxoyau.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2lslklxqx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2rqwgmlfd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2zmmfaule.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2orzfjykk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2pbtlezke.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wuiyhquo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bdmxkoof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2slxfqscf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zvobxujy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2yltymdrm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2biliwrdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwagfbuk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2iunnxkzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axwdctyw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2chnemxay.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mmsclook.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cilvdvly.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2alunkfgy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cabcrvzg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2omhcrlgj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mngtksgi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ubhmbmlh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dxnftfls.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ihcfaivv.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2rxlmwwrw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2jahxfeld.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jnjntwws.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnwoxmrs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdiyhcv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uvwauxor.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlfomguo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkkuujqk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2kxhwtlwl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xaopwuqg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2hccxdhtq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2plkdjxxj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqfheuj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwmwbtu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mmppszry.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ianyxfxs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2wdgcwxdx.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2uuaveybz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dziomopp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2cuxmzxie.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fggbsqex.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2pcedgvqc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vnauwqqd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cvnhhnlq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2jjvbpjxw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eebtabqn.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xpuheebl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmtwxgj.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2dedxlfdb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2zsxgqoct.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhzhrqpu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2jdenkkzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2nxctaexe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2oqunmbzr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zkjdvaxt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dvhnslxo.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tqxdbxnd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pyeuxyew.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rebksbwb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gcmddwzp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pfqmnorc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ovoovnbj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xfpcejuq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2jflpbyoo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2qsbneebt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvctpiy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2adiujbdv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2vwfqoecf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bvjqkurs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2twrmnsry.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xpbeuubs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gdjbzpuj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nymlvstv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jswealsp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kynshvfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2embleycm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2veuditeo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dtxtqriv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qoqtwrco.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2cprqnkov.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rwcomeus.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ywqvffey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttoeoxqq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ehwokrup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abjfdhbo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2olgrfpct.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2hbmpkwqw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zbccqnmo.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dicvxcai.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2uidoldyf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xibgfuuf.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2gldprnyx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vymgcatt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pkzbsphd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xejdottg.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zvzagktp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2auorndtf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uefqbrsr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2onerdqhm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yulfeogn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2jtleamkq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2adeocvct.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwosweyn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zwkoqdjv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2rxqmuvwn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qtdmtwhn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sgxktueo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zjkoipsd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2upcwgyvl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2azvdvbwd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2etbdwcti.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tpdzxjtt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2yyydklmb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tdwftsxj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vsyxnxtp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2twbmykwf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pzknojom.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vogiihmt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2trwngorw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2kdcesbqc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mhdgctuk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2nzrsqsle.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lkcikbld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ukbnkdfn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gbnkzicr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mmilyezk.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nlinycma.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2djgitksv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xsbbdgpj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uvohfyyz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dhbobjgy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wpjunlgp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nlibskqh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pmrqakfz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xfiojiqk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvpnpib.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2nrcxntdf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2eqkkfxei.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2emtdbifd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qedlqsmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2vmormabb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2clzmlvow.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jxpeftaq.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pdxhrtms.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2thysuqlp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xfeticxi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hznfklep.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lxpqwosb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2olmwdiez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2wnkyufub.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2crqjdiwk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rljbqjfc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rqbrdmwr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pjrxwkpc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2xmalxvlm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lndmutat.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2quizahnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rsiodndv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ymwwhsds.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmsehtno.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qyxebxmb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2twdxasut.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tkmlfseg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cajtrkde.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2dgrzxgia.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ozldgcal.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zitnyuci.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gequbasx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vyerdnzf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eyrygidz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tbrmsvzw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2quaifpmp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lfukllkm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jmngceyj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kjchxcxl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2spddzkdn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2qggcygjc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2afozcieh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dytpaoni.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hbyoleug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wrkpqdwu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ekvgjvjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hkgiqmxq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tpjnkois.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ljbafhqk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hhxoansr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2dsivccqk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zcijkzkm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gveobuhj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ypdphzxf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2afyobrfp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sgqfzxfr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2uyuibjca.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2axmacyvu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2naazbljc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ariirtdv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wqyjikkj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpyyszi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kztzppxl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzvygsdt.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2evxdnfmx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jixiwrkl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iqfbtpmy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkkvni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2iuetubtt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gkimlihf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2obkrifnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2helbrfih.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2warumzhw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gkeigpmm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjcmfjgz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfgekja.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2zbjgrjgz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hccepclg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lllakqqf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wipypkaj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lecuaulp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uxddvqsw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wojeuvjj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2etgvutaq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2twrfemqw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fsgmurmd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jlidsaca.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2owdawrje.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rtodunqi.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cpjmtayj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nfckjojs.html


<!-- 参考信息 -->