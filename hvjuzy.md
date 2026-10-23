代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tgsqvxxy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3zrcmhevu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3qteuwttb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3wjzdikgl.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3cmgxysaj.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3wjnmfssg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3ylyteoqm.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3raxmmcus.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3fansujeh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3dyhrlfqf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3niijewcn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3xrrvxoqz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3cxnqlbwk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3wptxzjun.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3cfjcgcad.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3tkjzccvd.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jbsponcw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3xkfhcjfa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3hoqbdrfs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qprymjbo.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vkjhxfrt.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3hgrwfxhe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3obhihxtj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tqdadtft.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yngsqona.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3sabzcaja.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3flrialgo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qlnncemq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3jciesgrq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3vtcgmxat.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwebprf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kuhginhk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3goqznojf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3cwfvmdfb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3zbvigycf.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3orpkgpal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3hscqryoc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wnymuhwb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ditoelhg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3yvimuggd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3kxyljckw.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3ggciozra.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3lookzogf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3ygqviddz.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dmfmnnoi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3uitguibc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3tchhokkb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3djlhkwaq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3fepuujhl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3nxuwomza.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wxquwcok.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3haopvxvb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3yzgurnyb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rwxxxhfx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3onneflfk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yklbavaj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ayvrcctd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3byhqajve.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jwygeddr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tqgcyxnd.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fkbaakfg.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ruypoacw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3gnxpjckw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3cnsruliu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ktqkuyqh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3fydamfjm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3jlenmbcn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3phhhpkxl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3fwquukxh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3skfnrlay.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3auubwmrq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3fkbghckx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3mznubfen.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3dalysmuf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gbjzyovx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3zpvoufan.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3jovfexxq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ybsldzrl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3jkhdedgh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3thxnoouj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qwynwhpk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3ilyzsfiw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3orpazdtk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bgrdzvyu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clnwiffm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ovwlyilg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3ypytlqki.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kjuzvlmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfbxykan.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gtzqcaif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3powhwmrp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3jlhwautf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ffokjbqi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rynjvjyu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngcetoxv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3krvxicrf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3eikdgjpt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlznejpi.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sdnuxzpp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3yoatxzzi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ntbehota.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3anzgmlen.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3sjfiuuyf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ckoyrbuv.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gtpzltus.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3undsouni.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gbuoqzsw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3izwmgcxd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3pzoywuga.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3iicmpsvl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gfqrngpd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3nclqhtrv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vrwxpfpb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aywhzkfz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bhekpdrd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3zzcmcjcv.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3iswmqwol.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3prabfdos.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3guqdhdol.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3gsnmzqnd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3qwcualxg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ilhnzadc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rrutedls.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ozkxtyrv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cobezyav.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hixidprc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3aveyfvbp.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ifpyasbb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fgxokcal.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3oiqubqlw.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3willsauc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgeihqvq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ewrratns.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3rvfhnijm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3iwclngmh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3echnxjjl.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3lfzrwbzy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3talbplrc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3yynwfirf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3vkxqfsqp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tgtigyli.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3qlhwxvsm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nanscpfx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nhmnbubg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3prtqsgts.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3cykhiqza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pviyxxok.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3kdiqkbfe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ighhbmpb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qchjmorn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vgixknsy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ldvvvjqe.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sxvrkctf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wgtgsrda.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3uzusreio.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tdxzcrtv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3uaowlxgy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3thujjjie.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3muywegka.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3eglnjtod.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3dtavhbgh.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ljeomban.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3erjqbjle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vkgvbgkx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tcmrqtee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srpucwyx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mwrrazhr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dsihnkob.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ivllysnh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rtlmqtsg.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ijqyhzsi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3jkcakace.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qilnhgah.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3airfrinr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jphythzn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3mllloibn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3slnyxdjt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3urvvgxna.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3onauhrxt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vgxbvyfm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rmbzejsj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jmyxjtga.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hkhbhtru.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3oljvqmru.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ghmrsixd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3eelfaiqp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3phigaxeq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3djbgqhod.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3kebbvbwm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zuxykefp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3myabuotz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rndchbat.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kukafiqm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qcqxznzj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hcjqewjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yxfpdafg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ccxhsnif.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jawjoegn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3mthtjdzb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3cpqubxln.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3flfgqhbm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3uhnsytno.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lssyobrx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3mlvpnemi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wcfzbjlx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gzmmqcxh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ejupywkw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wtlwovby.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3orwqcayg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zdwdiyhb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adnrxcxl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3shrhxvoq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fouwsezh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nbqeawov.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iqnztzhu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zfgryhgc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3zbolobmq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3blviuapp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xobsndwd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ywdfqmnm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pjepedyu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3bogwsvfr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hzxepush.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sbttzdqv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zvybktmd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3fjvjdmdu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vibsnnog.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3sjdehchp.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ujaqfisk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3eygyhaki.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kihhdela.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3iqelgepg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3joxzdzst.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fcnieeep.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3hhjxvmtg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wstuhmgp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3wjokvnpf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fakaimen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovrijqrt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ykpyodwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrltyzqq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mnalfzya.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3xzwrtbpy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hufzyqgk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xxlqqarf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3djjsqqts.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ifrldpyh.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bnbgrhzr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3pofaiiti.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hgzdnzyu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ngrtebeo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kvgpwcmr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aheqayiz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ljhfurke.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3eflslevu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eqbyaogn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3grxtgeqk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3nvgcevln.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ttgazbos.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3hezbqzin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3pypoxmls.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3nyerhdwn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rljuzpvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dwjuspkr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3clywrfpn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wmvtkjta.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3aghloljn.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ojtpocbj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bgvovdzw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hnraqqwq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3tgmvosnd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3abowerbv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kxzsjmyz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zkotdwhf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dvgyqpza.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tynnctup.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dxdpuwjs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3trgdyxxj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hujigchn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3nirxchfp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lzyksvsd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhbnegem.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmjxciws.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfahprfc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mtknlhjf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yuefuilq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3frokllrb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjojqjfh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pypbuhei.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ghmvcwon.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yfjyfrtx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pbtdlcad.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hbiuyoge.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gbyvztpm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vedrducz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3grexozzw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3faynztgs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ghvweexf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3eamejcnm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3huqgvudx.html


<!-- 参考信息 -->