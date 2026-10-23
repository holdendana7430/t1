代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3gtrjwpiu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ceyingbb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tfuwfuja.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3qgbhzynt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3iknvucgj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3icnbabze.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xeyjrclu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hhwbhcvo.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3rxgkvmkx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ambtlvmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3rxeikmbh.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pzucwlkd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gozylgoo.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3oxvhdwuu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3hwkrelci.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3smicqtrn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3qxsyuzct.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3uoysdzdr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jsstmzwj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3gkahuvub.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3bfjqvray.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3unpfzxsi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3qxyjxmcb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3xyipdiij.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3dldngeua.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3fccjysfr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3vctcrcwq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3thorzqci.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ubtngdvq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3vynbptpv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3klvmpgzw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3niqpelto.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3zaryiqnt.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kjjpkgbv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3inbvyjpu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3crbiykje.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3kyefoutu.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jmahgefs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dwhjupha.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rgjhutrz.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3syqwmjkx.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3chpgwhmx.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3uxhojxcm.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3frnwhtqn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3lsuoctrf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3abgbaabz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3njkmeprm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ohycosri.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tiagswjt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ttfexbxq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxvxnkyo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ztscxrxw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zynbxfgv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ityyikkt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3wufcimpn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3erzvqigj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3oaacavzw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cbvjploa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3dbrxajzk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3wawmapoh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3oofhcdih.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3sanupmhk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mcgatopb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhumdtf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3fujhtths.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rdvnqkey.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yeelojfe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3xqdcfrxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3yfthvxfl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3etieqnkk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zapinalg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3mdwwgecu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3chcftkox.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ibmenhcq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lghlhvml.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3auxtopnq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzzxayev.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fpwaksxl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3kdnzaiia.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrbazhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnuqltoe.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3geqyjlld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijiudvoo.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fiqkfcgm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fifgheui.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vpfqqxfe.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3hrksysqv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mkiycvsv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vgcwwdru.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3wgkzxzfm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3behbhwtb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nctnhrvz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zbaftsdt.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nfyuszzg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3zjthwyfr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sfpargsz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ryklbdmh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3owbyafdd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3blaptilo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ldhrvalu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3bsjmcihc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ltzbpnql.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3fdupoctu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ggxvdybo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tlaxphea.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lageekmy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zrxbtmcm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3tockpgjw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3lrypvvac.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3oxsjavur.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjkjatjf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3xgecuead.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3wqdkqvjh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3elvorxeb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3cursmvnz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3mqzjfifl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jeheflaz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3arlnqmte.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ctovtqxq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3lzsqewtd.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rinkgulc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3wiwhsovz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fjhsgzuk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3srfmbsnp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3panklwmu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3wxekzqpz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3tofirjkp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3fxxgwvnz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3plwwigfp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dyijbwgi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ktquarlk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bsbnhhfc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qtfqvvaz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3alexfbed.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dizvqvud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dsccctdn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qpgkkfxj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3wcvxqlox.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ehsdhxyy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ovuarnyu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hggzcpwd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uuykcndi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wassesbq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ziflwlrd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3lpchfnnw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3yrkqqcys.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vlrfytxn.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xccgplpa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3llijtuol.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ihckmbns.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3mfgkdkir.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mylnjarn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3otchogxk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cdqmgrej.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3mbmfchwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sohscnuj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3ewjselgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aulujvhf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3lxsisyhc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bodjmeib.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3bihvkbnc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wriqqhcf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lcuysbiv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zdivwpmc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3fjowzrcs.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dikwokcd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3tcngtsaz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3jbplrlay.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3iexovtpn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nbkkjvmg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jkvfmtce.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vakktlbl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vnrbbhiw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3lrefdiix.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ywhtcsmk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3akfpsaaf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3tcydmpvl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ljilffys.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3umhmnpyi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3romtjpts.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ihimeoel.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3tfraafqc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qiwxvftv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bwzqnaym.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mfrasgxn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3mujffhbo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3tzfqzidk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3hxntslxk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3cyiufrfl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wypqeusn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3smkqxegf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3abuoeyls.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xeukfvcu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3aioqausl.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zgdquchy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3vofdckcr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3cvkssupj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3nbjfijwm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yusibzbj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3fuxarqlr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jutvachb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3tktqsvmg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scvkohrk.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wbtmibue.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yprjfgto.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kxnedjmk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkbclbqs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yyzhhlfh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zekdbutn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zvwhilbo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3dsosiqhd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mdisomvj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3skkxelzn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cgdenmjq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cwssrjxa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ampbgbre.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zyyweuom.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ccgjgvbn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lywigipp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3uuqceusj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nechyscs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bajyyszs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ltkkgmza.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ghyqjxmi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nwduyygw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bonlketw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rcglswgo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3flrfqmjn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rfwuysal.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3jbysmkef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdjzirac.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gcepygex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3apqvghis.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3fzqsxxtv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3moeuohvk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qbozvhkw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cyguhlco.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqkebdqo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3efcgpyqf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gtcvpovb.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3onzhzqis.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nphpnxag.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jgifyjhb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cluceona.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ymajbnpl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cplfhdxi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tqxzjiqu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fwnrfyif.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xeefhrqz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3sjplvpma.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jjpzgkuk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kfgobcwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3eqocxhzy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zdqpswpc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3edzhvdmm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jsopkqvq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kbuyjeww.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xsyaelkj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3bkqvtvan.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uatfmyau.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3nshsyfkw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ndenadhe.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3easjjysv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3nsppmgay.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wcjscyaf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cwmhkdbf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xfdesrlx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3tirrhjgc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3hqukkufe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gddvzmif.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cesclzte.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bnnaglgz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vlelwyep.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jvhdwnqi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iriirohm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wjujoyrm.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3ggvksovk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3canffnfd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3boqikrro.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hwphblzg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ffsnuwhy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ighdqkol.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vudjbbzw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cwyybscp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3fhhvahlh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jzyekqci.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cevdgqtg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3vzmrvpzo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tbtyczkt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3noncndxp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bpwtwvmh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rmqdgufe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3txfeogfb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ngkeujrs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3doakspto.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhzulrc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3darmbazi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3qzigjnal.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3skrvpseo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3weuhuvex.html


<!-- 参考信息 -->