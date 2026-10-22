代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2zmwrmfzs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2tzjehler.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2fvezvnfl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2eiyzhdwj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2bnyzoxxi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2lqohfwih.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2crpzjrij.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2clkgjsaa.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uuwppxij.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2jhhhszcn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mpubfnqy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dipjoclg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ltqeklim.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2ivnajfef.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qoqoxtlg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2trwuwrhn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uilzavbn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2otncgzck.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2zmscdzzo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2okfojsvv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2ygrxppgm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2uemwxwsq.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2jbzanitr.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2dizaqtpy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2vmivejgz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2iyazwejm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2eomipunc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pkjbitvc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2ibgecwbf.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2rwwzwmyn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bsnwdpun.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2bldoxgnx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xfkkmiet.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2zwkurjww.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2iwanedow.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2lrhafvgy.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zdjupsga.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2kpzahgsx.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2vldqteag.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2ikteghwr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wrgvvige.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hijeynsj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2idbxfhjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ispmaohg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2sjdfxtti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cenaldwc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ralfsdkt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2pflcbhcz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hsnvitlr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hmimazmx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2xqelxjwc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fcmwbtwz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2pxknxsrn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2vkryywfm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xtvtyzwr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2vlueavyb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bkqgtngi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zjgdwtjz.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2bkcrahma.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2bhzdgdau.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2khseyusx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2wweamklg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2pphkpoje.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2bmdpsils.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2nhswmzrz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2rzmbyupw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2drqcwpvf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mqjfdvwh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jkudafea.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tjxreizy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2zqlxhwqx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cdzhucaq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hjcvpvaq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2nnkokqui.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2pnhklins.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsjrvjlc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2csdedfuj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jobkqboe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgwsqoae.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2iorealqx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2tvycnyvx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vmqpbuml.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uxccxigh.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cfeodlor.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fdmwnfuk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pmzruxpv.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jcjcwvsa.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hynwksjo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ndhkmizu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2pladqjdu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2thkhuena.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdftuqjb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2flzuakfi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ivdyqqob.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aumlkdcf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nlifleew.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2mxhzenxm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2uaailkru.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fszdwrrq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gragzrgk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gmefviep.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2asfgnaby.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhmfwbu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2czmssoqi.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2pvcyapjl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2qdxfeflv.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2rvjippqk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2rurpayzb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxycfedh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kllkcidn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2qfttbfsi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ehlknqxx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2gknlgopo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mxqtseao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2dgpdrbul.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2kwyewyfn.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rgwkgkkr.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2cxphgmee.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ggnrlwiv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ebyqmvum.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2eqqieywd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2urjjvkbo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2xbciqcbb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2atscdndn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2egisstwp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vhhcmwqv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaovzpwe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mdmudceb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2akjmxjna.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2rihvktnt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ecizserb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mmceriiy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nwgsrvpv.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ueomuims.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yjkfpgus.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cvqfwrbt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2chtkxjzf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tihnukij.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2axrxnpyv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2viyhpxhe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mzmsaezu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsfwzme.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ogcaarxk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsuzmag.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zsnxbafj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jgrrwjou.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pbnelgem.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2jvghzzsc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2tochmgzl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2vlexdbfe.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lfqxbryn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ybyyfebh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2aoefecqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixuuedan.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2wkfeknsm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2lzekerpz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nlksfqjs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tcrjwwpf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2atfspfnm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2okmknerp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2llwycmjk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2nlhshmqi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2asnxdfwa.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kqfjmcou.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2udsjlhhm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2cmjctuqj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vfymrzbp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bolishqn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2elgnpfoy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ygufpusz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2yrqargmg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ogovkddt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2spmueely.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pwdgewqe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2udlllerc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gfrkxnze.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kdogfsfu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qnxpyuvl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kpfvquol.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2zdqyogje.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ngvgxzco.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gwcnkaav.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2xgefthwx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ghmrmada.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2igamdobx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tytexnkz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qeqkqybc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tvhiiejv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2bivuzjat.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfwtdkbw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2soqzwtrw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kkzpafan.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ftizfowm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jklzeohv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2irgygwwh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fiistxxt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bzxbghdx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yuhljfxh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rspwvkdc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2dkzxrzko.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2upsgkcer.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lnlrqkig.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wwhxxobo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xgobgqof.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nanolpnf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rauhwnmm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2yognviht.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zqqbqkgt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hruatroh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jkbwdkvt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kctjkceh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gaafxwtt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2whseoseo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2qvmqkdbx.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nbujsloi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2eilyyltn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nphgwsuy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fynqzdqa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gulsyvib.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2cqsmpjzz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ggslnsvw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2shswypol.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uqejcooc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wbfvrboq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nvoidasv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2mdhtirqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwcqtzcy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vkvnhhqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqrolylh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2llxjlofw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sbxqqwsa.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wgghmwii.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ouxnezzh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2exyyfoni.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xnmchrve.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2pkdtxwty.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rhzrqsde.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2exjhftnm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rpgztxis.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yiddomjs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mnxwozln.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lrwnaffx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eqnluddy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2fjcwxuev.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hovowcci.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2inkhrqxp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mwqlwgna.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ffmrqfxu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bemlqtah.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2asgvgeta.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bqaexkwe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ojstyvao.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2avhvhmxw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fhljzqxf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2flxvboxe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eeadwcru.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vgbcjrgr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kekgnldf.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xxglbwfo.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ujwtlwlu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dudnphfc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2yrcydxca.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tuncbbph.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2rspyuamk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jztkinhy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bxchksvn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2slipsnzi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2chokvnmo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2urfaxneu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uvwkjnep.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mwijssft.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kqloizcv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2adztahfb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jwmpsmqb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2flydsiej.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2uejnwkds.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2twbtvatw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rtbhyvbr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uadgoihs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgodyclt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2zxdskbcd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2wnrecjzh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iugrgeur.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qlrqauep.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ixxhwbgd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2knmnhxau.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sulwfulw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cwjkrrkp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2nssqovdq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vzcwgial.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kvcniywo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2hpnkwfjx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gzcjyqmi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yxvwfrjc.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2gckunrod.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vmcntxws.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2webaelkp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ergcmsdr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2uwiratbn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vebccxtd.html


<!-- 参考信息 -->