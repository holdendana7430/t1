代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/ggysspsal.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/glcccubir.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gecldbayr.sHtML

TS:   d.toISOString()
来源：http://read.share.hesvh.cn/Article/details/gcbxyrxwq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gbyyyzacq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.zdbjq.cn/Article/details/gdducqhrk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/ggbyoliqs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.hesvh.cn/Article/details/gqmmschax.sHtML

[J03] 字符串解析为日期
来源：http://read.share.fehbvm.com/Article/details/gdpotncof.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gfiktcxin.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gdmhbcbds.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/glnnrndfk.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gjywzaoru.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gaarefwhk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gsfoqouue.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/ggzeumrds.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gwgiyyyey.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/gaykbswrn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/golmrdyjb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gzsgqqzia.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/ganuyjycl.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gcylobuln.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gczrwvylg.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.fehbvm.com/Article/details/gosweqjlm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gqdagoqpo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gaksuioxs.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gqtzgxhdz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gmormxllj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/guycbojtc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gnnzwpkvf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gjomlqpyo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/ggkxysabb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.hesvh.cn/Article/details/giaropplp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gcaqewues.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gtpfxodqm.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gvvepzzbz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gscljdkqu.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.zdbjq.cn/Article/details/gfjmgmvyt.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/ggtnlwyjz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gbogtzofp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.zdbjq.cn/Article/details/gcfpjklfc.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gxiahmokg.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/gghtxawbo.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/geewoxkmt.sHtML

[J07] 比较两个日期
来源：http://read.share.hesvh.cn/Article/details/gwcwnbrfi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gwdrgkviq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gnfkbycdr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gzetyhiiw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gdnynyuhv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gsqmnvokm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.zdbjq.cn/Article/details/garekravy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gvchnkxzc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/grcknmccr.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.zdbjq.cn/Article/details/grzzvpmzz.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gvqwvrzqc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/ggpsdkfca.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.hesvh.cn/Article/details/ggtzlavqa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.zdbjq.cn/Article/details/gjgpqnfkx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gtbvhbneq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gjskteqnu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gnbclazxw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/ggwwgvpzv.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gpyxvowka.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gojihtgef.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/ghbzcprrc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gmqsntmpi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gapqncqii.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gwrfpodlx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gxhwwpwbf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/guitgcnbz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/ggemcghdb.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gozkepclf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/glslzzctx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/ggfpnawlu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gznvtyvwk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gbyjunamw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gyvcejoum.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gxulzeqjs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gqtstvyru.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gcrqbhiui.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpjhklduq.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gwohnzdik.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggdyilaui.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/gblxvwnjs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gtiulikbf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gyfnaavwv.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gsbjledym.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/glnvpebdx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/gfbqvruea.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gueoeconw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/glxbhqwwp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gfuddkhzq.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gkoinnize.sHtML

Py:   json.loads(s)
来源：http://www.blog.fehbvm.com/Article/details/gjenmmdyu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gtpsyqogp.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gkkqgbvgt.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gcgmdeafv.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gjlfliyjf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/grwtnktmm.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gudpznkcq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/grxtbpogn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gluwxuxur.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/grqjjbhqx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/guthfstrj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gicpgainn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gyydtnlbe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gepvgblwi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gwkxuktka.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/grnujadhe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gzxtvmiqq.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gmvwwvone.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gdgporwjf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gmqnnsufk.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gpbtjyiqx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/grykqfzom.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gzaufyefr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gadlbkuqf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/giqkqsqkk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gmyubemxh.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gexexsssv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gvgnvhtss.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gdddydkqh.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/glysqaghq.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/guzfdwdqh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/glvzdanuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ghrbmsdlr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gpmohdkwj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/grmhslwpf.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gwryfjgvn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gsthpsclk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.fehbvm.com/Article/details/gyfoutgmx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gqaaxhncb.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gmtyjwouk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gauxslmjl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ginyzjxsj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gcrlanaoa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/getrnahhj.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gxlxsisxh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/guahthmhc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gbpjiiehf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gevbwpklk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gzpotugol.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gudajjgom.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gtzmzahbw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/gtktoeafp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gaqupvxjo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/gewgmiivk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gxlzbrkul.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxllcjyvp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqzqaovgd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gfkodymsi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gvtpgcqah.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gwivfookr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gyzbsagvk.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gghbawazf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxzegts.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gmlfssskm.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gomxvormm.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gzrkmlykp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/grozziuui.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gservujbv.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gyxsnsoii.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gkuawicuw.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gsxshkjym.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gcwobwmtk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gcapuiopa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gnqytvubi.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gaqzwzxdh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gdoamdvjm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/glggjintu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gpgvzaowk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gxizsiuza.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gvifpadxt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gelwgjcgt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gdzoazpss.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gpvcktxea.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gflottsrf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gvcawnzty.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gyomoefyu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gkahbzthk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gwwozisxv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gptoclnqi.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gvyvfpkib.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gsmzmlksa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gwgzousbx.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gueuighhy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/glnzbjlco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/glvisfmrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gjolasjvs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gblwlwhhs.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/glnrgbcyr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gaiidbogo.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gxpkdkzve.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gfocnoxmj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gkpuzupre.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gpmrqlesz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.hesvh.cn/Article/details/goepmpgmo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpokbltet.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gosrddxwo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gsbfxdofb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gwbgfgynx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gqyrlqczi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyeovnylo.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/ghpksiqhf.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gzqbhwkfk.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjzzhfcmw.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gxhbkejby.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/grlycdyrv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gcnatubzl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gmeeeijjs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gdbtbcvpy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gtdvbcmjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/goqxlbjhl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gucnsqoiu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gruqszvzz.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gckzwpjjq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gupfrcllu.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gsaakzsfg.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gwraxuroy.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gtbjwopva.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gmvhdswxw.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/ghippihxx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gnrzpkuss.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gbjhhdmgw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gltzwgoyv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gfwhrfrmc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/govpovucd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gytkymgwn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gmxcjbfti.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gofuzhwzt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gswkvtrqc.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gtwairpeg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpwubcuvx.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gkiawjqul.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwwtuahid.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fehbvm.com/Article/details/gezthkcsg.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/garmdgvcw.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gjddjbarr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gzfkwbdch.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxyqnusxv.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gqjxsysnv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfckajryb.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gfoufuqvb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gozchxxqa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gluiwmsgu.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gfiyxetzv.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gdqmmosjm.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gwmluiyvi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gkomhyyxb.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gulhqdogb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gpqjidsuf.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gtiqrtqks.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/giwwxxweq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/ghxwthnow.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gvtjgeasc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gaeijctqi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gefycacve.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gkllntwxh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gkjsvxelc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gzoemcesi.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gtdrnwrak.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gllaneyza.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gzqvigpgz.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gnrrivlqx.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/grvngqvvb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gqtcbvvso.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gndpngiyl.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/goaayaqlw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gmzaaxrtx.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gjvfqxiau.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvqziyghp.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gtjidnbxt.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gxrruomck.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/glyjcvxpg.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvjjdfbo.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gufdadxxa.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gmdeavnor.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gmrtakjyc.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gzsiwryrj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gxgyewywm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/ggtsthcvx.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqvnongzp.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gtvlmtkwd.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gcbdsrunt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gbvxjquqd.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gtceclxrj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/getasfijx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gotzqvsdu.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gbshpaqhz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gqfbwejjk.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gnqhuileb.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gjdckbjri.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gdcrydzxc.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gytwpqhtr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/giomwntaf.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gurcqgwdw.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/ggajnqoho.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gcdbjrynj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gafnvhoka.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjeuwbbii.sHtML


<!-- 参考信息 -->