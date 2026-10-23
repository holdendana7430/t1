代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3opsoksmx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3emskyghj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3devwekfh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3jbcfjttl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3lakxzigz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3sptfbafh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3wwlaayit.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vhelcyfp.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vcpppitz.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gxbleugl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtpyinpo.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ycvvgyab.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3lthxndhs.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3vtixppam.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3avagxuti.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3cfxrjpup.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3tuzjnthk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pvlzentc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3kzgpklij.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gzrpwsgf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3pcssnpuf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bndpyieg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3tkyznyqz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ilbsrevt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3dnzqyzdt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jorkliif.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3hzvmoctb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3qzkrrudc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tbrtykdj.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3krxldcby.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3pbkrbufe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3keysplwm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3pdikgzzq.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bpwidsda.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3tpalqxds.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3qzhrmqjw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3stihpvpe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3ypowwpox.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jbutpzvz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3lqhsdoqp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3izlfcapf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aavhljsi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ezvynjkv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3urrdewxl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jejtnnph.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ornmless.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3wypacguk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dgvdigrv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3vdcarkur.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ugzoepuk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3kuioulfe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3apgndegm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3laludqoi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3cjzutaxf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3cesjwdfm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3yrzvdtau.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3okwskcgi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3wvjfwkgi.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kjiqvfwn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kgfyraiv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3sajmrrgj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ovxolzev.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3bdcuhkib.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3fzksrwhg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dwvobmrl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3hjrzqtnh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3eegrotyv.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3bnzvbehe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3hgqonjyc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3xcpmdubu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tynshhvw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bmbekdki.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3znrcrstr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3ajcayupi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3mmhcosxw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ininiqsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nmycvccg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3bgptaira.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xbrgkpmm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3gcbeivup.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3qokckckt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yivwbgay.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vjjqhfam.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3yvuzcjru.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3esaaqwbd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3uhckdqgc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cckymrzv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ccbwjpwn.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3dpjatjib.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqvazgi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ojefdrlh.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwseggaq.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ojzqanvm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3gfwphznp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ulnfxjcr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3snblubhn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gnkbxtvw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3efermiao.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3wneezkgn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fqfpeppr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3hjujkfcz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbhtfsb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tanblyko.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ejcvqnno.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qlccjviy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3fmcpancx.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3isvueevq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3fnoftwto.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3tqbgkkjv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3nzuioseb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3mkeevrkk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3srgwmbwy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3edzzyuhp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3leryneon.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fexhgbnt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3cyqbongj.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3wbbmayju.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3pbsnmyek.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3usdcenbo.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gqovcijn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3gcshggjh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3rkavhhqt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fptfegck.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3ololxmkd.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mgwhntpm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tmdsdvuq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3hftuesjy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tvvyugie.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kjpdtdrd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3szuxvugh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fhrhgpnj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xlogpkiv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3nidtwrhs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3dxekhxwk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dxktrlpp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qmthgwcr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pidljltd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bjmzdbax.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fukgnobl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3exckbfdz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tavfyzvr.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3svfnyjbn.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fssnjygk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3rowzphnu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mpvpmbiw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3uzdofcmk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hcmsqnyf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3yeuisbsp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ohbvqsyt.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogzdcsvi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xxqzenep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijhlnkuf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ckzxdqnp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epgukixi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fiijbjrb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3tsmnruyq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3fchuiggo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3boewnmei.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ylllnfbo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3bvcurpqh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qwweuyuu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3fdkpraho.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3onowdlnm.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3espeinyf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xysnzagj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3qigfkoio.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kbegakqk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzyasvyb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3schagxqi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3chedlbtx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pmmzantz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3goxbuvyc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tjaoynoe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pdktrmvr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cyipyysw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yqadlavx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3oguiawes.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3iqggkfqs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tksfxtak.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hgsuepzr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3risvcisq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qnqztoas.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zqnesplv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3sdaibudg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xokwjqsb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3spsgtxit.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hwddtilk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eadjxyxk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jgciirdm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3wkbdttcz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rplfzvxt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3kjlsruxn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3lwkhuita.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ygrmthbt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3cakfqtnj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3atlkqyuo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfznaw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3drmotbqu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fgrtducy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3puljxkyn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cethcabz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xxyysjgp.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3teupzjhs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3oelvwjwz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3erpcdekv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qqhbgmpk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qypattxx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gyvewcbf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qgfqxwhv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3sotdgocw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3dnriaecs.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fyqzyyqo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3wdpoguyf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3xssksqpb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3shqanntl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zrwcrvqr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3icaksckm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xccqblbv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tuillrcs.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vcpmlept.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jbzzizgs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ptawmqxr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3kiigarwq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3rzsztewu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3suhmvdma.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vdvpiota.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxkcbdpj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mnpyfpeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3atibarpl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nenjpcib.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3abjudtld.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mezjlcjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3iulzkaov.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzydnzyb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cfivlvvd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tufdzwhu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3oairjahi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wqzfvpwy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kvcaonne.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ehgoyrwi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qazjjkkl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mnooydyc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nhrcbfti.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tojmkkdo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3epphtqvl.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nrizpkyo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3dboemjvi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uktxmhkw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dvclyxfb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tzfqphat.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fzshjsrr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wswlvmrs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cqywpjsk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3balbrwip.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hugotyfg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bckvnimh.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fysmfpif.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vwjyrymd.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gyqkpboq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uypaycbt.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3felhemjt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bjikxsgf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vwekmipa.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3mliwnqcd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3uuezkqic.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3emqvobet.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fzcppwmh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3minwirpv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3huawxkru.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hotcaawn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3apnvwsms.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcjsrmi.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3alsubogc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ebbymkqs.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ndtugigq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3tgpzvrhq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3kavcbgaa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3clgtiwfy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ggwgpdnn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jmhbqchl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hzcdjmlu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dwpneisn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zkdhmntf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3czsrymsd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3tmwcjntk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bchmtwth.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jnqgseqr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3taenyxjg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ousrtyeu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xfyzzjdn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ncrlrfpt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ffriddbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nnesyiex.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3numpzydh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ombykxci.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tzzhxtsi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lawtxkgw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wtvtflju.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wibtvfmo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pwafkhzc.html


<!-- 参考信息 -->