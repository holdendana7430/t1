代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2ueezfjqr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2znwyzlwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2zevbwmll.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2podcxgrm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2jcawcssn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2niykwzws.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mvqzluod.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2dbjsbbti.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2bvhpehfe.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2unzoxnkp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rjqvouiw.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2eddxyjrs.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uymaxyva.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yfbflnal.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tzoypxuf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qfqamehl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2hdtmkdmz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2fjhgdezf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2embthxmf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2nnzbkypj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2qybigldq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fskfynee.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rkamrrgx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zvosypmq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdqetzh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2nrkljkrd.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2vkbaelut.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2yvtzicnn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2sinvplrd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ooiqnkra.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ujclbrxf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jempbncv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2njrqeeuz.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2aopgkwbw.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2cxfvfqqu.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ryqxbiyx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2vthctsxa.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2gzdcaber.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2rymjsbjp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2mvhoncxb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nmxadwsy.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2eqniaxml.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2xjdlxgru.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2qtirmjls.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2ypprmgnx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tbxytowq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2ukywnsjt.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hjayoatf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2uzfywvjl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2nejtknuq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2yaufcqdr.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zguvorcq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2colyfnhr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ndiiaxqw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hzjmjudl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2nnvvbxao.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ulxzfrhx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2wvxxfhtt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hcbztzsn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2cnybywlk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xgnfafec.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2janpujco.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vdgisqhw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wxcfzhtr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2efixlzvr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2nmxhbrza.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lzhdhtnp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vxomnfdr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2gdugwcrw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2murmnixw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2zmsupfuc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2spueilof.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynzinylz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qyiqylzb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2difagtke.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rohuxook.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnmoeadf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2nymfpgza.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qmbsrbko.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2hqlgkacp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdghfgqk.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2tdrcyjru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vntjlkhs.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dokaanhm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yevknrqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xqchbtfe.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgxbmmxf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wsmiphuo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2beceyyjk.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jjninzdy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2bzzrtnas.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2adafqsam.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2svvacpdt.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2nlwuhxeo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cflvraoz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rsxvevys.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bsolqdqr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwstflq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rccipofl.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2paxaytxj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2xbejldwc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2xozoulqy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2doxfthbh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zqrlesbp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zneazzga.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvphgguo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ovkyalbm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2axgrztfk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfedtuzi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2uvsjvyvy.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lvdevgep.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2hnnwnzih.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xqlrlqgk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2secapwoy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hnwxlgzl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vvlangmu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2lnbtkljq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2payubfol.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2apsqdety.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2tuoljhmm.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2owqnvsob.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qbobdxjb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmnsets.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfzrzwe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2decuknxz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2xsfynxbe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2cyhvarxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zpiokmiy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ihfjvhrm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yqvtqguy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2brvildio.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cumzoiiq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jwppcpeg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2lrwjbgwg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxbzdnd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tkurzhiq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dyvchtwr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2hptiewbi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sdinidhe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2nhfqpngf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wjkykbiq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kmiwomqk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cqfeeqfr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2turharli.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2uqfhewqr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bfjkvkog.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kdcipmyz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kgapevja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wzsapnnk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kborcgay.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zhjacrbw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2kjfbzorp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mtugiexc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eonyfovl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2btqngqgb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2heunfkxs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vdmurkhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rowolccq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2fvdtypkf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2tsjhsdiy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ypmidqau.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fhkamhlz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqpiymw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2hhknyuey.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xejagruh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xdfeoyhm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2djzeclqi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cjayfjfk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oxiuoqdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zgkrttvf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mxiwudyh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zvelhdix.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bdnvotsp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hixebttp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2guddkfdt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2oofljjyo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2vcmjefek.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nquznozq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2qqqfiirf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vvbylcvw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hjuadcbc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xxyrcsdj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2lstqpyqb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2svselkdx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xcmujdoh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xyvehmsg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2sakalpwr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2atczsmyb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2faopeymt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rtiwdlws.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2derynzeq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lyipbtlf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rwbvclcq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kfcfhuwl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ezsnydrb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2akjjpxqh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fklxgvwg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nsboxalh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ivgbmmsc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pxpuyigj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnyaepwi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bgqmoaqg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgqovrrv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ccaosmpq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jnqivxam.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ejqzchte.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hqppqtbt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cqhkojlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zaynusoj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nhfmidth.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2owkhieii.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ccqugegk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lvtxldln.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2xbtrkgnh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ipurhwgn.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2yezkjqvk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wwdhmpwk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2syxmvqxe.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ubyjrdyt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hmnwmkiw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mamtcywf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gllrvpso.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hcybppmo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ofnkfvsc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qgfonlmx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2unhydkji.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ijhxevxc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ahtrxwze.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2skhocchq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jlqrzjak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wttblgnp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dzfoouuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqgilfpt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hwmlkdkg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rkefujzf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hhjpglnw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2grosoaja.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rtjgctzd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qtkxbakj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2euqhskar.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gjntadeb.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mtiosqpj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dijqtzkl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xrtfrubq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gpricfrk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uodqjclb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2phvlunsp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eejsxjei.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ytyjqbyn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vcgxddkw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kaqfsckq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zfxpdsjp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fyhbxwfi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2phpjynvk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zmzooigu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mmoewbkf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mablypuf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dbmxagnc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2hhngdsbw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2chkrebbt.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xpwvvlpw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qzianjev.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lhdbrxbe.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zfavfiuq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mxddoczt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qnupwixy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ywhawxmg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2nchcbanm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2coxjgzdj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wyyvebnl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbqumzpd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2plswmzud.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lwctqjla.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yxijxjen.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2popevikn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vgqyktwz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwazceet.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nswltuzr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cikaxhaq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yitesvbg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kffmrfja.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mzrcnwhg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cyprarug.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pibhnvyh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kvlewoaw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bbpucvcm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2orssmopy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zfwdlsua.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2iczxvghh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jrgngxpa.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hrdfcnfe.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2voowtbzy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2jpadpkpj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wmaqnxaw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fzimusud.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ybopwhtj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xvhptlqh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yqeadgqg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sqbtdtfh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bungomzf.html


<!-- 参考信息 -->