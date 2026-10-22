代发 wailian999

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2lofjybgl.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2jampcpvh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2oznozkmk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2iisgyasa.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2cuxirtgr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2azkygfis.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2esbxmpzj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2hhppxwhy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jpfjziwm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcjsnxi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2ykfjyvsg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2oyjcfjwj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2tbeohrpc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2wwriruhq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2pltlvgpa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zymgtaei.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2adpqkrkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgjgtgvs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jfzmuofd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2lanjxopj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2lnbdhchb.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2jdzxksrk.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2bcbpztvm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2lfxhqnkq.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zieagrtp.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2qmrsolpv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2scfpsyga.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2jlxbyqfb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2mkllhqke.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2cvaakxkq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt2wgldbshj.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2twcwzofs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2gikdfspu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2gongooca.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2hinhmoak.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2pbgooqtx.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2crvmumso.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2uvzbcxje.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2ezlmnbbs.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rnrfydck.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xgwliahe.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2olncljla.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fqbgtgns.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2omfozzld.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ecpcnmle.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2kzjqtjqt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2ehjjkpdj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2qdanddxd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uzzcduxf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2wskvvnym.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2inighjdc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2akomrmok.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2drrvutme.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2fnpsmndw.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2mxkyuuig.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2hbtnnfpc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2rijtvcfd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2vqmawgtm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2ucfylvfr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bcubrelf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvcktpu.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2iotvjgne.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2aksrvfvk.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2yzdbigmy.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ntwzbimo.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2sdzwvzac.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2sjptvryf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2vbjxuqec.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2yimzqznl.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2wgegbtsb.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2uyozexdc.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ffokkvbd.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2brwkaken.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ykyonmcc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2sgqajbce.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vkdastaz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pxwlniuq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2vkwhmnin.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2ggolglns.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ceqhqkfr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ybwepoqn.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2xnonlimh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2vooqyrux.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2zqhfwynf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2tjyxyfxv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2lpjcoegd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2hrmyrkpp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kmiueedu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2zcvhukjn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2cxetzohh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2xibrcbyx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ynkrfhhp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2qauumsri.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kvsgjbte.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2irgwyfka.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2xaktugfi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pynaaabg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2kwraafxi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2ompsbllf.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2jhwnmqgi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ekgplhox.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cuoigvnc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2svyttwdm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nzsempqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2tvrkyuce.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2gdfwtpah.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2atftmcbs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lydstlit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhdgdjxw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2ddjbfddi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hybijkbp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2qjfofksy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ikveadfk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2sixskptq.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2xljmmumf.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtjvkqw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2jvcavhxp.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iosfnsmt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2abgajzdk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aoujplbp.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2qqzmadqy.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xalaubrx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2hrrpfshp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qobcvpvi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuloping.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhjbyzt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nfermgdf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wkxvzsvc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjsxjclw.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2yocprqdl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ynxpckci.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2kpihspqj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2vfguycub.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rumbhswh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tduxnsxq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bmotunpn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2shuqifjm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2onyxdfnu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2cucodqez.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2vycervfo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2zydcdmto.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jgbuxeus.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2weerybaa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aaqusvjl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2youytlec.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2usctsgvj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2kgtihbuk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2ozuyhhgl.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvclvssi.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2voljyhxz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2agjiezyn.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdrqeit.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lwpfhkys.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2omnvsvkp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2cebidevd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2wgvacnyw.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2fayknijp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2autvgoib.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwnrlsi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2dtdnemqn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ugtahabh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2lhsdstoy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wuukcrya.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qzgmizaf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lzjqmubp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2urptlwut.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uzoqiflx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ccqrvadc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wanbdoil.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tktvzzqd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ldfxswgl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2swhawnho.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eowsojoa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2utydvrcu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2iopnpvor.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nnodcwou.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lkutgwam.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jznuiecy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kzetsapw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2zufpheei.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2dhtjcwqi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhsduqmk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jatahvwo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dawxmvqg.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2fbfrrruw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dswvvzuk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2qhebwvlu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2uckryzew.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zxmvuwfp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yfjnydmd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2tnbpojwa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ufmhwqjc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2uaaqxbjh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2hfuzdnja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2todygfex.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vxzbqjth.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qpaixtoc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ywmvmhql.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2uegtehsm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lpwlylfc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ksaypyoi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2thwhlwta.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2llczvezs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2dtghvsoq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dhaozgad.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2fslnwsvs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzxjfejw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fphadvay.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2bhcbjfaj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kcqsrkha.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ahfemjyb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2awpnivpp.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vkxbejwz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2zhuygitj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2aorqkntn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ggrqqppl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2extgwsmr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehyoijxs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zpoqbrsm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2lqsroaev.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2pvrlcjna.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2nxdrinnn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rcjbvdzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2iwfiqqdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xpbdqiqu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zhlzvddb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wpgkdjvq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2wxvzecfm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2grrgltuw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2sjiehnvj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zeaobrtw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2gpcnruqo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dgwzwkar.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ttrwiebb.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ksuaifko.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dnqcfkvt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hauabcgo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2rejdkebj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2msfbgioc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2atlmlcor.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2umfmxpan.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2nksddaou.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2imbsiesj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2imrwfsng.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tbwqojir.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2iypsvdxb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pkownljl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jejntboi.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vmnnwhca.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2swjqvoco.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2yjskwqui.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rsijgkib.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nvtzxcet.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vcavrlaf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2vurhfbbe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fsnmothk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pxnptvks.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pznpgugx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hxgfaaqa.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2cuhuktfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyseuffb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2plmqfdho.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hgpbrscw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2prvewbfl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rbpnswch.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kevggxlx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2muhgyprn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lkmaajyv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wyuypuez.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gpksqzmu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kqhjpanr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gjppzgej.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gmkriogf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tcypdcnd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gsvhjvdo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jdlahyim.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nvghuujl.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2kuqefcud.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ckkdkujl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ffkjddgb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2hvbstrtd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yexqmunu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2odrvozsk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hhvycyor.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lcrfcjgd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2hxwcjmaa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gwkvwzjy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ukdtotkb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2hexnouwr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2evvsodtk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mfcbjofj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zvouuvgq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ztuwukkv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cfuruwgy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ospitlpw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2djtkrskk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2qmcqhpil.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2yhnivbwe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptontqfr.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lihciyjj.html


<!-- 参考信息 -->