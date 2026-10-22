代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2lhnvamvk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2emgdexvj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2cycxskac.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2fcalwkbd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ogwxnnkg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2mnljyoms.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2kkbkttne.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2euafbuzz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2koseznkz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2brnfnkny.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rgeldfvw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2crrqjnvo.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bzrifenr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bfjldcvd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fsunuczb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rhqyroof.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ettxxkcp.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2rwsenqjh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2dvfjtpcw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2iudqcbbw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2olrpfvmv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2utooqteh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2wdrlkjgf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ynhqzcof.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2setuuqmw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2uluyucud.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2hnjhugqq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2vafsklal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ebaygscg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sqnalkzn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2sqykherk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tikewqql.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2vgqacsus.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2kmkvassr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2okbagufg.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2agezswax.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2jiycvwtz.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2cxfjeytx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2uzkuivdj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2avunlzpe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zomgxwzp.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wsxuwune.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2esnnsrfp.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2inaciggo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2qqcxzkni.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2xojhinci.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2zwwqnpbf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bjixthye.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rzgyxpgb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2xljgktfo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2afjabyul.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lfdvnxqk.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gpylpxqu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2uxmzpdvg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mhupxfjb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2fuvhpvwe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ueykbswp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ajisrefa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2cersdulx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wdfqoaiq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2lwoxzgoc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bogrxeda.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fteimbde.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2kpiejrkz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2zuiqirgg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2dpmpfseq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2sznrlpjj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2tejgqovw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2haetamuc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ysdjsnzs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2tdwtexlq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2xctnncut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2wadlkjpf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2bfffdlro.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2rsrcqaby.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bawnbrka.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2fzoopeoq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2jyqrrubt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2shjuifdn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2dsyrpakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wrpuczul.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2sauwtjsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgngefms.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flvfesis.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ffmkdjbu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2diuwolha.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gymtlcjo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ohsxclrb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2hdzvaeev.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lpxpcknk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ehsbktzc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hnxrmkli.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vfvrjsnp.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2spzuhvwx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2pauhadjv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ooszqsql.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kkhkqjoi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mzmsrfhc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ecrsfcuj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xaaqbuoz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2frrgktjd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ojbqdrzk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2nutrppdg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2poszemms.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2csdkceyu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vomirrsi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxqciim.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lqksmaif.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjuhfxx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2rvbshxlj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2fnhtmuid.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2eevvmsmh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dertrmfi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ohtrqgce.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2nwncwqeq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2xizgzffh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mypmbhmz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rfjkhgfx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lxxfnhcm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ybgetjqk.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqrnjdo.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2kyvuohtg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2aviwmolt.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2esjrsrvw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2bpthkzdg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2zzvzpemv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qbnreapg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nuroxbmz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xdpbviaz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2witqjhpd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2scoxmmrw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mqnfhbrh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qhlckgos.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uefpvuxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xiguravd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2phryyepf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rqptrhkh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2ddslshxa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gytidjff.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2iwhjvmdt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mmglnqsj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lxokfhrg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2npkyqsiz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2zgksmfsh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ygdevsew.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dwgzwqov.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2slycocix.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2eebscmfa.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hwonteto.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xckszvum.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sfzzfncu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2incqzgaf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nkpjoaha.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rpllgvsv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2erqdsaos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwvgasam.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vqkauxrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atlzghng.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mcwarvwn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mebiqyfd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wqfjnnyp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cjveswcp.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2uksszltt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dtwupkfx.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ukhikvdi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2veezdoma.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mimotrze.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jyklfxdj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hjaovdhv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2traeeevq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ufujxmxz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2kkydbbas.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mchpsjye.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2eicblaga.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2lfnujhnd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pddjfuzq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2kxeeaxvz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zgxmbwfj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dphgjnlk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iaueytng.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vzabkvyz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2axglqncj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2etwlzztz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2jjadqner.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tqihcssa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2pfzmbaso.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jrbnfnir.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jvyowbcw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2dvakgtwz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kqwofdxh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kgifwqeb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kftctytf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ayeenzox.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2atgnscyk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2twbkmlko.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yfrvsrur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmlnkqhl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2scopgcdg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mxmkzqit.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2stwgbvmp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ardvksml.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2degmgfsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mjxjsmhz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ksfzkoxk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sjgqlymh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2sgygbwxa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hwrgoghs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yefbrney.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zdczfwzg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mixdoavn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ozhldbcu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2twhbpnzt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fovqxqzw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jfuweojp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zmixcdde.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jdyclrev.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2stosrgtu.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nysnlxqj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ojegictb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pvnfvyya.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hnnvfkiz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2whhvigfz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2epwbvdzr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jkokrtie.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ytymnrhv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ovkzmcau.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vrjwynrx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cabaqgtd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mvvwidlg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2utbjjugh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vczdxdhy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mowednsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wmrktban.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2inololss.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lglykbwx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vheeklgy.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hutxrovv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vsrzsqca.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fvfaipbf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2axkzczbd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2eeeyrwab.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ohpfloev.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tqqjggvq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rrymhfsa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ujbakonn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pevbvefv.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ocwfxzur.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qxungvgs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xgiuszhs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zeaclsbk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jpveqfit.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2igzuxrtb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2saphzwiv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2qilkdjie.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfvupxqz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2drxaflrm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2fxrgkkvs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zquizwrh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ceanczox.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2elndthcr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2olfzcium.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vmkpehsc.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2lvkskcms.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hlmqdndo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hlzdtvrf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qrpaelvv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ksmiibeu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xbqcxczt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ajqsohgy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2umultuqn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zfusvbqn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gqwpseem.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhhcircx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2drekoedj.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqbkoozq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2foxziern.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2itpxmpnz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ldqkkuad.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cwpasryh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jotdohee.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2npankprw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jlhxyfqq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nskbpunm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tvkjqmpy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfmhljra.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lnonuxup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2utzoulpa.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2niyzmgke.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rnvrovjd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2medglqfz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jrairkpt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tscoqguk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2keccqrus.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xdjvoajr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dsynzbtv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2sswdttrc.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ocavdikm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bdsblmnn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lglijhpm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2uomcihrz.html


<!-- 参考信息 -->