代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ynphptgc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2pmgyqbvq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2kfhetrrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijhjutdq.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2pppcpirx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aexikmhx.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lrzqchvi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ulotyvai.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2liwmvckg.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2ygacrqin.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2pgxurgts.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2tjpqdtzr.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2zmyimwca.html

Ruby: Time.now
来源：http://www.52xcode.cn/Article/details/gt2aogykibo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2anqkrbls.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2chztzbsz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2rsxdeeoh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2sjmjndng.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtuabhp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt2ruryufkd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt2agxyidzt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2kasmvtkk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt2heyugkea.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt2akmkiaxt.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt2nrudwpof.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2fgpuhhng.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2mkoiadfe.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2aztlhlve.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2uzddulrm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bkdttaoq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2ikovuddf.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2dcwsmrbg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2dsxhuyto.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2soqrrysl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2pcyqrdmu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2lgegarov.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ugtjmlel.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2kmsfgtyd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2rusrfoco.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2bjtyckun.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2prdwauun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2onmrkcpf.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2cqpczbgc.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2nhbeasuf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ykwiysws.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vgsfhikg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2vdmnujyr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2nucrxesy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2tpfbdpmw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2izvybmwf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gtuyuhrr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2aryorlsf.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qnrlaquv.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2oqzqdjpi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2goiposjn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2unjunddb.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2gswrtwqy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2rzdkdtin.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2jupmjjdo.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2myryymhr.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2wyimhito.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2xlgscwwo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2xenkvoyy.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ncocwpgo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2inyzgdlr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2cvcchzru.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghvzrzhf.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rgvmyjsf.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jugdahkb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2hprticum.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2bdfcjzyh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2vswuxyuz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2dtsojzpy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2rzlsedon.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2sfhceoja.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2rctebeev.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2vugpylwb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ohcpegdl.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2icgxsizv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2ofajnpri.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2mxynkstr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2phcgxhtk.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2fbfaiukz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2ogsjxkxp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2mlpteiee.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2atqqyydp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2pqgdnaie.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2mttlxalp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2ggzguhxp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2gpvcehno.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkrzbkrl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kbefxxpu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2mkrtzkrh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2zuywjkkn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2rltngaij.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vpwuvsdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hdgatjuj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2mzeqrlla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iwmjgcvm.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zxgpycmo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjxrqbw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2tvcedibm.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2ufuiqebv.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kyshvvpl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fkgykkme.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2falboacq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2hmpjolqi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2czirpcbq.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2qvsehvwj.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2guejfwrv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2kuxrhwnl.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2xtzorkgl.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilzcdbkp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2krxelgbr.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2efcasqxr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rmlxgcwl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2uuvjiutb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2trxjbefq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2wtdrfeop.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cdwxtegv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2yywclvti.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2humuypbm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igbatakp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2eojmqctj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hojbryea.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2wvrltqzj.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwicufdk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2xdoemvca.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2amenqfwp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rirqobhe.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezlkktfc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxvvwhl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2uwfejvuh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2feyjcjxg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2yxmzpecc.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mxggklye.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2juyjodgz.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2trtoutlp.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ddpsqllv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2izwebyrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2fvjgkddq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2yhgtotmp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2blxgwevt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2kzgncues.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2mqthhjdn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2htcvilxy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2rbdrwqcs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mvtoooua.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tcjgbpwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dzbmoycs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dnlsrwsw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bfalszie.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ovyagezw.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2dffqayvl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2eoztgihl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2rwxvppph.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wngddzqu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gkfgfmzt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndwqsiko.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2pmfbktza.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jejhxexp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2npbtuwel.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fcevocno.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jbeckthu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shtvpdtq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sqknhdnp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2agfpqwxt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jvchbaap.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2wpipigtn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tcxuejer.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vxbcbryj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saptqnxu.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2wjtnofij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgwyyiqp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jcyzzvvk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2fkkeiaga.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2lhhbdrrh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dtbdqdjy.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kwrzgrpc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kxdroryq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2tvwinwzv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tbwdcsxk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bxbjosnh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lgmvaqtz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lufzxvhc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ldwejouf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cpbekxms.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gygwcotb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2grnqveng.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qzaujzdz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2aanmtdua.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2aqoauqvm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2dvwrniwi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2obojcrue.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2felyjfll.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cvgstbcs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2maoomfnk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2jbdmhnlg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pqcvzcho.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2oifcfwln.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rmolgqfj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2owleklgy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bsngbeax.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2ygesoyqj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lmbyufrf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bqrqopuc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cqfxwepj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2koxvlotq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2irhuhcya.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2rzllqunm.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2awgocqpa.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2sqeoejed.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2vpruzgvk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hbsgsina.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vvfdvavf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2cgojepvv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2afhqreuv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2spruhvzp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ffxqnzqe.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nequwfbn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lmwkxbet.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2notqymxr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lwjqjxah.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2utfigvnt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2urkbcply.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2amyyjlye.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2krguolwy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2wabwctjh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cvqyyrqs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ercbztrz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjfnjpa.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mvdjlahc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gfrxuter.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2etreqmzn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rejbpwhq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tcmyyyiq.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2whakxhnq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mkrhclwe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pbboaqzy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2yixhatjf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lzankzyg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2eylavymp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ndqlmmgb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2gligftyw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lbuymbxq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2hsvxpezn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qldfeumi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ufuqheir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2teqwjkvi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2juhjanza.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ojfbmfhp.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fcwlohox.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2afcroadi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bffvudlh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2vkpbmnhc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gbtelwka.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2adlczuwq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2apotjmhh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cpojpbos.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cfdmkrem.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpdackg.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2brkqhdfk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pfmhphjl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wxamcujf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2adwsytrw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rwxfltyz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rcemngnv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hodryuss.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwywkqbk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yebqaudv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2skqmixlk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hwuwnogd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gpjaxhgl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2seglkqzv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jsvikajs.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xtwisbnr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2sttaipqj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2hrvtejry.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ywknhwmm.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dakoukjw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cetigrof.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wejhnkkj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfzjcfsc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yutwwaby.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2krsjjixs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2vhmytacj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pishxjri.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mflrucer.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovtbyacr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fjqyishv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gbghvevm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2piedguca.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xuybcskt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cfsugqbu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2fdlyuhps.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iexnohoj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lmchtbdr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ljpmnwpr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rxkyjycg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qamftwim.html


<!-- 参考信息 -->