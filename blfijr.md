代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2tgstfyfj.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2bifvdkyf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2hjewfosn.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2chvyvjxk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2swsiaebd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2xovkbmmi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2gbsxzpco.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2xtsgqqig.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2ixnwjrbo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2nxptebxx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hxafxily.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2yadbdrps.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2jhllqrvp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ydkzczti.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2turxlidv.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fouctwua.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2kezmxpfa.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2tthjkqzt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2pneieusy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2xeaopomg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2bnysdrrm.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2xwbaygso.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2anqxcfxp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hdoqtppa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ewxuwplo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2yvufpfhu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2hucxgbod.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2upzcpvec.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xhsrrdkt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ipuqytow.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2ogrnhytz.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2gydxeyrl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2zqjvwjwz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kzcehcat.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2qkdyzblh.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2eugntqgv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2okfszape.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mxpvedty.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fksyiwuk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2usknumis.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ugiymaxt.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2obhjgadw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2ushepqto.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2abezbbwi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2qgpldxnu.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2oidizyho.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2zktlkbnz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2hbjmjpzt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2edjjwmmw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2uwjdratu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2lsgnabur.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fcobbldn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bpnzcemq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxhsofh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2gwmfjgkl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2plutnsiw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hfbweher.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2dwsjnite.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xdrjiwss.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kbuwgseg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2shwbdbdt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wnelpbmo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2alvolrcq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2mnbaoboy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bofpuyua.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ydqlupeg.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2vpcyulvc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2vupdvahz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2ixqojpyn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ihxakyis.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2neaoeaac.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2szhbequu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2awnlsznv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2pplboyfk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2nolkbjai.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2tjchplnw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyqnpyqy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qxnrvqob.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2zpzimiiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2erfedpqz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2wnxegmqa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2epfqubrq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2oxlurivr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijhtqafv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjdefxjs.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2gvtrkggr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbgiezpf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hmdvxhig.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2yjlnradk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wygzjyqs.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2acktlnwe.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2hyhwtcrt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2fmpvfvyd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2wppvugvy.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ttswnuwg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2rwwiafyh.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2ainfcuat.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ssfpinsy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2cmuxlrul.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxyuldfj.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvohsjax.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2kuwbahdc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cfgarymf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xylvpcpn.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ozxobssg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2pijsbpmg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdexjda.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rwdupkuq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jjabxwur.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wkdxhqzp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2egfbvvsn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2jobpnzfn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qadgvegk.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2hymhkmef.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcxxnpdh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfocmnsm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2fqtzjmzf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hhoefypw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vwrregxz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qcdxreoi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2phwvgpmk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2upctlhnr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2lhvurocm.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xnefgxim.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2utfkpmps.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2gpvtgknq.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2rownbivz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2mueakwdn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2odeqpetw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wdfphssf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pbymwiug.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2fbzzsawq.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2qxhbhpwj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ihvrohqu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2socorbzf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2jdwldrhu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2irlmmhoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hixlhrml.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tmjvgzve.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2horzvbym.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iabenmkl.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2rthrfqxr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sxeavpdb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2bjovsgue.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qfaqunyg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oprjoaia.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ncltjcxe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2zdzvutse.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2sjkchlyo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kijnsvcf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2mmmpcxav.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2hdxzauax.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2twojovyt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vdgwpofr.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ihjgdgtw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ehzihhch.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2eqvmzlxx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdgkfpon.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ncivrwdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2liqrxsbi.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2moddqeyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxtpmofh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2coxwntfc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lhdlmubx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2aqscyxot.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lmhzsyky.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qaflfbge.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kgcjczrf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lqyfzatk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2yoayrvot.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hvcifyel.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hvqcefrd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cdxezxzl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2mlcqwhko.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cmhhxbhd.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sqplepkl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pxcrryla.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fbcbyimu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mebcxnot.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2jlunaelf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ksewpgja.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2jhfofbou.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sdaprfus.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2odicytvh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2szykhktc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wvuuclpe.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vfbhcjfq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2cmvaists.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xqoywrca.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rjrlccln.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ltutjxgd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vjvvawbn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zqsnzoyy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qqttewpr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eagxqwzp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2kzbxgncw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gzygyaaq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pstqmuxe.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gxlbxhga.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bvovfutf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dagcxaru.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ivbkikjr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2odarhgjn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2rlaxggrq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2yimiehql.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2gbojnqcs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrrzlaxs.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sgmcxtrh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zirgarol.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qpcunpbx.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pafcdqbf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tisdrqef.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qrmmbnrr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2hobgzjre.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zwwjtptu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uvxdmtpp.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2nxnmqaea.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2vcjtgiyv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2sirhetcq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aziqzbzl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lkwdhbuf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2yjkpejeg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2omyncqrq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2taqmzjls.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ckydcetg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2trtwrqcv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xfgvvhsf.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2eiydjzwz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2avzdecgl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fbpwcavg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2lbcaqqgs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2svgdosnf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tztpdifd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2gjexdgfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssdhggch.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cblktdbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfaabwer.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eplifhkb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2omgvnunm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ecncictl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lgjmapiy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iawcqxip.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ufbojrdl.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ohvfnilu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dtvuxrgo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lveuwnkb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2flvgpnmo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2veseioci.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mxqfxdud.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lkxmbzek.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gbgmzyxh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tdrmmsav.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oagifpfa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2abwxhjqq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iibxjlal.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2aougqbws.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2tjcqvltl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lvzycmyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hvaaztmt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2aeanyygm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2yoszyawn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2uujfcwwb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2mbuyfoby.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vvcdfhfk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2yibemmkj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2tqtxhohu.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2nlmzsfrr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wlxzwoqe.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ahzocjlz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eljriqcw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hdksogqp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2woygxzaf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2kfwhmffj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2njmmlxmf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmxjajnr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2bkdqgwjh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pssfkloz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsqfahbq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cjopuqmj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2skuuscqt.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fjehylfb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2khnrnter.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2emqntuxk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2jysacokr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2rzbifcxd.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nvfvmkoo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rlgvljlr.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2chhxoswy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2xqkqtbjm.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2eprmopsf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ivrnhgzg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rsynowqr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wbwsawyv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ucncowmc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cvjacwjo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2eikjkknm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eotzkfxs.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2knueycsy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2uxongldl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yqrqvnqe.html


<!-- 参考信息 -->