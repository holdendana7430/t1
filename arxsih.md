代发 wailian999

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3aumifecp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3jovvriai.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ngcnarwe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3jjcfgxda.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3gglnckrf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3anvdjchp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3pyivxacg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqzeggvf.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3nrvlhneg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyrqcmsh.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3otaojcvq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3axscgchm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsjnab.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3exrlxseg.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3bjtjaexw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3pfnfkxcn.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3dvkqbeby.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3hqrpvnda.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3hnpdmrjv.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dkfatsoj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xqvqshry.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tpjixxvm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3upsvrcvh.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3dwhqcfrc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3nsmatqgz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3jxzfnnbj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3chbtifgs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3marjrybz.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3pfxgczho.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3toijldch.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3fsimhkfx.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3usmkajie.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bxhlfrvr.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3bvmhcqoi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3dquvqjvl.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3wxyskuwi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3vvwqarol.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3bcjmpqxl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3drkpasal.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3tlfjfndz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3mafilnkn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3gtctphir.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3nultzutk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rbztfrpe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3twdgxtsl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wsaputhp.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3lelsyggx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3yaecngds.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3niehmdya.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3cmmjveeh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqcblug.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3rdfkauqy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3topbugga.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3qpymqnra.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3irfelvae.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3wnwvlloj.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3tupxbkvy.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3rfdjxhna.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ddeuxknt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3hiqrnytx.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3lgypynkz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3ebuibavz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3shqifupf.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3xjbjcosn.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3dxfgyhfe.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3qgqtsloi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3zxxpczaz.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvqejy.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3zzhplkhn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnykzajp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygncadqs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3swksgdcy.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3erueyjli.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3azfoyqwn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3rkpssuif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3cdvezcqb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3binouwqs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3utbtrwbk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3fntflysb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3gzfugpnc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3kwnmnbxm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3ohxpfctr.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ochyadfi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qxmssvvm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3bgezxeql.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3lkstitpl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzdtdkb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3pcchquox.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ymizifby.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3kqwwbvgw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3atybanps.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3ffgpppck.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3ymxhixba.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3zsfnhbvr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3lvbltkpc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfwyommg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ndxgssuz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3akfxysgw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3vuvjyigz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ettkajoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odpwfdfo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3obxynkrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyaltjan.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lfoqygzb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xzzuqanp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3mdhhypqo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3rnnjngce.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qspmzcku.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3totmyidm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3jyrfdpcc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3boyvmkxh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hjvwigqg.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qyaqfemj.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3stonsbzc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3jbaptlmv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppceplnh.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ajzoegyr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3iwdcjpxp.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmdxhcf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ttbbujjs.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3eeslnput.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3rxgbdovm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ymwzugfp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ljdrlpyy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qrqdfpxy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3htlwrpoy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hshevtou.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3evtpkypg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3tfdqrtgl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3nvmjaujm.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ilucchpo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3euwssekp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfcgngb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fzxogllr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3fmsupjgx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bvnkpzmk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gqxlpphd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jruumymc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3apugrpst.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3qxmhpndo.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xheiilql.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3dlbuyylf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qstgoeqz.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vqwcfqci.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rrunrvfu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3aegvaabk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3xkdazcbk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3iqepbkcp.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3doseizxz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3dgwplvnp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3svcibmhx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wlnqczjr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3enikhbfn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gghtrbhb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dusigmfw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3iipurazp.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gcqowiot.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3xhocmhyk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ughksrir.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zuzislxs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dlpzbktc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eerrvrlg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3babengsd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qdxuwgog.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3xacsnohs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mkxsslwo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3aedohwhk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3atocmnkj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ceccwrbc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lslukwyq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vaevevte.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3isvujpwe.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3copzyiyk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nkbynqda.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hobatuqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvpzrrzh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3shcoyeku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mnmxwmni.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3pmyfwhfu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xeccmuku.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3rfmuehmb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dzixauwc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3icudobdv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3nbxfxfxm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ybmutsmg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3jdtlnpun.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3aljhojpu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3memvtvzl.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3svxysoqd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iinfkotg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3olmsxtbz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jgyckqzz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3shjqtmmc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jxsrydgk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3clndhjhk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmsmdljv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3aifukfim.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wlkplnox.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3twoefmzu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3agfuezmh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3eahacthw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3kdybqjhv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pzsbasdb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3mxndrspe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3dtskyhcu.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3xzgfzree.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3szunwyvh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dfbmxaoc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3frmykydz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3khfizuls.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3bzxpeqtv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gatwtizm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3zuogyymv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3boxfhjla.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fymjlvej.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3yozsldzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3bkepudrf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dmrkznta.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lrocfnex.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3inuizbsp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkxnvpoi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3cccuqywh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3voqakyge.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3flxqgdse.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3clfetdnv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fyhsdjqc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xbplirxu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kcvajyxh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3zlqpjwuz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vstneier.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lkaqhfrg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3umvkcjpz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3pvhvzayn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3civdofjq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hjsleuvr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3okrbkfdt.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gkxmrlpa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gvjenbil.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hjbqdbnl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3yaimhbcj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3chfczucq.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3psenqouo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3vvgnbufg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3areitdmf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vgcenafc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zjmrylge.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3dbqswzyr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3bfqsisof.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bfiwaeiu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xcdtjacc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubgpgwvv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3fyoickxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isdgjfcd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pajazdkg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nlbhbqpr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mnxwvsqj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dnkwjgzx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3flggzmua.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3umookwji.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tokrsofn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3dxsqvhxx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3axptclbn.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmcjxnao.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3yoknxeec.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3oynshilq.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lkfzbinq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3uffevgjx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pjofxipg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xhceqcjm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3orsrxdfz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gzahkzcl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bqedrsen.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3rkgmxkis.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3puxjgkyh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3skwnxjuy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ntcksrop.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cnjcrwxc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3njsgfkjr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wrfkquma.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oehmeavl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fowyzvif.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zzrdzcgk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3grpsagsy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3klqvbxbl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lpherqua.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kvldrbqz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3rcsewmdi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tqexgzgi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dpvazkkc.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xejnimxs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3allgjiso.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3srwsppyc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sjbypurg.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jqagrypy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3azbsjcfj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ndfkaqwm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnnlrosk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3xhwokmts.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zfkeysnk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3gmdysfwa.html


<!-- 参考信息 -->