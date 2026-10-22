代发 wailian999

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2spmdfxai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swmnpqni.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2myasherp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2dnasyoiy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2zoirxmzp.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2rhnbepdu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2rhxwjlwj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ipsgwubu.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2cfqgrdgz.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2nayktrxh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2idwxqikd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2slsxzmua.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2aupaejwn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2piilzmnp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2ppyhuaal.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2mpfizjnj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2wqlgrdrs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2pfslypoj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2ihldfysi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2rhfjaxda.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2qhizcvck.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2gnldubsx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2prwuuwpa.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2hgeijqpb.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2dieibsnk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kszjbiam.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kzzchpan.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2yojprdmn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2adzprkeu.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2uythumcs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2qlndzpop.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2jehuvxah.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nqdhqlzw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2creumqul.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hnlciele.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2coggvofc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2brilawtg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2kwmozkvr.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2ubcwwuer.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2aeycnxme.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2udbixnej.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xgkgzzfi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xuodqopu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2hfwqxtnp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tdosgpjc.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2mzmzviiv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2spqmcnlj.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2zqpztreb.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2monugdah.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2nkracckt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2orptbliw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ckrrgnhf.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2emzakshg.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2htbxhtkm.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2butxsuha.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2eefetlkf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2thngkqzx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2gluiymdi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2gcbnezwh.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2arjvqoaz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ersxolrd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zcvpszzm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2laxauemz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2jmfujbod.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2idbjmavj.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2hbsqwnrr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jgosxaqv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gxfouujp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2covsletm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2adrifiqv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2xzsxddmh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2wcoassww.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2nhzpdncr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2fuilatzb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2idczupgp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cxpymkzm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2frtuuzqm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fgremjqz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ryoagles.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2glfmgifs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2osfcwvtu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ocycuuld.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ujbjnwou.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2anupzmtv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2suugficg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2pbxzelvs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tspdranw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ooaqpejs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cccqpucl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2eibtpyho.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kxgezijt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxmtffwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xktjqgas.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2wycxlwxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bktpdixy.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pwketpzl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2aeraumzw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2mlkjgysu.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bzctgsgu.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2artpbtzi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2udlbszmp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ztddpymd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2prorzito.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2zeivvnho.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vbccgyfe.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ednkrvkc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2zrdmezvt.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qbdtycum.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xsxwwmig.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2vxfuiazd.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ujekzujr.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2veoylykn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvkqrrio.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2uvxtztha.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2evudylgm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tgvpahce.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2aexltdwo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fcvbvubs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jydabtgi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2mvozepch.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vgxkzbwa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2uizvtxqn.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgwsivsj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2scmpgmme.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bbzagvlq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2daozjfpo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2iatijblx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2pjwzyfsb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mfgeyxva.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2eamfhxpk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ryyxnseq.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2vstvleip.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2aonggpps.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2jpcafmhi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2wmplacbq.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnbwezq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2nlrziqvb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2jfzrdjjf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2smgewtwm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2bmnprjpu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2gxfjzodl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jiwirfos.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2eqrjqzpf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2orxmiuql.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vnvwxzoh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2hasclwzg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qareqxbr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aiedmhjf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ztztarig.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ytgyvknt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gxdgcxgc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qwkvmpkf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2awhpsobn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwnzjax.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zmytlspu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sbgprwdm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ztmwtyom.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gwiaezxz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2keibxgez.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lastktnt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2feoiderx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gjtycgid.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sakgoqmd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ipjrsghp.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wdhdknhi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fcbsggkv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uhegspos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziyqhpau.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jncxnius.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnbadyau.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jdaondwf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mclvmirg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pejkvlsa.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dfjohgyr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jmrikdzu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2wkrgpgsu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2pesdgrul.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gkjtlhqw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2fkipannt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2opcwkaxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vxxffrre.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2onjzxapx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pdwzrppv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sphgxwjd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ayfviqhj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2idproxsy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nphvakao.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkblnwac.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2qliopgvt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2bdoxpmrr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uaaogwqb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jlercomv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kkafltcr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2torhzlop.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zztgyyfa.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2knjtrdgj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2txlgjlgw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gxumtuhf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2czalanin.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xwkcbade.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zojbpxcc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2kmhrjafl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2cbbwdhas.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lagxmgay.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2jtdwypfg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2hfbnhyrk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bcyyvbhw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nzsobqqp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fyvupnjq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2uufweadr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kxajwiii.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2yksimhoi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jblphqji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vjnrifeo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gbmwnyoj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rlozwxeq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vxajnrop.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qmmajvxf.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2govhdqnh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2knfwqoti.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kfxhbjef.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ocbyzyfi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2aetkqwbb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kiecptgz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2keyoodtv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2tubpxvie.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jfnjjvyb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2brlsicnn.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2viufiedu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vkaosins.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2eoomvkmv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vglfjdko.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ipgscftm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gnrzznpt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tqcfamjj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2vhmrpwyl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2muioicmu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wyddsext.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gapcfjzu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2svayjozr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2empofzfv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2iafecpsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gniwyjwg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cztyjonr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbblauwg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2pcsiqllt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2isykxudh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2cjlvkibf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nsiepjby.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyxtemwq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mvnquhse.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2odebyjpk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rlpghiqw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2vojsfabr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2mitczoql.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mzkelcjb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pccsdexn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wvrcjwnp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ahjmwdju.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hzorlnwf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vyqhyhev.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2btmosavx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jplfaloe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zjtsobvv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mmpkluoa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2lkfthgsc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gsugffkf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jtaatwse.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mexzergq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2znqqnxyh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ccftyprk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2iudfxdww.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qhcixbgx.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zbckbehq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eslubskk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fprslbmr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hfwxidki.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2tjmlihth.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qzfxxrgz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xhywjrhs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2boeesqzt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2bfttbbvp.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kzemryed.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gksltbni.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zesaevmm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xeczzcdm.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sydzzxbj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jlqfhzyu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hcjufwaf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nmwkqjla.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2onutmvvd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xsgjpfuz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2acwvizov.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywzxhieh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qahqrprh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ufepkbmt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mhocsbek.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2khuarevm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mcxdqbsz.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pyzomqxh.html


<!-- 参考信息 -->