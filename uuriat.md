代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3qikpeovw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tehermib.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3sfrmizjk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3ijgaachq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3bfchamaj.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3faxlzycg.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3rzxnvfsm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt3ogfaxqcd.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3cobomilv.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3blbpykgf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3dnuhvdra.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ijoyuepy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3nolidvur.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3xyarhpqn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3zvfffibl.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3zqusmfck.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3ulornmms.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3omdxkzrd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3gdryhqul.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3wczomgsq.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3jxkqqnkn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3kxdqdnri.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3sdimeicc.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3umldrord.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3vunefsjb.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3dqwrkegq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ijhjbrni.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3mhwpqdul.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ngrzcfqk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3xeapnnuy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3pqpraeyo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3hprmqydo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3cwvxtkyk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3nbdcdlts.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gdyqdncy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdighxfs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvvtush.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cdfjxkne.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3rbaokrhw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3rsnnvclz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3ckasjkyn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3bwmxckio.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jtaxctor.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3phxiwzuu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3roomtpdi.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3aysxxsqe.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3yvztloje.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3kqdhanmd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3wdnnwykf.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3gnggzkmj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ltcfkupv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3nxiothon.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3vrqyxwaz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3iosobvxe.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3fvhprqkb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3vpxglskd.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3lmanwomt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3cegmdzfu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3szmquqkm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wbgyqhgo.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3epirizee.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3anzjuioy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfocfsv.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3akaebqeg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aeiphuov.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3sdkosmcm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ksgoagss.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ushkieuo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ilqpmfmo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3cnhtzkcl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3hwtxevmn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3wezrckkg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3mpurfqlx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3sjqfowvq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3aevobjnl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hexxuzgt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3rmqucwlt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tmrhvxos.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wznvypwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rvruthbg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3dndxuenu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3vqonzmsh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3piglhpyl.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3rvcrslpa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3caqjelaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3vbgspipk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iosevrfp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3usengjov.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3iuvixfmh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3iaoixfpk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3haxkgvka.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3nzzrffor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzgxrupj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3yvgthbtg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ltrxjccp.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3lokstnsa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3uwrzirlo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xzyakxad.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtorqtmf.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3djisrpvk.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vebjaaof.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3ahjhxxdr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3lqlwflsh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3seaptccp.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3thsoyorw.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vadcoeqr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzwxvcah.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqzoqnt.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3osnuamef.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ppuukbgg.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3novmdtlp.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oshmfhbt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gsbwmxhp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qeldaagc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3njqhpbfy.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3asjbvlee.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsohfavt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3bxshnxkh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3aaouizzz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbppagt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eifkwkai.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ijnoncnu.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzvxziyh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3hfoxzjdy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3peqdofqm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3czkxzyau.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3akycisks.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jyibzcck.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3wvggordq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gstwibnf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3oqognnpd.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3ssuhpcht.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3dffxnhfe.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3iaihvyym.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3opyesffa.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3vbwlbjlt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3cicnjatc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dgnhgvfk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ghyuykrw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dppbanzc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3yqfaahma.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3vtfmvbcd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3xgdigikx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vimaozud.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3luqiofzi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3cjskknvd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3eucdjglg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3hkyvxfiv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjoaytb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3gufecpqy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hviqlhsh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3eecveodo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3finoaeno.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tyjjaifs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3whlldmuv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3tswfmbkf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3plwhpmcp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tbkwkcaa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xfoocyrs.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxzywpm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3pvksgqya.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3pljjtigp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ilfomcal.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3jcwmwesq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nuktibrd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzxwrpl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pksjajgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cljninfg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qjprxkhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uvzixddp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dzvrlbhn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3xjgnmhrb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pkdlfcak.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ssulcujk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3lplekobt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ckawaqob.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ntelilcw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dhqrzbrf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yytvjxmn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uxvdupku.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xrgbhcyz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fposcdpk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ksartlnc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3vwjckxrl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ahensqfz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jlkkdzhj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ycocaitw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3dgaozlmt.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gpddirgf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yqxxepfj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3alvuvcru.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3ykpdqlbz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uqftxcon.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rvbtuisp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kpkweebg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3nmpypckg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wsaqfgew.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bhmketqg.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lfipyjrs.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yosgvlai.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3rfdnssrg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zqqedxor.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kninjucr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tleqqhkw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kgmeszwz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3toclxsiz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ulqjbrdr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3uoxelvbk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3almmjoxl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3sjrrfknc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xkszniss.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zbjhwouu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3afmmyetq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rxvuyemm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tlniqsis.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ndemvkxu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3efvgnpax.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gqshjpea.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3brnnvcpp.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3plxcqief.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ubjbrpzu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3kymyfhrk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3jwhwqgiv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3nifesnkp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nvnelnmg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3iztilnns.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3txwkkbxj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3bysgwynu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sbemiipv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3uqsrkjvg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kjfpmawv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wlcdwxlf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vizkusax.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3onmruxin.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pahwjyll.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qdlvjryi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ihapfsnr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3tgvwwcvy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3tvohmdtr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3igbffglb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3tguohuwj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zjlwnggb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cihtvjyt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3oqwpsave.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnxdrsxh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3qzxzodzw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3swzntzfl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fhbeetfa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewqqnkfz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sngtbccr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3turzyamz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hzuskpqb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mahwkvaa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3pwhxoxvu.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ljxfuxlz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kfdxuacb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3udxvbxte.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3asbcfgfk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3prncqoku.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zanlcajb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vqimmsds.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3satqlbfw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tjstlush.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3mctgsbcs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ixezoonr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zevvcpte.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kkgecbrr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3luognugv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3qeipzokb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3toaejpns.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ipmpkoqe.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3iykbcaef.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gihusfuw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kpsyyeng.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ecoqjxui.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3euzegyox.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ajkolosm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3cxpnbitl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ingrpwtq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3aiprzlqa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3rpsttzlr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gespfexe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdnmlxnu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gouunnqj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qofrtqnk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ewrlzywk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sxtlbzhq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bwudaswc.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmxgqemm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3yvntjody.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3dcfwevxc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ztiobwmm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hcsbcnkg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtefttk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hckhlkke.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qwzmnbzu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3efofirco.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3szklplew.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3trsmuhrl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3shnlozpl.html


<!-- 参考信息 -->