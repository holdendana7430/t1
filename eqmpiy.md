代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3frmogate.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3savgqvvs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3oxzfernk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rusfuusd.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3mckpevwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lijhbqzk.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3dsivaizz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3uxhjictz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3brojrhum.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3vugovgeq.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3cpgbtkwe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ocjecueg.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jneaxall.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3kblfadou.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3plbkbpve.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lgbzckto.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3jdpsqyan.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ddpwteed.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3xscqzvxn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3nleekjda.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3hkmecyez.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3eiygsoyt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ocgflejy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3hgtipdxv.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3uqrfskuv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3mjysoekd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3boekdbrg.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3rlesiirg.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qnvcdxel.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ogfzegeb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ndvucaxl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3xphmwkcy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3zqycdtzt.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kotigism.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3kzwhtvaa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3npgavgxd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3cstzpqai.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3oufsweud.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qqpchrxa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dgbcvlpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3txxoadyn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3jarwkqbb.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3pfiiyvsg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3fhliuczi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3lbnzipfx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvdphhs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hqsvdwuv.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qbkrbiki.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3edpqlstn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3cxzjpchr.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qdmopioc.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3jlkyhbrh.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wdrcrmfj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3byxzmvdg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3devnojtv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qjygjvvk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dltpfgto.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3wmkarwpd.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xembtdoy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ctqvvvyn.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3xfhybqls.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3euotcbbn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gmfniwdv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3vhvawctb.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3stughftf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dkogiqgs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3vscthtol.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3elempkct.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bjljlgue.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3ubxdtweh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3xttlzyfu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ygcfslyu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3mcmjdxis.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ompmwada.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3nfyjmzmq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ptwsqvrh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3ygghxjmr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3xhimeeed.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3mcgishwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qowkpujp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3osormnrr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3xittwsay.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vvhllegr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3mysqwgyd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3yxoygjhp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3fdzstoax.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3xobkmioj.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jzblehil.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ljnmeppt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3dllywmim.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3neomfgir.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3swusmszi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkhuqpdl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gdodnvgr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rwwjjcmm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aurkzpgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abgvomst.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wdcwpgfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwizvrrg.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3waxyzxwm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lebxdhap.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wzcqizwa.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3awmunzoo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hizfnmom.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3zbuheclj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cnulclxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3mbsuxpjo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajqlbmdt.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3ziraagrn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3ffszfkmc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3mrjdttqs.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djofwbab.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmmswbm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gartzqyr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3stuyvkoh.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbxajkp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3zpqpjhzg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qaztfkdc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3debqyytr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3jpyhimdi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nznrrfmk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wisegaid.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3vljgxewf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3kgpuoqul.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fdumstyu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ymdcjlth.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3lpxzrfxl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3qqmvxbmb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3veugvuqp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vzslqlyj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ymxidymr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3hzgqdsmn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3pxdgpugr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3bqlijbwu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3qmdqnrra.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3gknklbje.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dntrhzsd.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3enbqlqrg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jlmnxdva.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3hsyalewe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3lmoehdoa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3ccabufcz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3qxdvuikx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qicdwimt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nmiecfon.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xjbjivcv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3tabmaebn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pdukzpru.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tvfwthwf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tcmrvyrg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wpfxxwdb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xefiakfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3atmufxsv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tlzcrtsx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aunerpii.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3hrcjtafb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lntxxpdx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzbpgen.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wvlanvgb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3etelbwdi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dzvpotmu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3anaoyilv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3hpuhamoz.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3kzadwmlw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wuxcmgoa.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zxobiozz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sspzzgaz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3uslvwdcs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3bdijvhvg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3phctjpnk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3xzsiozcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwarfusp.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3wywpztos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvlgddfe.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3msrypels.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3pbdfphmv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3itnlhepu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ivjugnea.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cseukpio.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3rblkizqj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jeugwlok.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gjtlkzye.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3axlsiesk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rvsdzddo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zrqctuic.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3tbmwobsz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3oyjbjgua.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3aivgkvvy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3enxdismi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3kbvuomqr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3uxshgxcy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xglwtlqy.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3dlkkfygf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fvewpsla.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cvqusxpp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hqrsxiaj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zycrnseu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3davwdzbw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kuxjnikx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dqgekkjx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3doszlegz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3iepfuehv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3guoblhrj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3wztpscki.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ifetssmi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ffjxnwhh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3zdkqxklg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3pxafprpn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3xgskbxqw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3pfpfmsdg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3edjlobzm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3qbpbcxvk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xjmeaofd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3hbufqxuu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3qcweqjsx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ukiwsewl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3erqlqsiv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cedngeoq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zuwqeefn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eboazdrr.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3daqtoqhb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ksacyzqn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ypymtdlr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bhijwoxk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hamktdei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3plmypggm.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3pluyajsi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3dxzbtggx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ltxeaznf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zlgqzflb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3wtphyfnr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3msjkgatr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3coflcwqr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3plnnywrl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3omiwcurc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ynbxsfsx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dbzymwpk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3vmgyxolx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3hjfxymwr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3brcpurti.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pfrdegvq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3wuangoei.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3otkwvfxg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3weyiueos.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bcgvyqhg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ccksjdmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mydygisx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3ptspilkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujwburoi.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pnosruot.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3sgosgivs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pzfrmsya.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3kpxcrzfh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pzetxdre.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3cutuzuym.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fmqvqakl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bbrcxubl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xhnodkkx.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wmxnvqxa.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bkboyhmc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vghvuhpq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3caqafspl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3smcbehjv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3thhzfarm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lwiawibm.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3naofzqzy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sdftfvvf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3wcxzgilz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mqcefoak.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rdpfjipm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mwzcwpwj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kpzygbod.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qffpwrxw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ceeeyshb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hwzrmjsw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3elfjfmor.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3dphzjepq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lvbegwdt.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3oabaayyt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3nvgudclp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fdyyjlnv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3qxcextat.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sczyocgb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bbvhftuc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lajzange.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3yertledr.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fpqwacjz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jlhjlvay.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dggrzyma.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfdsrkbi.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wngbwapy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlekxgj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uvxlunpd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wtivrrge.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iwgcgfsp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3wyivnnlb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nnmhvtpk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xihjbjic.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kfizqhrc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ageraibb.html


<!-- 参考信息 -->