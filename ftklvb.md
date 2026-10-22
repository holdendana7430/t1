代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2dwtfsnya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tupwfusw.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2evrrutgk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2piafdofn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2kcrxgzpo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2hbngfepx.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qiakoctc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2rmdoqklq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2klnanbpn.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2rygvplre.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2sbsrkvap.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2gvrybdew.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2nzntxcbz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2fqtfyyjg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2oxxqtixq.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2urwudrts.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xgjrjrsh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2wnuwsalv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2alngdpoj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2kjuyjkjl.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2nsfmrkqa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2xqavamma.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2pomsaezs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bbuhfspk.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2wqvihsyx.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vcvqflbl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2mnuxgchc.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2apeppgnl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2cfitxtnn.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2bmyiqijr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2skcokqrv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2yfdaldav.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2bxmkujnr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kwhrclbq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2adrjrupc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eyxskywi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfycat.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhmnmwi.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2dwytygjp.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2dimjrlrs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ruipankb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2jyrrrwau.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hehfxwxh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2favfrxqf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ssqbousx.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2eoijfxpa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2tbohqnft.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2xtogthxp.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ukjlxtqb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2nifdrdix.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2ulrfyhav.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2ktvpsvep.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2cwvpdveh.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2acnhenar.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hcynshul.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2awrebilk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2nnxzsqlh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ixmgygyz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2sdwndqnz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2hfdgsqwq.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2gtvkdkie.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kfalgpfm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2auficvmx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kbyqogst.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2arshwuha.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2jyeblsxd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2ltslfxwx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ycahlbhz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2odduugoa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2naqiimwt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2aegkwnfp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2sywgdjqs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2lsddmxfw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ujqnwbab.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qqavdbha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbczlta.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2zzvmxiwa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fqcdzolw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2jihdvpvk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2houzogfg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2iahkmurt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2lpcxaqhk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2hkdtjuqa.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2snwyxxgh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzmgilj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2tihljuja.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ofbvyftg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwnvzwg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hmrtohlj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2gnokgofg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rszceizl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2yozudjpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfdwczkp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2isxwyhoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbmqwazc.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2ukglplty.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zrbvxhli.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2uvjrtfog.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2fakboyfv.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hqepsqzy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2ejhdupuv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2ygjnjcbp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2zjkgtgvl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2gglwktjo.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2szksyjlb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpeqjevz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vnbczzkm.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bpuirhwa.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hqivhbwi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ziobwvdp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2mcljoert.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ucuwlwsm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2gpgebifr.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2pjptnxwd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2icrwrxyk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nnilcffl.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2mfublxuc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lijkuxcl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ldouhtej.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2lhmsszdh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwxgzckx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2zaehqjcj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2ubiyspop.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2lwvjvrgt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2mywlrlhu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2yknmrfhy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tcxiavyu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcljdyr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ibfbscnq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2slbmjsow.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xmvnjzvw.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2elfqbekl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2xuwjxtev.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ncifowqg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2oispzgrl.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bpjnsoep.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2uozwpoqi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2glttfnrv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2vdnuzjun.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2onzhqllh.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2onnwteso.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2hyqooaee.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ymgugoqj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2itjsivji.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tlyqdnoa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2klpaleru.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aeopqjin.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bstcxerj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kupzdoah.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mgglukyr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cwaooosg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2swhjkmpe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2flsuzinn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2algwcjrm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hbdjukqb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2seamiriv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2eyworalp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nlhwphyl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2iurvzrue.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2xvclxlsr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2cygfywsr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2orrydmcx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tqzmcsgy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zjptiryu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mfbabpad.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxhutcjc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tshwajlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afvwxkxy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rcdacijo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drtgdkqm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2kjkbyppl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2kcfslyrl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2ghzanfap.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jrhspgsi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wzeqckhf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vhynfmvt.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2whkidwau.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2upvvqrep.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lgngljag.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2undujcry.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2veylqsmw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ntdupxyb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2idgtfyud.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ujdquvxr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qkywkmjf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xjrkdfiz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2sdjyshtm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2tgaxtvvd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mdvbojiz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2yusbhgij.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vxumajmp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pfwwefwy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2iviflsyq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kmytjrfq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wtigoidd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwrwpu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qgdpupaz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2jvnfljdv.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jfvbcqna.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bnrscnjx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2mpwojier.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fofgpytt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2mcmvfqwo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dhbzpdbe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iwzyduwo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fsbbhhtf.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yakptolo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yypegcqe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vuxssjoz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zlusoxdz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uedcedbr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2noxizrxg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ijvyiqhu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2znpwiupl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixbgkjyg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qxckrbfd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vvtcbasx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2tmoyqbfh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2weclpntu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jmmkyesb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vlofucoe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ldslpjfo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cuclmrmy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fnbarjei.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ycylalnq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2jkigtlsl.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ylhptbse.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2grkroell.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2niawkqsd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tygeedbj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xznidhkr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2askejrio.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qxspblbf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tiidswdo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2tcdjztty.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2imzemhec.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2exqjdnsv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hmafjywm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pnuswxvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mupoytmz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rndhekix.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2qnslbsxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmkraepq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2awkmwxgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmfqgwlk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwarrruv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pxjaerox.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2dgxqwjnc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqhbjux.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2orbjulyc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gtvakkmg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2cqvefmcp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wlvmlenh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2umhnbhuf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2edutjayu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2spjnhfnx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hjrggjdl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2bbxxmtxy.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jppbswpp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eoqjihid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fiowtcfz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vzjghnog.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xdydvebq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wdmdrvcn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kwjzbxgb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zrgbfmur.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2risrfoud.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hxrztlmk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2tdvmvnbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yuorlwhn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2uagxyryw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2llamrppl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qocpecwv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2enhfjoli.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ffnvkeup.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gwshwubd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2itixemjb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ixsgxdrc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2zapkvgkw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2zqbxfonf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2zlsscwoe.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hooobktq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zufgixrd.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nqzsebsu.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xofhbqan.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsezfxzq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zmivhshz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxvmoolh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2idtxsgfk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rzwcmokg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2clprxayg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ggpqjshg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2dgcxxcmq.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fqpqfnko.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dcbmgwte.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2segsqchh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2efncfsuk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2fhworabc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2whnjbnyw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dpeyrqwx.html


<!-- 参考信息 -->