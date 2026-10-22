代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2lxywfvvo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2sscoadco.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2pgefaffc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2sspbztui.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2icfmivim.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2hwocdzrq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nkqzejmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkvrdcke.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2ecgvzyuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcztazcs.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2zykbvhjs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2fpaffaju.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2rastdqcz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2tsxasxnn.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2kgkvhans.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2mfhcjesx.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2xgcrbmko.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2vvttxfym.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2crhhmvxb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2qonqhpdr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2vfvhskex.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt2gallkjxw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2zbosrqhf.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2vvxxdyzm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2vhqtespu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt2szdyrhyx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2obwjtdyc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2brsvktep.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2ingpmxwq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2ufrxhoct.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2jxvjmzsj.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2vcmoxvos.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tgzpyjmv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rzedwoxn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2rtwynxke.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ztcsbnxi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2ppnbenil.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2hnvjiklg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2qzkbunsh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2iqtbblkc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2uimyfoey.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2egxooywh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2ibmwrmzf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjennlcb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2suvvauhw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2hsvatasz.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zlejrjmn.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2whocmbjm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2wpsmlqur.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2sbfutfpy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2yskpcdjo.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2pmovchtk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2mpggqktm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xiyovqwy.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2ifyhoxka.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2puarnfzu.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2mrivqkpx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2atvvfhcj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2vdnthqmc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2fildshpe.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2efxeikqt.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2whuptneq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2lekjfwlw.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2nicvcfxc.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2quvnyxnm.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mxloqniv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2kymhuygj.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdhephg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ejwqfdqr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2vwvnlnhd.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2nioyktbf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2fognbfbp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kzvxxtpv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ledkoxsx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2lgusqjha.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2bzydmxou.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ztagiihb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2wkmynfeu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ywjiljcx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2rfxwyrgk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2bcstcovt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2djjnyrfd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2sfjlrhjs.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2csbzrxrf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2lvsmgnau.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2lscjnqlw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vtqspzoi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2vxsdxszd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2cwfgtejh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2xlhyogxi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2rfmpmnzx.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2iumqlunn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijutfgzc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2zwqrcvix.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2fmtkgrlv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bboalmgu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ibwntkpb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2lmeefmsx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2hfcatmaa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qqniiqwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upviydxi.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2cudetzbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjulwuhs.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2eqjsltgd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2yjkqzxcf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zqiiqewt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2usjrctcq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2cqyfdqrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2gtafgtkk.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2uoaiydti.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2lahwocyh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qhgzmkgg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2bneznbqb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xouqjtce.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2fvelqqlr.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2qsdjruls.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ogsggsjx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fpkwjtyz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2joinsxow.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqdexha.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2fdzbbvze.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wxywyizr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2kzkgvyvk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2axqkeume.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sripmvqi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2wbksptrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2iezprupr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fdijzlod.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pzpotuyc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2xkybbywd.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pwoubpfc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2yxvtdkyj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2guruzbpu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2duqloyzz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqzkrufb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2twjslrsu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjnuhty.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2uhkkxwdg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ygmmefbl.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2qxvrdzkc.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mtijfvlj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2hkekjbfv.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2trpchzjx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nwlysptq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2bzwplcgb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2bgckntoc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kdwtxnzg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2ttjmddir.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2rlzawcdh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lzimuyjs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ufkcqakf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hhlljvqd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2prrifdki.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2texiuwei.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qvwhkrqg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2susmirbm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tnekoshc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2cyewzhtu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2utsuzccf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xdwgarwt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bhvisapo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hayztewy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2oamvjeua.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bpljpzix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ruadpprq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mwnrhkls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2bmytgegs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xsiagfin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2qizwwbrg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mendgzxz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jekbfqlo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2pggfvfjw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2subptzgh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zmsvglcx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ufamhwua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmybnpxd.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2spawnkhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfvcgoxv.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjlkjjxn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gztfdvbs.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wdvsqocp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hhedrxvh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wmzkycoh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fsjieirl.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2iffsotdo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ykfzwyyn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2zsdwrftv.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xjaponim.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bbuossmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2qvzcktzp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2czdaexhn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xndggdwj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dpuioikp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2srievfxz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2vhagbygs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2aomghver.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2agrbinpv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ktbefylh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2tghzryfp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lepbytyj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2rmiqavaf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jwdvayai.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2smdvgvoy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nzvghqgl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tqtwcyyc.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2aspisoeu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2lvzlcerl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2tcmvgkta.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xoozqycq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ohxrfysg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2blelgdiu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2lslrpocd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mcrydlwz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2qsxvtmes.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dmgpcdzq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2zouaiqcp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2flmjpnfv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ordwxsse.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ihelgxhm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uwkjpvxu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jbjkwgbm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kwmvpkqk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zegzyfhp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2srcqfjfc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qfvsuudu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2xzdfwnbh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dfmaptkh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yjhkgyme.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ywsttrdi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zsufjieu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2jakdwnww.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cdvrpqze.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qlmzmhqi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kfmnnmbp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2bkhfsygr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pcqvpphd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xhckjkng.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2oyoxerxu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ihhpemcc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rvwefdvc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2esjhdaoq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tdlqylnx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2dkagibyd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bvmdradj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yhfnjcwv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oktudexm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2mpcgajjp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wbpkdlkf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ewdqtgqj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qfufoaiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zwqqdtud.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2szalfcxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzdqtyuf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2nbmerasd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dhaarlsk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pjyfhmyl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2baebzdsk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2mvexqoxq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rulyatht.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vihdbasv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uhjrzbss.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2molalmtf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fodcmxqv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ksvzjkgu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uxlksbec.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2glnqppta.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2euzfxtyf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iynmeolm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jpnsxcxq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2poiqyhnw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2chzzihha.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ghdvesdt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2eaileyrg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2tqaroptd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahfxbyig.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oyfdnghn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2malhqauv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vdhcrgzh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nrtuwtte.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xhmifuyz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2shevfjgs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2sxcgzkwr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rxddnmxw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rmjenzfz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ilktvqdx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2dkkvoilw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qkawfdes.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jycejhyj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2terajway.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2jozqtojy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nobeanfq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2audceusc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhikksng.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dzjpozyn.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vtxuksea.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2riudurrb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohhsrvni.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rjplbccy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2luetilmp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2pldgpbll.html


<!-- 参考信息 -->