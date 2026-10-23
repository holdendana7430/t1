代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xhxypehc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3vhirgocn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3awgqflck.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3ewnqedxs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ukvcbval.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3eayninsd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hxersgir.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3lovoydbs.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ocbengex.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3yzmfjkta.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3bevjsgdc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3yvzbomjh.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ozsnfdjy.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kbamlpwc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nktmmnqb.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3cysdclgb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3kdsafoek.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3gaeaapfd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3okpzllvy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3puhxyviv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lawqaaur.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ptuvurim.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3vlsqibho.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ibyfghnq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3ibrywufq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3osvpbttc.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3skrmlbiw.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3nckgdshq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3iyvfqxfh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3jbflreis.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3rmyxgrvf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3jnnhtarp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3hhccvgcr.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3unsjbspn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3dxukakyu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3aajbblnx.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3rageiadk.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3yqlmfyoy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3qdvbmpwg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3xftlhzaq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wmrrwoak.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3scfhzugt.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3vnsxunen.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3pqtakavo.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3qovpdymk.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3xubsmnyg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ufppscyo.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3brxxttfw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uqtnbznd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnoulqfl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjpxmgx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3nyrspxpt.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3kpwiwqjq.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3lbadyasj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3rvlspczr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3zslfcuaj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3amgywmaj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3zejzdltq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ajruzilw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lhojpmqq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3hyhxekls.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3czqzebgg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3poqjvhev.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cbwlqtqa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3bxrryvgm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3dbxbuyhq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vimmkgba.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3pxkkgpgq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3usngtohv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3szactuvj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3oryjlrps.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3orqardzr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtzkskor.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3mrgcngxw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3xedhjmnf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3keapxero.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kcjwzlxk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3aqrusdoh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hezacvme.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3kpxhnamm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iohtmvqu.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ufcwwclq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozazmgsq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3reqgwhew.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hbowcurt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3pjmelnok.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcjkkxx.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gpoqwict.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3stxltjrd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3syigowzk.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3wmqiveuj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmrnzftc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3imksjggd.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3scyrgmyz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3lvedpizr.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmbjgtai.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgohtrhm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pacptzcy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hkpcpglc.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xaucdaqp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ekwszlll.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ecmysfyp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3eyorqtvi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3cfoedpag.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oswprwhj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tecqurnr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3nqmmycas.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3qfbtxpbq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3meoladqj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zdonvstf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3dewhpfiw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3yaewbipl.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3tkujizrq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3xilocjrk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3expjxxzm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pspbtjdb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sjelhyzf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3yvyfqcym.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3pyatuypo.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3olkerxox.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3izjermbc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3bxmxhtnt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3jbdibvkp.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uegudbwh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3pdrglfzy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3owepxxmf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qzembpsr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3xelpjgdq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ofcdjlyc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3zlkuiukv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wjttiatj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cyxmtuma.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mrmthejg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3oaryybxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sujdtcgp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlrjudm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3udnfdabp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3wrhnhsgc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vyjxiunt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3yzbqbsrk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fgkchtjw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3msercwtp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ittnonvh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fruoewja.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yqheqxpn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3axjnughc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vtzueiqo.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3uifstdbv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3aohrxfui.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rntcwpog.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ugcnndfv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3uccokfpt.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xosahtqr.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3tjhtefxi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lfeyztwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktxtmszy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3psmuwdlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlqirnpy.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3mivohurr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3naxegyyb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kgebrryj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3hmjsbefx.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nedwolkq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3mugwgjri.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tamjlule.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3htiwnnbw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3esnwyfli.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fxczvwdq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3acyhnune.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3gpdbpjja.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nllfrkhp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3vccoceyu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ajbyfaci.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3nhzeskif.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xqkiygpq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xqyzssnc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zvmlbrhp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3psytwyop.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pmpoofvm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vxurpxfs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jooaecyi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3fvendbzs.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qunjwtey.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rmwpidvp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3odnlbhtg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3vukzpbrc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3aoywvenr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3tdghqfwy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jdbatlpr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ykfohwbw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fyixnoml.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3xlwduhsh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xdsbvaxx.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pvwottqj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3hjjzjmcc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gdxuybtq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ofvsuote.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3txlvifpe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3erjcszpv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3uielcrmp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwoyeuye.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xgiupwga.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ayllccnr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ynuscqqb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3bggsimna.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3exziysyh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kxtuibko.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wheanvxj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3snjmfjpp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3qvzukega.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ggxhnvgi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vzwiayas.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3amnoymvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ulnxmwpu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sdrwevwo.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3uiuykrdc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3voknlqba.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3eusdpfrq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3eddplrtz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nrhybqxq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uwphgoei.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rbjelhoz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xzvvoizo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lmokokcz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fjzprspg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cjjpacpv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aswvvcne.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aqqdtayx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqoewcf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lrvahpbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilbsedfi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3fwkgtsvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lictmjjl.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vskghnoq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ngvofvju.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3onlzvinr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpucpxou.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3hazaxjbw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hcnvitch.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ezurilwn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nhfwqedn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bcrogmtl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3deauykkm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3krppyuex.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ksaiasmq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3alqlafse.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ixfvcura.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lklgrgit.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qcplypmz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sbuwpixa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jfpnpcpz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3izwgzdmk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lvriiinl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3qtiowiop.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3okseqney.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kkwalmjp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3acqoqptm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3rxuthoqd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qqoemtoa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fvmevqft.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ocbksmkb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ryuynpaa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3eddlkphw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3alzkqngp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eykiutvr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3qdbojvbz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3byyitwki.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vwgvzycj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3grtxwjla.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ohofsjtd.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3shrtfvgx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zjfhydgl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdkxzbtm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gjemrdjo.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enlfbbve.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3chhzjhzf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3pxhiguzo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xjhbsenh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3cowalyhp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qqhvosjv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fpiamzoe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hnbavpgw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3xjjawgyo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3txhlexsb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dpcygejy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3odzmwfon.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pzjrvewl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xhhhwbho.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xxhqhwuf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3fzbpgsrr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sagaekuj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sajatbfm.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3acuoxket.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3idfljlyj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zlaatche.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3sxuzobyh.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3odlngnzh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ngptlbni.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pxrcuaef.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zcaapvrf.html


<!-- 参考信息 -->