代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2jdkxvvvx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kccvmebt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2kgnikmib.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjloammd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2dzggeoea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2yqnnihzh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2paqslfiu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2dnhzuwnf.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2cwgifnks.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2srtwmtsz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2qqnluseu.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfupgce.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ozjjsbly.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eqgmrznc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rynvdtrd.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fwsbydyu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2adkltoft.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rrnwwuvf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2vssmrqgf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ltradlyh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2swwozpok.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2xktaspxv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nbkazvet.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2wmvcatvg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bmtevrda.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2qgsyuvzk.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2kiupjvgs.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2wkxvesls.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2mmtfwbjq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwidzcg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2ixlxmkbg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2usudigvv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ptydjhgo.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2cwgpvkgi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbmvxjl.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2llzepivc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ywnfrulm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2ytuveoev.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2yistwqea.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2bdgqzolc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2lpwolwyn.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2mefdaynz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2kljgmuaa.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2rhmbnswf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2dcntcojb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2daqiquiv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sfadwmgs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ulbcpvwr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zbewipxj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2fnbiuhqa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2uyomduzd.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ksxocjfs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2utxjrvlh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lkfsaosf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2niiwrqio.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2wghtgxeb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2merkubxa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rcjizrhk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2zgmxbddr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2hdzqooot.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2kncctuuf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2oztfrsga.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fckllfvg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsninkh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ydfkawic.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ltximokj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2htcdohlf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2iskajaov.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2vwsrigtt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2fijngsyy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2nhfbibpv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mqcnadtn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2hrrjrgyt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2rudsqwdw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2nkwnmdrn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2epiwiqbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2vgvgrhev.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wheldyih.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ntsncxns.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ipibpvmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tlfvcfdo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2eyquyevo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxhxokpw.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2lpwadvro.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yzkiozur.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zkeayzsy.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhcotoj.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pdrckiwz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2tiaohzkt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmpsuzqj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2jseeogaj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2jhimzage.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xxzjqdeq.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2blmcngka.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2qjdrsbfw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jtemkagl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dmnxyqkw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qlktojit.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2raekdknk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pmuxmjnm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2apyguyre.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2jxoemfuu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2muiyiojt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2lgxuvemn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rawcfzsz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ydtbomcx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkkskxa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ogdjpyeo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vtylcarg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2zoextojk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2txbmhpvm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yozxdbyx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dnurxjkt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vtplneut.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kmajvbgk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhnbqlh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2wfenmbdk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qcexobik.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqkbzqkl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mcunxlav.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rofrrmvo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jthyoljj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmmpeoyl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bdvshnht.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2exitqzkp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2heigddif.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wrmjqsoh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2iahaxjdu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2tfmefhct.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2pohstgvc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2egzifycb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2awzfcryc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2uttqhfio.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2eqgsqyid.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bknoqsnp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ketnseip.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hinxxhvm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2pjjfxiwy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhdrkix.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2jslegwbj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wfatyxgs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ivczhlqy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cczzgswb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dszefcgs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mycqkwjp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ksudjwym.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lmdyodho.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bdixtejx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2wpsrcbel.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iwjffajx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ffpuknch.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2krbnebfl.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ywvivfpa.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2svomnyqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2lwjjgiou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clhtxurt.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2sahkxcmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxbdoezg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ofvbpzwv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2nfwimioc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mregjjkt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ygpvqjim.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ctbwvpxi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2bjfnhspz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hfqhmbgo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rfsiuujy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2jbwmnfkg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gjwrvomo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rzyobszu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wluceggb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rpybkzgc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nsmqyqnb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ugjvqdji.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wuvqsdvy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2daozhfit.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmuterwd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mtgtbvgl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xolmsrjj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wkdqcbgq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ojkbdvmv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ngwurmel.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2syjndgsc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lyhewccn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fwcjlerb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lrvuzunj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ratnkmcr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qagtypsx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ribidyoo.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pslpmqby.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jvvoooym.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2uncvmmtr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ilfjaqox.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bukuwxwo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cgomuhcd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wylerfjn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wsoayfpl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ddrxelez.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gqwhuqmp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eczrroyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2xehpsmnt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2zhnpmusq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ydhiyzek.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mzoalevj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2hbqnrcak.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zvlhaaiq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2htzzsglx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pyuyhfls.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cjtuuxip.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nycjuxgm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2egpohgbu.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jjnwusfw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jsplwwmg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tdfwrrzr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2uqitjzen.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2yqnmrxlt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2rdjplezl.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xrbfmegk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bsbyzhkg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fnpvgbsk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2axzgofoi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xitpygmb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jtctqaru.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vbyoyhva.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vtcxwdcu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oohqphcb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxksspab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2babvzmac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qxmrcxjw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkogkkk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fmryzhiz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xcwsqhuy.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2akfhvcun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unnknxxh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2epnzylht.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dhlgiblg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbuekml.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmuffbr.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2catltlos.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ggmqnaqi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qmcsihje.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rzspxutm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ejfgdazm.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qmhufygj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ioevbqzn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xkkdrgzw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rjjdylek.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hgdijsbl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jndtdrsh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ibwchiud.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2izisdjrb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kdjjfhdq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ztxiltyx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2udqyosry.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zyqygozw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjgzbjom.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wlfzhwsc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ikdrycic.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2wgintjre.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2oxmfqhsz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sqbcjsmc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2yimatuso.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bvqeohwr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2kdfcbuxa.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ldcjpgpi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oerbrgcg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ociypauh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nisaeohf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2geuvlcml.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xmjcenqs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kqvrorop.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwdixza.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbmygcq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lhkxpcoh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uqquwauh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2engicxwk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tablibzh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ssbukavn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2znabsnbt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2nqwngzru.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2csigmuyv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bnarzkhc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gpguvtpv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2phmrfkvw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2blzgsprs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2imoyzxwc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rioaqswq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ztadajid.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yzpnktae.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ufhuljvx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2uesjqgkn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvbnaq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2psaolsos.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2clvsidmo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2jpexuwix.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gzgqttcq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2cahyasth.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2drqhxkdm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kntfzjjg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xmkgnaxb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fibfaslf.html


<!-- 参考信息 -->