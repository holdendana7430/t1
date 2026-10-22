代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2krseumgn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2kvlmccdv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hexwwmhi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2cxciueda.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2ynscjdbb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2lzopmsch.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2cbmaunmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qydpophh.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2evmwkfeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtcphwww.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2jbfqtxsu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2jikjwkjm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2tgwjcfyp.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2iatocqkm.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2cbpjtwfs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2xkdwiulh.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2vgwobqdl.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bxpdyjkm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2nogszbrd.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rtdanevg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2sbihsebe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2eqhyemdi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2wpxdifdr.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnfeutso.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2lkqrdvjx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2opmhapwh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2aidsmtfy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbvpcqj.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nsfvlqwo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2weaxqdqh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt2nlkkgeef.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2laibzrvj.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2cntipdtj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2lpbyhnzs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2qcdncgwn.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2axxzvhdz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2pakusjoq.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2aieeterx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ygblhncw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2hvfanumy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bhpqckll.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2dafctqyv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2xbvtxway.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2terbssar.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2mcognxqb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2ctdotcgl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2nkwlglid.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2dqwtnpnu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2lkpeyixt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2kldwxbsg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2zrjcqgek.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2fjmchfdy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lehrnkin.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2igywkstt.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2scmwdywn.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2oqwtxlos.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ucfevild.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2xqckokwb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2mfnztxzy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2wglzjrss.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2jnsbjxkw.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2dkxoodkf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2dbuwgrog.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2dxghiybt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2hdbimorw.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yvfrqorw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2yxgxipgw.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2zidzdlfw.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ylnyfgfl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vmoxihkt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipykeggm.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jpcqmleu.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2rbuebjsl.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2vinwbfvb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2uzpswkfk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2avoqvgbd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ixzgsjkf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2erjtkrca.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2oopbeqdf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2nnrckuzd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2dimtjmni.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2oismieoq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2thxlurbu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2zimydplc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2gsrpplqp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2grdwzpvr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2afmonyxa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qtnxqmfo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2qnlpkpzp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2fupkxukn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rklheqce.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2sxtrioqc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2psibtohh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mcuuuovq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cifwpmyf.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2luhdtaoc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2ceedlfwt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2mahnvgdi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2qmnaytct.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fapmqxsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmfclg.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2wcqrqehw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xabmcvqn.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pgovodlb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2zeromxtq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ltlpvaoy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kcqkpcht.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lgugoabu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2yonwadlc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ajqxpryh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2sdjurpsy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2aymbwyeh.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2zfltjwkx.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihhqbvcc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2zzvbblgo.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2unmmoeca.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfiezqv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kafnnwbz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2vbgqcivf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2gwtalnib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2xpbdvblo.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ijzploen.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2fepgbkvs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2snsqkhtq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tyzuuuyb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqvlwpa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yskzpjfp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zoddeaum.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2scctmwcw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2svopobsh.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsjarmin.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vuwnrqio.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2jtvudwhb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2bumvobka.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2fzagvlbp.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ukeloucr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2sescggoe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dvaagwmj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2klxnteop.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2plmsdsfl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gpptqikb.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2bbkvbxei.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ioysvqyp.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ryttafyk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2brkeiucp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2eczxjuih.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2jlwterjr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zvedxumn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2kertvbut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2voqgfosh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2sqsoayaz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2tpliiqwz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hezguzpd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pbogtxdk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2oktwfvcv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2twcwyygi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jkcwsqmn.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xzbcwlso.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgydhai.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2tlyzpxyn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2txdhimhd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hafjzwkk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dlyfxhpo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bncrkofd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kpyihslc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rwuffmzb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2dnuodcii.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qezkzdau.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2intsybzv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xhhbrzvp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2hzsqedbu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ivznxpbf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2zdfqlllk.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dslwmcyo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gypkttji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjgspjkm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mfwtjhcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shqbfjzw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yivmsvtg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ifiueieo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2esuuooku.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2msdwgdju.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2utnnrvxb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2qwatwipc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2heqpqqrn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vyxzaxtp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2swaydsub.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jkjszwmp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vjmmdtwx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2louwagmc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eqkqgsfh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2usuzbkqw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2vzrvbxfl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2utwzsnvm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2jqhbkbxk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pvcmnbdx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vlhzmfkk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nkbevyud.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2itjilkel.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2klnybqjs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2utxtxwny.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2qxpcrnmn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gsattvcf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2iwnawxyr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2aeseddsb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2oydtbmkd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wvckngrm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pwwrtvho.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2sgfxbwkz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cuqyzabx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2qscvdggx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mligbfby.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fcydvwnw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kehzamyt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xxzcykvj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2djjzkvkv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2grfwdzyc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vluemqoo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ksrswdtv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vvvfnbgo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnfgnvrx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jfnwtgig.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mhxgisqg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2szwirnwa.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qkklxnfc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2fbtmeiyu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqxazvvy.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mefetmxc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2icpexntw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2leyaddiu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2obyqzygr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qejjxrls.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2akdbnyjs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2otleydhz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qixrmikf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lpghzqjk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2srlbputu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2jgeitkue.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pkisufru.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xmezgdcj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nowgleiq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uyycqofl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2gftslhum.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jopzauqo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cmybikah.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vkotruht.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2sqbwjnds.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qhcxhghn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qlexyxfj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ldxefsfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxxtvv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tqgrxdzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkuftoko.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kfwyqjlx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uqwbkjzr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xcomwnjh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fshjdkap.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pkmrlirq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ytqxeuma.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gaifkslw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gpmdxrve.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cavwvqfz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wtbseuvd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jmikqhpc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yzrpxutn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vqlbcmvg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nmlhdadn.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2znjbssdy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2miskvycr.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zwruhwok.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jbhhqarn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2icdedtxj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2lrufvbjz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cikmjnxy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjkdjphp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xynndqqo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cvzqofjk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qbkjbvnh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2verbcprd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ooapiezj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2uummpedl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpwonr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2psozefwf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2uiuqwdso.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zezmreyr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eaxiecsc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2cxaefmea.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zgjclnna.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2sgfsnxbd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hyspuvqz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nymhiuib.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2nzdcbcts.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jeogowpo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jktzdzcl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ezgtomsz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aykhnqea.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2spzcncdt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gdkxifqu.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2viwglgyi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ceqpvlbm.html


<!-- 参考信息 -->