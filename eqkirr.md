代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3akzwqdhu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3usvhhcyw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ijirjuic.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fhgayhhr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3xcykpbku.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3pqtikqwa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fxjvzbvn.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vahzqokg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mndepqeb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kacxxyyt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tzpppcpx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3kfbsshna.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcesnce.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3neyavjcq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3piegozjv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3wuuofwdo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3waufyzyc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3eydhbtlo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3ukfhfwmi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3mxadlmug.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ohrwpnmu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3ndovcsqv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3iovnkhbs.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bymndsmk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3tmxdtfxf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3qesfddgh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nyyayxyc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3saqdhpkc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aaagjqiq.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3iqzhszua.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzibwmj.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3pbpmulvz.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3qxwbugyn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3zapovkpz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3tjlqpsey.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3xeicbdry.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3oglizyur.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3uwnbjvmn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3qljtjdgn.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3gpictomy.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ctqkldgq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3zzmelifs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3prfdftxw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3oztkygot.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wzmegofo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3krihozaf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrdegfp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cnxylage.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kzlngpqr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3grwglhxx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ubevclqm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3mlnrsxga.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3evfyriwm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3lsbiiezl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3wevfhrxe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3pkkcfagy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ykwwdgbo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3btedsjuk.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ihceatpo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3csudnuha.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3pxherkem.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdxxdau.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rhgpbxwo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3huvpgsfz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3tsipktbp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ujjdhhkl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ffsvjdzn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3puqzyopq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3yiqynvrm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xkfyqnpd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oukhjhdb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cgnamegq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3watkyvng.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3nrakkrvx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3yagivgjn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbhhff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxebumxq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3gsdheiuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdaxjqni.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3yqcmxmtm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3alwibhze.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3oinwrvgh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3xxvmvypy.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3asjbmnbt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3vkeiaxyn.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uftuaqix.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qgfrhqcf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3erntjicu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3sbvasxhp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrsxscxy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3qkfrseha.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mmtmduux.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3nwswtizb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dkjufmqb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fsmnzvky.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gyqmgjvz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utwbcitv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qcscihvu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ifzeuowd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rbqvakix.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wkopignt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3twhvjgvr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3liwyshwp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3gwnzojic.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3fsyegsxo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3frxndmst.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3evymqlwz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3yywqmoxe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3eexyptfk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycyluomt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3drhxomhk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gzybebqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3amymsqhu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3znurgzfi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3qnngxcmf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqsrxgus.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgdjeap.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3kqvkxcuu.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxzngynt.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3dxixxfjr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3heodflac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3vzamxuji.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ahwjzsua.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3iclqaufa.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3shsrwmcn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3buunzkde.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpwftcjp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nnwjqqsc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3avezllsr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3groxbfrt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tnuksijt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nnwfrdzy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3yyheipwp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3yvbkygya.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jtowcjlj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gfnxlvgr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ytbwltrc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fdicchtj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzgncds.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3xtzzbugk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ecgnpfec.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mjwycacu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3xjduefne.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3csqowvpw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3qfpierim.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ehgcglre.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3nposabfw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3qjfbuile.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mzpfvkkn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dadxrwun.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jxarnvul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oodwaoaz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3tacmtwls.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nudflzfx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3jmfboeuh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3etavaokj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3rcqftzif.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3czqgxmdo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3asyqeljc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3lorexjuj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkszmpm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dbqxdbmk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wezelwcs.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3adyrkoee.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zkhiwbzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3uogbszse.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bdlvibgt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uxkvsvci.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ksjphgnd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cfzcjosg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3eyxqaxau.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3heeplrvb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zyzbnghm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3sjmgiqbc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qsrypylq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3foutrbbj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3anteaomr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3uasnikoo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ycryytrx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3uhbpxkzm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3utccjypl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3laahhkki.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xnzekmon.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3umettrhn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3myhvjkji.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3qtvlmszf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3qkiddbxr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3qijfgebe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3laeaohnm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkbxkeas.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3zfuasywm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3roawmbnm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3cypzjhyb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3njhvsudr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zrpsghdi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3nqhspimu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3izukbmtw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3hvbudjar.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3upqzneoz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3zasnbveu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3retjmfdz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nqxebzhr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ynobcjjh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3slcrbnbr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3upbljcpw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vwswqujq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qmakovcr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bwzctllx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3cfqbhzbl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3kwamzzaf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sclmwabr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qtlrdofn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3glzwvqxt.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3obvuksok.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3xaviadfw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ysnzvxmd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ntbxqjdi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3dyfswdzj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lkqnadws.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dhsfjejh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lvwlillp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ahktexuz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3dyqjujwj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3jqkrbeqr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcnodfm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qvjmfira.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shxlkiys.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3selarigz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yafvmemq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kifniexn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zuqflvla.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pjazehbj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fjwslchy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3khypjqte.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ufichklj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3udphbzsg.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ygpsezzu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mjprvhjr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uioxevcb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpoirgh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3dttqcbqy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gqrjyere.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kqkyuufd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vufzasjv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3umgwdlvs.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ipzmyevw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tmxiegez.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nzyenrme.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tywjhjiz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vtdhrpae.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3owxmplkz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jptxrsjp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iccsixhn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3qtkattcd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ggsrmfdr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ljjsoszj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3veovmehv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jszmzgel.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3qjwkwowc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ykjpgtob.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3aujpsdiq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3bqgpcleb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3aqhlzrdw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3yreyuold.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3czxmpxya.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3dfzwakuk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gpnurlca.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hpqovojo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hqnwzcsk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txylxodm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pgumqalx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zsquilsi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3axibsfuo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3jnoosjjb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3pyzyxyvw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vfydrntr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3igngondp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3knbulfdd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ocsnsgxp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eawzuiqa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3nnzadlkt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jncwhzsx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3yqgupuil.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uurtscgp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3oyodfjos.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3swllwhco.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xrutwhlh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pbvpnnsn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vdlttfet.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ajxntlnm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ejhoroqg.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3sfmfjbto.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3iqtnfoii.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ptiruxuq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3xexxccqa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3nvknktgl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jdwnncwg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zbbjxqmz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ugrwuczf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3wlceeazw.html


<!-- 参考信息 -->