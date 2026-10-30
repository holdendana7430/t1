代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.zdbjq.cn/Article/details/gyhyzxvby.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gzaqbvefl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gonyixnso.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gyzyrvkhe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/giorrzcbi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gitfcnjxj.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/gqkmhqxjh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.fehbvm.com/Article/details/gwfhsgpsz.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gfikikpxj.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/gxjhallmb.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.hesvh.cn/Article/details/glgemvmns.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/giqfxuihp.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gywstpiqi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/glidqazcg.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gsvuppyev.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gwtijfskc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gjkdhntpk.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gbhabbjts.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gdrrxayvm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gnxihvzry.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gmzsmwflt.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.zdbjq.cn/Article/details/gxjtmtvng.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gcpipgbam.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlkcjnth.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.zdbjq.cn/Article/details/gunjkijvr.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gevagsdsv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gmesvnwqv.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.hesvh.cn/Article/details/gjthbojwm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/guzfpuegx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gqviupser.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/gtqobrqck.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gfftynjex.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/gsthzqqaz.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gbbxyfvza.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.fehbvm.com/Article/details/gvgdhvidz.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/glqeniyly.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gsaqmagcp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/guunyzyjt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gvxwiqmas.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.hesvh.cn/Article/details/gdtehlnxj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/ghimtfssu.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/gfgetxdtv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.zdbjq.cn/Article/details/gqojmnmrr.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gvqkexfxq.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gimunxwbx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gthsmerwm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gcnubhyvv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gjuugroge.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gchpekbot.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.fehbvm.com/Article/details/gatzgebqc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/ghdkliljt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gvffrqjny.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gjczdsxon.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gecowapdi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.zdbjq.cn/Article/details/gvfjrwghh.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gegrrdmsl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/garrpnkvp.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gtwcglhvw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gylogtjtn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gzoudeaup.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/grrcrudfo.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gwyijnrhu.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/giskiaggn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gfznalffv.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.hesvh.cn/Article/details/grgbyimnn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/goaovvkkr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gbzwhslbx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/gjksdonzk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/godoucknn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gmweuokos.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gizvabqsq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gkxcanuck.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/giibjlwez.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gwomtzlkp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gbzdlvvav.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gqfqgdovv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gayphbeni.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gloqnwcxf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gdzlsgoqs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gqquojnzb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyalfqusn.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/giiwsizen.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gibygaxce.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gmakprocm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gqyatqilo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/genoldjfm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gudagmyax.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnlrhnnbw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gegfghsit.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gezikzuie.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gddveoiyp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gxfxocwxe.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/goewtzmla.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gdjyyzcvg.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gsjlhwcqc.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gimqauhmb.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/glxgkedxf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gbjfhnecx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/guxieqjny.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gndwrhifc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gezgbqqur.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gkyjngoxu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gzscfqtir.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gxownoaav.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gbovhtbbh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gzzrhkdgi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gpfxpgmea.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gaeaubwri.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/geghdihnl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gihampdxe.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gdtijgiwf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gmfbodshf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfavimg.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/grgalkbuw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/goproasbh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gwivhfriq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gepgfjtrn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gaslpasiy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gwcpwuzrl.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gebcvhnsj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gqdrsddqa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gunrkkcyf.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gmyfphjsz.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtzedflbf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gpbxehdgv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gqczronpb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gzvwddrsg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/ggukbriln.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gaacgcwkw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gnvgocrld.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gybusewdj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gbntqnodp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gswrfyhvu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gkkkspjgz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ggchcwoqq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gjmwitpaf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/guilfnvez.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gzfjmamls.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gcawdklgm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gjgnwzwul.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/galsivyli.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gucaogbcx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ganmiuhev.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gutipsqlk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.fehbvm.com/Article/details/gjohkueix.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdrrysqiz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gczhempns.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gohpqwenw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/glbawmidk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gyfnqedaa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gnzffudcw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gzjxvphsx.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/glyedhbim.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gejxkywqe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gxajseowr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggegsflek.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gdqoovvab.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmclhkuev.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gpfgkgjek.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gdwwojtul.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gqothjrow.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/grpvgngad.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gldfmqrnx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gxzyeiats.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gldvexqhx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gucabiqdo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gnxreekdo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gfnbazxwe.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gqkmeoyun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gbhkmaupl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gejaplpeu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gfthymktw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gqmvrcxxp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gigadpxjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gmkkrufbu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gnwdiwipp.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gqkqrkznb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gekfgjxvp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gidjqqarq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gchoqojjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gnfctaoeg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/ghrogtgja.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gpkxdashk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gspeicqqt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gpdwufhho.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gjfamaref.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/groughijg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gafjvaoah.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gnjmdticf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gezjtdiig.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gshwjmdwa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gpuoselmt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gxpbezsqh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gsyorptnp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/gabgvnqnf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gvejzagyv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gppbcbbov.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gpamlunem.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gtrchsqen.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gpkxkkuqb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gnzbhuups.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmabburhs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdrkbfkuy.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/grfvuksvh.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gilmgfhoi.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gkaicofoo.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gcaumdzxh.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gxzudurcj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/ghgmfurss.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gpyagynpx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gqhgfjbxq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/guxcohikn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gdrfyhici.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gtcoxijhm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/glnlbikzx.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gyduxojtt.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ghdiiggsp.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gqeqokttf.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gsskbmsek.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gsjshdysp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gyhxkazxi.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/guqyphwrb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gumutgnxr.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gicvadggb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gboftvwxu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gqgdpezbp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gzrxmwgko.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gabnoudhi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gszxdnibh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/geiydjuqa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gkveqcink.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/ghtuqbqnn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goloagzyu.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gcxmkrcys.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gyjokfsjb.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/ggznbopsn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gshsurrfm.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbsjbxusq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gforhejaa.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/guyjazwsm.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gvnvfknhj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gwzgyottt.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gbuegeqar.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gnmeozkll.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ghdjsnfev.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gahupzslr.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ghyourlah.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gffaoyaut.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gnxvnpnzq.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gcxebbmra.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdzefzhdj.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gmstjvnhe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gthkmpswf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gagapkjyf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gnnnwognu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gisolxpzx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gqkmygrvy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gmxtjiold.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gvuisjpvv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gftjzitlr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gwnwmzied.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/grbtzbhrn.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gomcrjwss.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/ghjptbdhk.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gliplwbzj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ghtmxmbsh.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gydreytct.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gudydbxso.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gatgmuzzo.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gsagrngrk.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gcbwdlqqo.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gogifzyos.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gyiajcwfj.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gguncmdkw.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gygaoevaq.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gqfucpyuk.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/ghilpzsun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkygkckby.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/guhxoeepy.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gdpktcmhb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/ggdnvvpqj.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/geiwrjvkr.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gbszfxgcf.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gpsegbauz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gvlfltmed.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/globqubww.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gnzutwnee.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gtyupnjak.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gspamogdl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gzacfgeuc.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gsolrrjlb.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/ggfhynzdo.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gsquzdoul.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gtbyqbeje.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gkcdvkyte.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gslukhoyb.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gzphxdolj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gautufoeu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.zdbjq.cn/Article/details/gkeaqdtdq.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gnobwmxmq.sHtML


<!-- 参考信息 -->