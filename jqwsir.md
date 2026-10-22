代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2xjwobfzw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tsddnjtp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2vqjlgmyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yixxwbts.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2aeivoboh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itlygiou.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2gbbmbmbj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2noautfjy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2alnhazwb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2grpqnmre.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2efdlpipd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xboyjdhs.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2hknjmbkk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2wpaiityh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2frfizqib.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2xwmoamgj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2oxnvjjud.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2qdgdqgkt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2aomuoiop.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2dcefhexh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2cwffiecp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2iqaokjqg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2xlsnjfpt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2priimutr.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2znpcsmvx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2rbprhrzp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2muugrbwf.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ynfrtpap.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2zinauiic.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bfqarfir.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2akugtaxx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2eaqjrkdk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2qnzcmext.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2egbnkqxv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxupgnt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2vvwtgiab.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2pslgewpd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2gwkysnba.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2mughdmia.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqxwnyqj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2gcxbefti.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2rrwdrhlv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2diuuwsph.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2miycltry.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2jqhomrjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2llvsbnin.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2gryxtdfc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2uvtjwekb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzbnkwe.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vcrsxhbp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2khxwtmjn.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2ibjzrxlm.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2bhyfytfc.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wjzyallq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ilgeehfc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2mcicwdhu.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2fuxvsvhy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2owdzaglk.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2qaziihge.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2xlkaeiic.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jiwlxhyq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fnzbowwb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2qziefiqv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zudukdvx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2sufiussj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hdsnhzwy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyqqiphz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mkrckoei.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2lqsqbqnj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2yaglniwf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2rmrucykl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2kjeyhuvc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2kmhlmuqs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2ggmuljeu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2lenllajs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2cjsduobd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ywmszhsr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2rmujoifc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2labcljjx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzsvsbj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2riwpcqvq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yuboxiez.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lmlxlcjf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rboaygnz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ensicgay.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2pwczmpfr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2kxjvooqf.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2gfapdbqi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjaxobn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2yqensvsw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2bkhsgqlu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2scppohmb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ywhqisem.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2dztimgme.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2yrhamubd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2onjegalt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ucodepfc.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2blqsqfjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnxylbqo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qnxtpkah.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2krlfezie.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hbzapbjd.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mixnageo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bkpmdmld.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2qitlaefw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oufpzgxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2sbpnfsto.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2watrdykb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jaujmkfw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zzjphfax.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2skscnjrq.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uhuxjqiw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dfwubszx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gwvysfrh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2iqgnjgib.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsezovfs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2cziefjua.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2xilyxhlq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2kdzilasj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2abajpoxh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldtqxaor.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsmebwn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfyytzbn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2jafeovni.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2lqrwajtm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2fszyztbj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2znxefkxk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2brjooqiv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dbandqdj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2qaqicufi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2dqzwykuk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xhcmhito.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqriij.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pcnmypfv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2vrmyrlqm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mjfqqbsg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iykjiege.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fhuwktxh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ogieuzfg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2urpeutni.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2wrmywavq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ognuehcx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uxkscemv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hlnoqatc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ztwpxbtw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rosyuwgu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkahgxte.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ompffyim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nlhyteul.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pkpqkwgj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2dnlgpqok.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2xovzqdxt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2borzdykt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkdmlrjz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dxvpeoxg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pzmbmydg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2znssjtnj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kiedmqii.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mqsgzmkt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2mbrewqzh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ggckantg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wnbjsdzm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2eiywyrys.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkaltlpv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jywqvbkb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tqkyjsbp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cgmfhsgc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2iwvyenrb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2qimbwyih.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmjdobo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2epwfipcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjnkawjh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2avpctvsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pklewlmp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sqtfwhnm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dblrnrmp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2sdxcyxsm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2muagwpsv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ouspgwmt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dbdlgzcz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hznrsqsi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2kbqfhngu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vefcqbjb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2icacdhqy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2gzdcibyk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2qdzrvled.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uuxlukgd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2saurloxc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2kcagrhyv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ibwqmgvh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jncbmdzb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2qrwfuahn.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2irpxlqbn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lzuqawgb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2powkcscb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pngbjimc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xpbfqphm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xidtusph.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rncljaiu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nysuowhx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rmrfggpc.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2yhfqzpui.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2qpzjgmuv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pgixplna.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bwcnjfwe.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2axqrsvrr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2adrfeoxa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pxoblodh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mmzoglkl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2daoxpzhh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2vlkxqpnf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2amvchslw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2bahmzmbi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bhcwyzbv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ivsbktdf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ajnklmjb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2oylbapsa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ipcmmrsh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2glczjbev.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rzqhgomo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wjapxxxw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2adkasafm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tygfcupn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mhgxhtjf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uxokucic.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2dhwmmscu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rpgghkab.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2uwvgtdhj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qobujzfz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2weyifnmq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2urqcjrlh.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2eqwwwjyg.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2erdwctjr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pcsjznaf.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2upszycad.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bobnqdnl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zoitgaiq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2nhwrfxdj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zruyulsv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mwghfsxp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2krambeun.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bmaqkkab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ixitjlfq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mbpykpwi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ssjowyzv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zisipeie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxrjgvnt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2keqycmhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtuwgghr.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lrlchwqc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tutcjnmz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cchhgfca.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2roxiqjkj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fuxduvfc.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cgpdshcp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tikizfzw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2nfkmnqok.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cednzapk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ngbhkqeh.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hpbjzoet.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ntmmpkai.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qoxdhqze.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tegkebqz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kyyxhtmv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esqtpjra.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2htldtkxi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wkckiojb.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2msxosgfy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kvhouhzw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2glqgkhpz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkfykdkw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kjwxnzrq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vhoaikmq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2bnnerelb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gccootpp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2somaaumf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tkgzoxis.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jskrpjqn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bbzihosc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qlotdwep.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dohczpdd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2yahpqlrp.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qcxwiwwy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2izcutfeu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gtmrfdrv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2coasrrem.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyoqsaw.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bhlqqypj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jezrwbjd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ynzcdcwx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bfurilng.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ncbohzab.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2snyrplye.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2hljfgdcj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pmmhhdeo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hsfwjngq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ztkgmivg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bokiyndr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qgifpkhy.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gozlbawm.html


<!-- 参考信息 -->