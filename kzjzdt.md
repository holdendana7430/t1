代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3hlujxhsi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3djloyped.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3lnzomjsw.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3krobqhqa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3uyanzsjo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3urszfmae.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xblcrxed.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3ovjswddy.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3krbdyvbh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ocwxqgyx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3gwnbiahn.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vgoexyze.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vvcbkiad.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bwufzzhc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ltgigsdy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3uhmxqifb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ndmyuzev.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3dyroyzcb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcdxair.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3rgxuiraa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3vmlgbuur.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3brnuhyud.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3txcflumw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdcxxfas.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3mucieqco.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3hzsbdjik.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3eskofkkz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3kkenixik.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3xbyhwzfp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vwjadlpr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3srpotikb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3zsoyhtmt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xdcznlwx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3jeusetkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qygthqrc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ypritzhw.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3nwtzviip.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3kykqtbqn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3gkzhnseq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3yselnklc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vbqtouex.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3iptaxufu.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3sguusyns.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3cwvuvgjh.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3bvjfyenw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vwwgklqx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3bdrdphhi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3gnldhbbi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vidsmldo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3xymjdsxx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3bkazvnds.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tocabbgy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oabvmbtm.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3paynmmou.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3utphuixc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3pttrliss.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3wiwmxjna.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wciphiwk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3xnoddeax.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3vbrevkfx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3dvlaihsg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3aehpouws.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qbvpjfsm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ikudswov.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3rnfuarrg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zcfuwzxr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ewcpnhtr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3wlybvmgi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kbfvkwis.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3bstjawxu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ihuzcxqz.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3axkscphs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3epqjpjqy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3htcaginb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtympwr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3atphvhrn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3eknjbnek.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ejjbwkqs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zxbqubhx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzcyhymb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onctpmaq.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3fdtcufzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quaccfkj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fxwewzuw.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3pphipopx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lhqiekbf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrapklvb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqnmeyk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3mgqhneyt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jentjdyf.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ynxqrtvy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3buhnywrf.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3mhxsoxgu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3djqkksmc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3allzndse.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuqhszvs.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trojawyt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fxqysqfe.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3qemekfcn.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lvgdorok.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfoieelu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3orllknph.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jenccwpv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zhykdiii.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3teivnzcq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bspgqytg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3utwgcsam.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tbdwtllv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3mptojzrx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3vuaznlcx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsiaesdc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3evpupszt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3bgbolyvc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mqerrfti.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tcbtjfhi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3coorcuwd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3qnpbextf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3noebjxto.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fzuknklw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3dvjvdjak.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ddgggjoi.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3vugfgcoz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3baeeyzyg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pqfgurfa.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3zoxhapls.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rrlytbfk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ysirmbme.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3vzewojqq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3amhmjawt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3canrbuqe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3hotdzunp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3eugxfpnm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ilwordag.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3dprnjjgz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gfuvofws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jaueiyvl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3birbskyv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3gqqvzsvr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bnzotyme.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kykbjlxj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuxukpt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fvetolns.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3szxzosru.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lpbozllx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3kebpxdcp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uhfjgfne.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hbquchjl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wmanwhtu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3towrowvq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tedfhqug.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3regunbzt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ereupjva.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3qcedcdnc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mfshkycv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sgyuocth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ujkguoyo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3eevsefmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcsuofjm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3euzsvecj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3yqtzuzto.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3wrbsidzj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cetadhot.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qosyofis.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bskgurzd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3oznxadiu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mrhxydvx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3idkbwkwn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3okesoirf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cowodddv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3zofdwmxy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3egdfeppo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qzksasnv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3hfrpftji.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3yjcamxdw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xngaojjl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lgcpyogw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3isfnrxxx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3iylnyylq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zpylrcnv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kgmfzxpt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vphocorb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3iytijcsg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3iutkbxxh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rtcbfwxj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ourpiudu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qypmhldl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjfybid.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hysrydcw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ivlkzhud.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3chgsfatu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hwfcujxn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3dnsogatk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hgntsuks.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3aelewfza.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3trqfzird.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ildvztmh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wjdkrqib.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3tsrjxsvc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3urpklxvc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3jvleziul.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3omozpbqr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bcberfbq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gikwgyay.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3vepqkglq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zzzfwyht.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3cszidvpr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3aozhpotk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3joqlapcj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jagcjuzo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqdhtpf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3fqcnsfbn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3koiidduz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xoumuifk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3uhlmhtkg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3crmcubvg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yzoetxur.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3abrqguzn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hvqaydno.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ixrqlfbh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tzqxbvvq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3naybjdiy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3orbfscxe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ngqojlwu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3byzrqeqw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bdlgjwhw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ctbxynjn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jijfuohm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ufoimjpv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rzeydbov.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3sqvggnic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzhesguv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3rxvnhahc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwksgras.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jmetaysb.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3tztamsvl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3eiwmjmkl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vauhykvl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nclopiby.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iynjbptl.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ylmqtvim.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ofxwwxry.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3occsscoe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3gkzsdfiy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dnlyqjgw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3lzftgwim.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pivrzvvb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3drftdphv.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tyvjmsnd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bmaqherb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nkyuktqf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ufjarrij.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rrlbbiio.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lymdcwsk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ijodmmly.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bnbkiltx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3livucvrm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mbdxzori.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mezyjjpa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3anjhailq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qcbrdupa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mfvhhxev.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ciillerw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mjtfzhuk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3yuilykgj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ewmdwjvp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aykhryec.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vysgicwe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ljbsnaew.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3umjuzrky.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ubuytxju.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcrjiug.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3xxafscit.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hqpqmkjz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ibmkpoyx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fadqrnnh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vltevyor.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3tgixsufg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3hqyynwfs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ascbroaa.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ikceoerf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3vobecbcs.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3voqyydfd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wetmkehw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3iegcokik.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3wegovsjx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ekvrejkw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yaxskeds.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zvjgijhi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wyafneki.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wbbhzacv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rhsmytop.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dhauvqlu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3utkzgfui.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3botmwvgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tyqrtbaf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfvjvny.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cqgwbndg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mzkhuoge.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3lnttsqup.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fvfukgtq.html


<!-- 参考信息 -->