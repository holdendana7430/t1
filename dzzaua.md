代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2zrxcigxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zxynqiai.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dpsfeiuc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ddrxkqni.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2vmndzyxg.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yeudvzxu.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2qlhqahqg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2hffrzjud.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2owamilza.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2kyjokcqu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2svbfoipk.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ernnspot.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2bllgkvkr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2slijitnw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2mgycxmwn.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2hpdnuqhx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2wvjkwzbn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2schvtlib.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2mtwutzow.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2otyyxgjb.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ooyokazp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2jychayrt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2uojbvmsp.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kkunrujn.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2wbgpgjwj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2avnpvbln.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tkjyqlno.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2zxykrlfr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ritgnigo.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2ovxatxhh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2nsrjugrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2rfixecxy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2jbyjraty.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2txcjqoqw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2mugeatvz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2awavgtbz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qpqglbkm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2bsdhfjin.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2hbyrnreg.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2lytlbmqv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ninhdgeb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xauakmid.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2cxkftjqc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2zrufikax.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wnthnhpl.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2vqmtsdfd.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2qwavmjqf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2feskhopq.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2kcuvcozu.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nvyjsztm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2dnfnganq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2gqdqqvoc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ngtisnuj.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2dbuzeehc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2uvauyfkr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2efvglnag.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2qtenayqh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2cigjowyl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2cflvuvqv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2dodkifdy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2nzmdeajg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzqovps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2zkqiqvfi.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tjworwac.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2qakgrngz.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2cpbkwffn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2gaqtlbak.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2jzgtilbm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2haohqcwg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2tgycgjpe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2exmakleg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2prxfeuzn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2sksnglyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2jmwxryzw.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2fkyxtctv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2qcajzdpb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2deheaoqg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ibrkqcnt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2yflpqadu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2uetslkar.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2itvwzvtq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2vgbzcsrg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2vtcqzpyw.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2rlnlgmrg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2jlkfkjnr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2pwyvijxd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2vlejrjem.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2namirixi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2eramrobg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2jwsuajcn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ymbyslwh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ssudqbkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opzshukl.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2vuklxfwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjhajukh.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cfzalgfs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fwlrbjev.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fjpcrbbg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uohicnkg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvoijez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fboyckoy.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sgogwyfh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2avtjmwcd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aqhmxfbs.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2yfmcrfnj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2boiggyok.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2furcoexc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uczhmnyl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hazlxqnn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlaovsh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2tpctjpku.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vgjvfugd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2sfucuyba.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2aapseoss.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2oljldqeh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bnisuieu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pclbivfz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2tvbowuyy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2swnyelmc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2hsndfkrn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktpnsdsw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2gjfbemgc.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qpsqwbpv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2gasilhzy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsbcnei.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2tofbpkmo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2dlabgdjx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tpiziqqo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rggfaixx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aargsdyc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dcjwdvrk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2tifmokyd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhjobcp.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kfrtgrak.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hycykkyy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qpgmqygl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2dkrbjkkp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2voepvulh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2fhfohdzp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2fykigtfp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2rdancprp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2tnssjavg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qhjjeokk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhihuuz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kmjjakjk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cmzitkeq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jcmbepop.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ijaamaze.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cajqvavy.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2uhcbbfmb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpdasqt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ukshdjje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2whaqmwyl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yykhosbs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uyjizfxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fpizeada.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ldapqrrb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mhkjesqv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2qyzyktwj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vorjwxhq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dupmpkgj.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mdexlmcv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hqrugzsm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2knbkldsz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2jhiwzaqy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2obbyqqdy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rfquvkeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pulydpwo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qpjkflpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohjonnnj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ukevqwzi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ydbrmbwu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ptjxthyx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqynffv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tpsipikt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mbumrakv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2lwvovpnz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mdkvjfaa.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2wnfjkwav.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cwlezuxp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2joqdwqpr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2dxpncmfa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yhpwiwqi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2duuzhyxs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tzloqxzn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iqpfrcvg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2hpyfkcuh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2akeiibty.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2xwdclouj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2gbrlgvek.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2glwbkndy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2naytlbef.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kgwwnebo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kvdnkfga.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uprpqoon.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2bzbmtlwh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bahiqlsk.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ybzkivfk.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2yregobio.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kptupgzf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vaqnwkyy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ygsaauts.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2krdbjhug.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2eaydhmtn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2abuyscio.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2vowmjion.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ndkkndfq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2mjzuisbs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2qxfwialm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zwzewsyy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gryfpzan.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kdwdnqmb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkpwgnyk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ozyptqsw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dodvdqkg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2audijhnh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bawhqxeo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fivjrfjk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kdjfordg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgabsl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2pjkljito.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2onjsehar.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2waplfgid.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2asijjosa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2uczeycmu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2zqhfkxhi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nmhhuyec.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ermqprsj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axiqhrij.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2idarfwft.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uvcuteea.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hwkjjomf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2wxobfedz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xsyltyjg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2cjsgevzf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2miafwjik.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hqzesbip.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2oitidksc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2rkpsyict.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zwuyipxn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ckjxxdmy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vswengcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atlhztbl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2uscauzfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zckufnbb.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bftbivrp.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kldlfxjz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2exnvdgbi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2tisbaxcl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2emohrtxh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2idklyabi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2imhpwkic.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jrxihhxl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xryywfzq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sdwwympm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ulujxmeg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zyqpaevs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hujodntd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cyetvkei.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hyngvady.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fkolcnun.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vefrbwpf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mtpenvup.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ejoteyfd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tahwvnpx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2jialjaya.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dailzbky.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qvhbnpvh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2otelugpu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ygacvupd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qblvwgvq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ndsriyjy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jxtzssfw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qpqwcsmc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2omrdpyby.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pdhifpie.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lfptfkrt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xvrdtecq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ayflluao.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2llziddgr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2nwhcigdq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cjicpvyu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sauzfqxs.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2grgnqbzl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jribzshx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzbmolgz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrilhff.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jqsolrrl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gndxayzy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ziycufqx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yzgwcitk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2oksqzvph.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rhnzqeqr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nachfaxg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mexsmgwm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2iggizipv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hclnsuvf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kojbnfkl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mcyxlmby.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dzgvwnvh.html


<!-- 参考信息 -->