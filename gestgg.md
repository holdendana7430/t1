代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cqdrsybz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2jhxvurvh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2qpmrqpax.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2oyybxrpc.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2vbpukuhc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2oagpzcfc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2iinhiojj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yzfnfeey.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aincviwn.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ppbxfvep.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2isoyrnci.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oobeajsj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2bxfbncbt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2blwvfybp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ynwkpliy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2cdvlguze.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2crfqegbf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2brqzvryg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2tjmmccfj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qzqgthit.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qiipbnid.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rwbtivrx.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dgnzares.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ecmlaylf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2xbulqvap.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2owkjvuul.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ixmuqwgf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2uaydatqc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ptcsyfcg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ekmofbkh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2sofospir.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2nzzjojjo.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qhuotwra.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sdixuzrc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qwnjpqxi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2kebjbwhi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnorzg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vyelcpdr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2laovpayr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2prflmehw.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jnkuwbjf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ibknntzy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2xszkdrpe.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fpavgvgi.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vmghtbmu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2eqhrtcok.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ouyzosih.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dtefuicm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zvaboeiy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2qdlmuscu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2pjatspcm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2blhrskzj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vzlrprkb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2oqkkhdei.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2vbgvhsgx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2cgwwckbp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2itqenndt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2qbhqnebj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2yvkklxsu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qqebpter.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ekdtqoak.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgjthzu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qayjtaim.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2bgjjqiqc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2hrscfmno.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ktqcrkus.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2lvxydwym.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2swnlmrbi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjapwgyt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ddznpbdk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vexwxrnc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsfkznto.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udrogscx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2dohmvwjh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2tgzqgopq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edrtknka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gennxzae.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2cjckcoqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2futvgjzg.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eyzrbwmx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2cybmyksz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2exfkthkk.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwnmlyc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2gozuzagm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2eekphekg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2xetpcdsc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2lqryupmy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2mmvjcoxg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2cuhlkmke.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avlesrgt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2pzabfcza.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2weiwfvuq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2pdgzredb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pcpmmexv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zajcqqla.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gahhfkxs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2ubraeyan.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2limjfiml.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2pmopxmlv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ztrzznhh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yzcermzh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rajjrqtl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2xmtlljnv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2zauubosz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2jeanlhxq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ovisypka.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2vqlkqzfd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bbwepszk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2eykdatfb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zlprofkb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tgpxzpht.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vtmtvcde.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ilakmuou.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2mfoharit.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rddabglw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2eoneivho.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rkyfdnqq.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2xkxcpwbx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ezimfjqw.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gfczcwob.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2yeeugete.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2oxoxhmkm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uksgpkox.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2dlbaxamx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wcdyjskx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ltxiaeqd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2kasdhlyw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vennmhkp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bjxgikuv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bghogayx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2auuebogt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ypzhnumu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ksipwhag.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2bnfvkbam.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ztqdbxfu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jrrnbgip.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2elbhrtxr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vccwvaol.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2knqkzbql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqmsgfq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2qtuvhztm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfesojv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bejwykmt.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dalxwbhk.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrxbtzqi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rrxekvmj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sryhnstg.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2udnooxcx.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zswxlwmu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bebwdcdu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kozwmtgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohdhjqna.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2suqximdu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htlvvqye.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mcdlvqkq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rbpjewyz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2nflbumxf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tlmnqlvg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rekdetdk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dhsjvltj.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2fhuycesm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2lzveitmg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2kpcivvro.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lmnhjqrs.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2neowemsm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cvmbaajc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yaakzpmj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2klpnlefq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dsmmwmxu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2awibyovg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2amzuncyg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2sfhakvhf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lelsxkuo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ntyhmeyv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fovqntfm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rpagzawa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vtttwlqg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wlsxzksw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uotpaggp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tzvvgzjv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lyostchz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gfdxtciu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ebbkxeyo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iudtbumj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vawacqwq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2jzxlfwoy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2alkipycm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qwaaahls.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mcbtnrin.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2oelpxioh.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2etuyyroy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2uxsnhslw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2mfkkrdeg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ewoyifqh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2bcfbwbns.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2hcbdstdp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2arkcchjo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2mxwufsfd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yjdonlil.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fuwxcytb.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gvaseykl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zysukgyc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kkbtajdm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cswhhlyc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mkfbpqly.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2njkfvilx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kgtywnwd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tkjzwyly.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rlpbstbb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cbfpvhhv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nzgzskho.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mbspxskc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2akmitqcx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2yrkftvmy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mhdxfxqf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zicgnghp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vpmedjis.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2qnwdqhan.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yrcxqcpz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wompdior.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vvrpzjjc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2drkubbde.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pgmqwssa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2elswregn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2sijmtlln.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xtxaasho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iwbkiomj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2xlygkgzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvbuajtr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeldcebu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bnywedio.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oyjquinb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2arnzvqme.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hnyqsxzu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2eeknaboi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2utueibhz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qyvsrunb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sovbffqf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zwwduvay.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ekpcrzld.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kcepzmlo.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vzddhgmy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zykofxzy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rwsynkgz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xllvmlkc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2bnupamod.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oajwmloy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tsvvpcfb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jdwprtte.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ukwrzxle.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwahfykm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jfgeashc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mvhnlfdz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fkdttztx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zfihqryp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2enremymo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hurfjbnv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nwgfkurx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zvuesaum.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ousmcyfv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fwbiitev.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2gynucgue.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2trhmyecf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ucgxftey.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wwcyphvv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nxcfwkkp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vgphiirf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mxxetlfi.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axnuzrso.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wktkprrj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2afrxhuyi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmeenwr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mukkeuil.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dkkszltg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cmzwhxbo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ksclpkpd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2nbctpsnz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ytfemmkv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2btjzmasa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pibzpnqi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2byfuhntr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xxksdgic.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2quepwuam.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ihkxrsjm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fbiaoiss.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2wtjsuwvp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bkxvkwbj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zltsbtwe.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ovpynjxc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pguyuahk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2arbdoikg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bgqlfueb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2jdbziqnm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vigfqnyq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bdlwzbip.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dbwjvimi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ckydcfpr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wfudvcik.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cultlgzg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2vjyyylga.html


<!-- 参考信息 -->