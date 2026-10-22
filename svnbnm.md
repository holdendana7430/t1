代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2jqucmcsx.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2kcwhdjvm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2kykqrkbb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2alrtotup.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbonigu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqtqrkd.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2qrmpvooq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hkxlyvxm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2nwguazam.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tctmvddm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2fkbnjwpy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pskofkdo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2hpvgqdks.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2tdgpcrwz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2odbomrgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzbnlckv.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2jogisgur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyasmuhv.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2leqmpatr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2yqehyrvp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2ucfalfmo.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zxfdgjwg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2ekjquvbw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2squbbbce.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2agbpaivc.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2hxiajfyd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2zaqdtqwd.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2wprfuurk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2majbjxry.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ygaldmqr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2fsmuyays.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2rvnnuhza.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2xfsmnhsi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2ycmljiev.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2yzomayag.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2xgilecty.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2falwchqy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2nknirkua.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2njfspuzb.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2fqxgluye.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2sznnwuwe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2muiqtqil.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2uneyeavw.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2atjnkben.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2ijreqcwv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2oghmrapz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2luhnxpic.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2aoretkbq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2nujsolwf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2xkojgxic.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2deslxgmq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2fhgvwjzy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2jrrpowfz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ihlsdkeb.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dhqimmry.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2gdmxoyoz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2izcqvvdc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2oypkqmlr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2mdvmqkho.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ttnokzyc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iutaomnm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2nhpwbmqi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2idfdtogi.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2sehpnswi.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2anjzqgxr.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2vcyqrwss.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2nughtyyv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2xovlvlqn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mtfmafkx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fomtxljj.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2rrfmqfzs.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2qdbspyzk.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2gkuvhfzv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mgwgyfyx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2nprdghst.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2mzhxcnhl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2vwcvezeb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2mqnwruxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2sdanpakt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ubnmfpuz.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2kvwkeqeb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2whwvykgh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2joobaqne.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2gsivjwyh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ksbrjtsf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xjobwkjs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oyytdssj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2quixhxcp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2gtaawexn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2aqyhnxsd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2agrmriwj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2cmpxkpvm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2aqczatob.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2glymlilg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ujlkdenc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2embywbyq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2swczkysa.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2zcgbjquq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2wlywbnde.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2tgccsehy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2cxvpwoow.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2hesztubn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2satzteoq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fzkegham.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2hsndxyyd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhdylq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2pqipqwhm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2fupmuqkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omzseceq.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2bcptefzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oitdrgyn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yxagipcc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zscluttc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2wtjcopki.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nvkbqkmg.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2snkzqsbg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2xjxpjnwp.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2lpeqofih.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2fjefbuok.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2icdqwfjb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2mznfqqqn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2ztdcbkmz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ijhblead.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2dupclhey.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tyhltkok.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zsrksdij.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2aigpqmrq.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fcrxyhlz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2wugovyqm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2mjjpfxrt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fjjptwwx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kaftzido.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2penmzrdn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vovenwry.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktostbdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2xpmydnwj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jqabxqsb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2qzznpdrj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2cdlshibb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2uyzvpsdv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ckarcstz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zxvjqqxz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxuwuner.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zvmtofsb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2rwodmkcs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gjdpgdnl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2nfckohlk.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2mketqsin.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hgkdsaps.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2jcvuewai.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2puhntouy.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rjfhiswx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ycyrvzkg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ykzoedlk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kfoplsrv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2gluhcrtw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2ukqjphwe.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mbhlubqf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2cqkjavxe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2drehzsgn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tifygoue.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ozouafol.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ntivznin.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iujopomc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kuajzqst.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2mxqjowvg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dxubxucw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2mkssvxrg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yrzplazq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xxbdwxyx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wfirdvsj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lmqcppmv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kvqrivpd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ioaczlwv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vlfdbury.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mckppsfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2siarwqtf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zusyfbim.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ydukaoqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ruqynfer.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dqctrbkl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nceymcqr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tgtwesan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jgqzxlpq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ttvuifbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cktavcvt.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mhgwzyhd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wkhxlldr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pwpwjcal.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zzrddqud.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kyulypov.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ufxdranr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kyhvxtpa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2oakttidv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2apgtxcdi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oebtcduv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2izyupazc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xxvdyhyc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rceqrtbp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pmtstsqk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pyrccsch.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2hwiijfbh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rudgeovp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2nveewgru.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jxouisrf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qornihqn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ikbmgekh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kcvdtwqp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dxeoznlr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2vexskmlk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cmnnokjp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vpfoewca.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2xcppvgpo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2blqhrgsz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2zhvwxzyh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qyimsaok.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kqvqbgnr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hymhwadm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zdjamlxd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2gryoygec.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtyehoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jrypciob.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2avtzgbca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fuqonipv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pzsbwqai.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rwhppefd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wbhvqzlh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cpuftavl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcbtjhgk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vwxvnhui.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jozmmqlg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2kahwbawa.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qnqacrzy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynnjvzzd.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2sdfdrvsn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2smpplbov.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2esavqbeq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2bbnfxefq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2hqwokhvf.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ttwmdcgh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2pjoffwny.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2larcfqak.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fibdunkc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xyccqvmw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wqlbaepe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2oehebwkx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jcnhpiqw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2gkqydkan.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mohwxcwh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vmolijth.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ugaparci.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2riwwmyjn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bqxuiopl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mtputftm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ecielzcf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2bwjzvlhx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ukfkvauf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zwehqxum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afxfrnpr.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ronschmc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzwnwtzw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2crejtlvn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wirtrmbb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2lzsgpsqk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ocyiwori.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2keqksmed.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2itauxjne.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2etzgdvxn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zollbrzk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cgydwqjo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jaxxxyvz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2srdglzkf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lueuagta.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yfembxjc.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2txllxdop.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zrgxhgeq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wjblvkfp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2hvemforo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ellnwxym.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2khbqzflq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2atokzzyq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2pmbsgvdd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ithxfgyy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2uibdeucw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2obfdkfvp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ctowzfvo.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bdoehuvt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hmciqltl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2vwzdraat.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nxbirmql.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ehweuojd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dhcwihxh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ijckuqos.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hctgnghz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2gfqqfyxv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iqtzpcrh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ioyrklos.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fbhczcxa.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2njpjlrop.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wjulschg.html


<!-- 参考信息 -->