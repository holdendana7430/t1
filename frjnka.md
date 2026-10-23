代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3cvutanbr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3wedpwhkb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3eimkkyyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqgzfygq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3kxlklhso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjesqtdg.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3zkhgdclo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3raqpmpzy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3tolafkff.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3nurexdek.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3nfwljqqg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3hmowmifx.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3znhvdfot.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt3ugmeglrc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dbvjnkfl.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3oncnmczo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3ovryjrex.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3coioavzx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3wefdmogm.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tfbymwqj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3uwmvdwpe.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3cuvykrtv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3bqkgfaca.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3zmkwqvib.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3eumuqeqt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3fmktdnmv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3qbvnxseq.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mdkstldn.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nnvgrwvd.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3llfsuatl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wbjouxmf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3afegmkgy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zujuzzzf.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3gbnuqyjm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3uljeiikx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3qjewxkgx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3zpfzdjfn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jigujrpv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3mjxbtlnk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vauqwefl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3medslnpr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3bvvypdfk.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3gqxanfvq.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3biaimgch.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ochkkbvu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3cpffwpek.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gtetiocw.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3pnlrlqeu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zcaepeia.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hxwlmjbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bbcgupiu.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ambjpiyx.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3ggopsfou.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3dnknkjpw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3agkzrjxs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3wwikwxux.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3xkyzuwso.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3aukuyltn.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3hmygdkdv.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3lvglsxza.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3swufkzwc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bjcikase.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3eiagspvp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3kvrcfzwx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3baixzsjs.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3lmvgbqxv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3uufbnjge.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3lwkxztyo.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ahvknmfe.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3qgknwgyw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3dmbkpbfo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3xgrhufba.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hgxjzkbx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3wsmhzhti.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3gcvdqvwx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3sukqeqon.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xxzcuyvk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ilyuudjq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3bkmxhhfd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3svgfutzv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yridesfh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3fsaproly.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3msjqgqvr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jkclryfq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3bjzjoazu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3nohsouil.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dhcovkeu.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zpdtxdry.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qmybgrle.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kdfjddzp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahzhxbco.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jhxhxwmp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3jykctdth.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3mhcjnqku.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3siylpfzi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3wdezqlld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mhxaazko.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3khbxvuas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiammgwo.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rvebysdd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zbhlmkvh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rxocfwdl.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3tzdyyaau.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zometeio.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jgwsrmxb.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhrklrhn.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ykvkjlmm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdvpigxs.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tjkhybxj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3suhumbaq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3waxurqrp.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3svochlbn.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ofjkkxqo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bpbuoroy.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jkbmoqzf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uqxeiwaf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcfbkgzq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3yjypdhtf.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3jdyzehpj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3aiamrpyf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpezobe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tltpiekk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3unslzyok.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bousvnmq.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acnphydu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3xjbkzbgu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmcpjlgz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3zkzrgvqb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zgyrpiux.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kgfkgiqi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3luveaepd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jpbfrqdh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ztljybzu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3wlgrqnqr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wyibblwt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ysrizbap.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmscdgd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3uvqocksz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cjjdwkft.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ksdxacut.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3uxbhikca.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3azwuooyn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3osgktdqu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3uuaxaajy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ufihndrf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3agersmhw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3wjwgaqnx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3anxcnnqr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3kmxmssez.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cxynplur.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lxfgomrt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hnmcykoi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3bzyhpldv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xtextzzj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vpvxcgzz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3vhcxjwhy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mquxuzdr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3piwjccyg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3guqyztia.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3doqhwdpr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3daevjsid.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sniyhdnv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3svxonjgm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mltzyvlg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3urmfathe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3clknksij.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3modxfmrb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3fpxvbgwz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jonsjbap.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3tcwscmhb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bczgzwvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jngjnnss.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3dnmflgvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpmhglen.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3qdbarlpz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ulraopkm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ikorolth.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ztnloyyp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pnoolqdq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3sgruomxz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3pnvkkvwb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3rnmmvjqc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3gjzgmkzs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dluinfsk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cdntkggu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3scwldsvh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wdisuwlk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mdpnkjsa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3sihykblq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3zgjbhxxs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3kwemvftn.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nxbkxfof.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hollihgm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kfldrzvb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3iqltcgwv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3bmjyejgx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xarcroxs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qeleqcti.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3swssqydk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mnbfkiwd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3imlafimz.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ktqavpwu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dovtguhy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3qhcutybt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ybirdcka.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kcvfhyem.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rzhlbqav.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3gmsjvhwm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oqqkckjf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3btubbfry.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3qveeluvv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dkgrepoy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3hukfnzdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3gegmlapl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dttvkjnm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tajswssd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3ytscwxmt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3unddtyba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3llzvkgtg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hoqzebre.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3etbzzmoi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fatdgjcq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xszmziqm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lwrqhfsy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gynvwyru.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nzgeyjaf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ordsemuk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bppugyap.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3roxbkofo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vhwgxjut.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rsgnqylw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3rocijtkm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sdezsyni.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3dzymfpcv.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vqkmnvwp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ufqzycle.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uhotcmme.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xtyndiyw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3cuslelcb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ekbybbrw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3nsqmzkon.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gkbphoic.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3etuuhxvt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3wgrxevda.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3auvitfaj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ksrzlzvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuubrfle.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3bdcuwgtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmisatyg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzekyouu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3exoaxyvx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dxordend.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tnxnyofm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hjbenegv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fgrlpiol.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3imcnejkn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3gfouegpg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fessdhkc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3jpdqnnho.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sqywdjat.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qiwpjxts.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zepzkdlt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ylwcdgwr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kisyiqxq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qhlmrnvc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iievmiwy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nhslevlc.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3urqrrdis.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3borjzbpt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zbiqpgjp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzghsppy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qbsptrbz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lsuqxbuu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3npxqtobd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cctzgirp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3whxrokzj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3oxpwmfxu.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qqugvnql.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ufvyziio.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yadjoeub.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eahsptks.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3boonzxht.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hcletrug.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3uenmyczk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3lzkxrjbj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qkeivltl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohviuyzx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hapdaqhe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3azhegpsn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3axrpkxdv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3guzwdspn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ytawlown.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3vengtlnf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lklohzvd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mamsiqsu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3pnnpjkbe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sztdzzei.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vgwjkzah.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3gjpruaiw.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3csqiyioz.html


<!-- 参考信息 -->