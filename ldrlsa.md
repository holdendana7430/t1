代发 wailian999

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3viirevjg.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3lovnkjzz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3xrspvoqg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3euadypsz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3sielfasm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3onosxuyh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3tpyflumj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3bmhamcvi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3axrviben.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3xnnxgxks.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3uqheyiqr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3fzfsrtps.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3ldtncdtr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3vgmjgzuq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3xayhlfyz.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3gqsovvzg.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rduawipw.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rsouydhq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ypfhaqbg.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3cfxcuvoj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3vatzzpyx.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3jmswnofs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3vwptouaa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3wjkydmwo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3scszsvxs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uospdnjd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3lanffivi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3ytntxqvo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zojzulyu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3hgukhiaz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3vwqusncn.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3wefchiyb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3jbecmmoq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3enmkkwvu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3eztjrquf.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3iqqlyziw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3tzzmqgic.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbuahi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3kqcmicjo.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3eismetkr.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jjvkpmtj.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3wsrqluzb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3lflpfjho.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ltpulyjw.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3tcpcpmix.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3kmlhjzrc.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3ympmyzrr.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3kodwmmnl.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3qxmupcvp.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ctcsbwou.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3dfmawjay.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3zeqduxik.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3cnsoydut.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3lldjsqsg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xblobwef.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3uqarubzw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3spadhpbh.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kvshvhcx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vobtgbfi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uozdmizg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3zgjvntlf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cdflhqtz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3qdqhpnfe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3lxcltewe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3uaxodeha.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3nhfpbhcy.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3kmuzxfrb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpqangs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hhkhcvut.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rlvkhovo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lhlcrqrk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3opdwpasq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gplzgpqc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3zublivlw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ltpvxiyh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zavkvxqn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjxcbid.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3fzqdinut.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3feahxbcs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tjlqypro.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ohfaryih.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3hanlxili.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3njvvzicx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fdisdeqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyucjlje.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3eijrifhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3phwpzfnh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sfjlbnqr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3rwosfhao.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3rdljjppw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3miwjgxhr.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dedirnus.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3wuncrctc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rmdlnnbc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3kvetdsje.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3mmghrhzq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3nuzkvuop.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akctomva.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3imevnjel.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uarwvkav.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfvptwje.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvfnogo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3lcycrljx.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vbwmksqz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3xiloyvmw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3plghqvll.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3stcrvqov.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3yajulsxe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhjkudkt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wiolluhz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3phwdqovm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3dywtgujd.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3bebuvvwg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nmfzsmwz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3drcnyuvb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pxayfkdm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lspjyfld.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewymzfao.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfllbaax.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3eisxjbnv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3iyosfgbp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxtuzrhf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3eafeybpl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3qtgkfwvb.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ecdrkzvb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3sqpardga.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qtytyltf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3uogjevmk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cddtxrwe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3eivmduim.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3vjrgpewg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3gfsfldxf.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3soslampd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3mtcbvsdv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfthiryc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3gmsmvjlq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pwstgdil.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3vrnnkiet.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zdxowvgk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ntomhwnz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3cqviyqvp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mlbcsoby.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3crykjosz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3ypqfdrzg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmaoyvi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vcxeoflc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cheztsvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3litsdzzf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sxxahnyy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mfkfxmea.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xgxwkxao.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qdyqqbxu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvwgxkkh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lheytvzh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vrqzcfso.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3istlgrqm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3txvcgoyd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zthafpgc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kexjycex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ruuavlbl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3kjpmbefb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlmhtfbd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rkmiglyk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3lfstlzoa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3zylowcnl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3grhahozz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nrxflrfw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vsrbsshh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bcaybwxr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3sititafo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rfczxyjt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dwxazruf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3thdueffm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3qcgmrbvn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3bboytruy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3atgpmosg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kirrhnas.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3qgptgqhi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hlkixfup.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3aqragmxp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ldvnchzp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3lxpfgljf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rqwlogxk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wtlzycil.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3gzddtgmv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3zvywpyhh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wqdoaxah.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ymevswsm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3cvnabhiv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3idhnnmvq.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pjshdtqy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ulxstaem.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3cwycwczt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jzxvwgnf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ckqzlrjb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3vlycltpx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzqliea.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3boygnukg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gxrnjfqp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ezzazjqx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3icgnifoi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vehhyajz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pxtmupwu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3flmikwpp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3srzrgswk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3buqxuqfs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3viuizxmr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ksoulzoa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zvlxqwkg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kszmthvk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jwlegnii.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3upnfuuty.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dsytwrql.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3syxgbelq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hjiyprgq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zfvlkpfl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3awqwpfjc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3nfrmleip.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ltputeox.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jynhyvmo.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wbohfags.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yxjolzgo.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3oexgkihs.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3gvtztkpv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fetadcjd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3hkuhthrd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jczwzicr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lesyllkf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nmubmlhc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ocvgsczc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3unkiyvzp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3okbjtlgy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ddkqmlnc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xbaffwvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywifkkgo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3qrvebfxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkgsijek.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3byjfqpio.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3enwpjktl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wpqpblho.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3odrtjlit.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tstrfvgo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yjgiyfqw.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3csrytftv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3egmnfrgw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3lzjztxjq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bjljmqje.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kaldwyji.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wkvzcdbu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lnqtdxtg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xlpiizzy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vpwubydh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qfmeofhp.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wdjsmbku.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ncpwdsze.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mdcmfyav.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ctavqlfy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ylxcdtit.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3vzcrnsjg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3anxpnekt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ccrqcwgv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3duxjocle.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vifhhhhu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3uzynebhq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ipkarltb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3epqyyoxs.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wqlyxzbn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oozycwtn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wsvqjzlr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xdgxkmzm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3beyqvozo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mjffjwon.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3cosyznwe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3cxjtaxeo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uhoesdez.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3qjhtkpjd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3azolvqxy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xjgqnkhi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gfovpapy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vrqrgmhy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ekejqbfk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rrrqynlq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jhfbzvty.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3aitwnyse.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3esonypqj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eadskpxn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dmbufewf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hppgxlvg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qgvyxtzp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3srauxgrf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bonhcghn.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uganezku.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3xxxwvwpa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xckxylej.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wnmvxgve.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3utjfgdyx.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hcnrcezk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ibvbmjhy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3elggfabb.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yycfmxoy.html


<!-- 参考信息 -->