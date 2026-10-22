代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vkxzsnsz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mtenqrbs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2mekwkliu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2stclkovw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2vgaptoji.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ofitgtla.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2chyauzhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afdysjrx.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2tfxkqanf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xqedewtl.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2fxxqvyfs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2tsgduwws.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ugnckdwi.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2gusydbwa.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xddkckge.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ssrjfxbz.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2ftuadabk.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2gkfemmab.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2jcsrvosw.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2toolxpsh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2gdlikuna.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2dycpfdad.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2xqefxgvu.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2chfceioo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2equkhgiy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2zbgzhxpi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2euoizvka.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2sebzdhuh.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2igzkuhmk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uwmacllm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2bfnqgjnb.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xyjkajcu.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xrluycga.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ymzcrtkt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2yxjubxrt.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdlembl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2iyrsobgk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2dtngvzub.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2epojpcef.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2ohnpqolc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2kaqzjcfs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2zadzsgxp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2cchyjwjt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2rktivgsj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qrhikcjm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hqeugvak.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2wyrpgeyq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2bkzpfrna.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2pipzaoxq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vvpamhxj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2xrowviwb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nkquehqw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2xwrhpyhk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2iyulkfes.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2kwdghsyz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2glatqvho.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2bzlpabqx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2xuklozrg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2mfnxpxsg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2zmumnpeq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2pzamjeko.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2zheikmgj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2cdzydcnh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2whegkfgh.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2enebvunl.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nczdmipy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2vewfngez.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2iogyirqn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kbrpjvuw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2leodqqdv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2edcgmagx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2emcqetfv.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kkpiuhju.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2vfqtiafa.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2wnwneukg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rpahaywh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2iajgjpoj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2nwgppsuk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2kyxbsrds.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2dvlnnxmv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2xvbxxgox.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pnapbvmn.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lobwvxau.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2mysanslg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2adcepkyq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2amdpspyn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qdjlnhlk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2ximgzzuj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ngfitljw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2ynuokcry.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rbgasxxn.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2wrobdwot.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2madbtkjj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2wialvdcj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2auazjmin.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gwuxgfhr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2rgzvqmfe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2mmtatwln.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ylurlbzh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2evsatewf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezpdwvub.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2mmowkhrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbhnxxzo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hnvusytx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2draqtxkt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zlxsicti.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pfvpwexq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfybemil.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2uvxxgdky.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jgjmiysy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2tugxgsjn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2kmrbacpo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2mgpwxjue.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2umlkzznb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jtlyboxa.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akhjmefv.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2emoxxzat.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bpndskhb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wmakrjln.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmiurbg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2njycvxza.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2dwbspxwt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wqsuhupd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pknftvzb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ktzljenn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2iexaayvm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2rmqiecfw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2pczprruz.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2ljurbagq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mshycpie.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwihvzvt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xkhtmtau.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2xwwxhzss.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zixzsdkn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ozmktnem.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2enzejjcl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2dvnmhtji.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kwtqpcby.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ctzwrcxu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2pnqjipty.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mnsbnzhv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2nakxtrgi.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nhpydkrm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2yvvunciq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2mikczdom.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2cgmxiqor.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jdufjlmt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2gjpyehzf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2hajbntsf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2usnrlokz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2adbsjytb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dkaeuowa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2isgsfbnb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gsfbtzlx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qvziufsc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ypchdpgn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jiyoxliv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hnfykefu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kleothsh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dvuwopdm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yfgntefh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2uwsgmmxw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bebridzw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mmytuddn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2mgaoomal.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2umersyub.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ylpyrklm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzdgchf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2opajbjlb.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2funpiqco.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2naxlatwn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2kkabjduy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ofdsumpn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ddvororn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2vmcauxlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjdsyrdu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2gurwsnyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dyvqzoeb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2roopvtrk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2iqmdqkky.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2mcgxyrgj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tvgcejea.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmzmawr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2pkilhpru.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tlrbjwul.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rkvuxcoc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmflhmh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fkvbtjvf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eypjzzdm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2vokxegog.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2usuddlib.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hbaqdtsw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ackmxqkw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2beiugsnt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ooltiqkb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cibhjexb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pptommmb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2eyiefnvo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2loqdmszj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zrkmbmht.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jfnhmkxt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dreclgac.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cdrdsixm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2pmrqiosi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2nsdumqfa.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rgsosamo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pokuzhfl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wkxthyca.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2iyosactd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xnmnhfqi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2axpykwob.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2riwoxsor.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gavaziag.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wvhfjbjb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ukkfvtpb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2edmwnbdd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zrhtemmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vcnwraru.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cdfplcqz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tyviqndj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2deluyipa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zkpdcjzd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mzggeare.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zoobrafm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ulxujarl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mxkmkddc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2uhdwvcki.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qegyfdxb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dzjjeuvc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dpqwvluo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2fmaddimn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2vpqpkmkz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2stvmjpgr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ccczwyyk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bushhsfm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wavktdsz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tkonfyzr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jwvhxttn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2grqieyxm.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2wbztsfyi.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xunkrtvh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jyyacnph.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yrxbsnkv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dgfjgguc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ulfnjiva.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pkgiejah.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2zaflahzc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2tzptbolh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2takachdk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2njmvisnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrtvshhe.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2enyysdya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwqtdxbm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zzhhrrlo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2phxbjqzs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2setwwxuh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2llyinphq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2puvurytu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vriyukgz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2exeimwhn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2pbsztfzw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2svlysxib.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dxpihaen.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mdlwamgm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2suvyrpud.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2klrpsfzc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jdbeawmt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tiaqlxee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bsfpcidi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xbphqhiq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hhqqsrqw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wrehzspf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgkolxl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yamhbdnp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2enrcptiz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xzqoymgb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mdtyhyyp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2snekjfzr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2twpqrpww.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qkryytmg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ypnuvqlg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bfordwcy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nwhewvtk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gidmdjej.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zvuprkyp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2lanlburz.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cghyzlvg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2goyqciog.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jnzhcrqv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kufdxabt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bmjduiny.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zzusxcwb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kpesdlkx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xumjvxaa.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zawnhrxn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2belqqemx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ewwkwoqi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2zokbdvrd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cppmhgeb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2yhkmcxoi.html


<!-- 参考信息 -->