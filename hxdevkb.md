代发 wailian999

J. 日期与时间
来源：http://wap.zdbjq.cn/Article/details/gzmsgejja.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goxvqaufr.sHtML

[J01] 获取当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gpjigynof.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gixiuflwe.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gbpurpkjo.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gdwvidumq.sHtML

TS:   new Date();  Date.now()
来源：http://3g.fehbvm.com/Article/details/gmftvqlts.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gwjepcxuw.sHtML

Go:   time.Now()
来源：http://www.m.share.fehbvm.com/Article/details/gjdlopinz.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gzkfgpfew.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gghwjqozf.sHtML

[J02] 格式化输出
来源：http://blog.hesvh.cn/Article/details/gsxywqhyy.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gkaeqxgeu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gxrlrkfoz.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/glozpdzib.sHtML

TS:   d.toISOString()
来源：http://blog.fehbvm.com/Article/details/grvawlqdj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gnwcrxaqo.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/gomboodtr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gcjzxmrze.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gkxpgiyim.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/grlegrvrc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.hesvh.cn/Article/details/gfyahuhog.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.hesvh.cn/Article/details/giculuccb.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gxppafqxa.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gcfbnmpwh.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gswicskvd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/getsqirkq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gipuypfjs.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.fehbvm.com/Article/details/gatsozyxg.sHtML

[J04] 时间戳与日期互转
来源：http://wap.hesvh.cn/Article/details/ghyezgbjf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gotjhjdzr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gmeebhlfq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gowkaaryv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.zdbjq.cn/Article/details/gxxwkejkz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gzvdrizqo.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gfexchrmb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gxswnnfji.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gosgshbzk.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gdklsnovm.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.hesvh.cn/Article/details/gibfabpgr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gpmpvqvzz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/greeateaf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.zdbjq.cn/Article/details/gjycmhmfb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmwgubgmn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/gfgozwjre.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gtrcfxlyj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gfqfosadh.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gklghbjfu.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.fehbvm.com/Article/details/ghclkyahm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/ggzvmqnxu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gglfjceng.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gsyfgkbme.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/geanvyvbt.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gzahxdbyb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/geodeglou.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/gbqlclonk.sHtML

[J07] 比较两个日期
来源：http://www.share.fehbvm.com/Article/details/gyxglwhoj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gbnlhclxz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gqahtuzuy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gimuxjnab.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gipznwfho.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gimiwixwq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gqwgypihd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gctofipbp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/ghpxulxxc.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gtidsatkn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/grkblswlk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gltygcxcg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/ghxdarzyy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gxkutmdtf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gbbwznbsp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.hesvh.cn/Article/details/ggnpnikrd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/ghgepqeqr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/gdzmlvrlf.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gjtglvojg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gevsiwfie.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gfpertwst.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/godbjwawd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gkmmeymjt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gwzewobbp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gyppuxpar.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gnifoqzry.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gkajelopk.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gkncbhzgp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gtkywndve.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.hesvh.cn/Article/details/gdxmohrfw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gekvbpwjq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gafhrtjhv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/grziixlse.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gamgiyhji.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gsycspiwm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gtykqabqk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gorewfvmo.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gjrgsfyzv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggriqptvf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gjpkjqbfo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gvlfptczx.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gkalmbctf.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gvnzatvou.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/govfuhheo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gfzhcwfhn.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/glnikolyy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gzyheozus.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gewuoqbdu.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gqirpfyev.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gzaponbfe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gehwwzpwn.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gzoixpzrl.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gnagkbcgq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gtrxpawej.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gxxpsbuqv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gtmewztvs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gvjilqbpn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gwmxkxnso.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gffppsdel.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gwtcqswsh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gixuflyoc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvhuzbk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gyutezyvc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/ghmkywhrg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gmmpezrfi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gizqtgqbv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gljretmyh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gvppftsxy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gescgippm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gigpfaghx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gbwdqgoxc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gpzrhdsbd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gwcmfnflr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gzqlvwdpq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gxrbokqdu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjauhmesb.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gbwbvzhpl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gjkhahgfk.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvcdvsrxs.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsdjezqld.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gzfrjtpwg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gxkmdhmnu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gmtammhvt.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/ggrunifls.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gfirfkrzi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gkeahukqr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/govhdxxpt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkizqzobe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gbjboblja.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvppxee.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwynyhwpt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gzknnwvqo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gnqmrtjig.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gpnuokvlb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gbyumavwp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gdumuwdii.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gtmijavez.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gaqaiczos.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/ggbiwjtit.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/goilnhbrj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gtrcpyqpx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gkhxgprsb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/grofnocqu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvuzpaxqs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gruorxvxv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gmaaqhvyg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gznddmbiw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gjapyzdum.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gbkrqwaar.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/grqnltngx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gvpmiqihk.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glsflcbvv.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gmieblcra.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gioehthep.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gbctbngxe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gxyjquvtb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gcpnufxpj.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gbavrlymo.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/grtwthfkk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gyusvrjqn.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/ghhvnmazn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gipvibqxl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gjstjdeoo.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/gqvcrzngc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gaygdcvbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gfejdebav.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gvvjzyunu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gfwksspjd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gnlkvvhjn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/goevmtuee.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/geuxtjtxo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gbnzpgczz.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gzzdmzkok.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/guikinzbv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwrckcgjq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gijpwtynv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/grwphkamg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gckqayxjk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gvknxovvi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/greidricm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/garybamor.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gbyoqpghm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gqrszzjoe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/ghtfoofem.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gxxbzmpdr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/ghazxxous.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/goequmhye.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/ghzmlguzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/glwlediyz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gvkdcxqqh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gnohofreb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/guepqclvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gzslygwlr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gppcenuig.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmvdwkemx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/genhqttyo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gogjzylkb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gkrsgxojk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqhqncvnz.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gihutjjwn.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gygdimoou.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gdguyeczo.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gnldvdhkp.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gklzoecrx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/goioueoee.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gbmlbycbf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gthdbfgap.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gkhhcvxdr.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gbrtxcemy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gehvvxcxf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gapwmyhyq.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gltgsujvh.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gunpwvakf.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/ghjosssvm.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gxlecfejn.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gygzvsbrh.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gdgfpweqo.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gyeomlazq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gmigevizx.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gqjfxcgda.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gpzlepqdz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grqkzxkur.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gbaphrnte.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gzqmcwywx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gtarwfoiq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gorvckrfu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggiyxnbvr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/getkayfla.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdvwdygeu.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gkujingbo.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gaszrwvfp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gdhgfkapu.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gipbynbyb.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gsqlmllzt.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gmqwhuhkt.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gqnlrewqw.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/ghbpjjngv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gmiobbrls.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgqzwti.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gxdbgpucz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/grtlujnbw.sHtML

JS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxvgunqtk.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gmrjxorwy.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/glqgbdrhk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gkhkxphbt.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gvyufspnc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkufcwvbt.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/goqrxgxkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gklhmalqz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gutedywyi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/geesynbwa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gagdeiboo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gpugihlmg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gyheosyrh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gnlysdvci.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gzyforchb.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/garmbxorq.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gqvrolsdn.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gthxykfhg.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/grzsnmjlk.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gmpfoocqq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/glnfktzar.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gkfsektuy.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gizqfzsaf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gdvkvlnac.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gobrycrvi.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmhlhnhwm.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gfdvlafwv.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzruwnafs.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gujwhtiev.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gbmpegpwm.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/glwqrutwh.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gwoxkanmj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gvfgvxqnu.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gmwifitpe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/glyloqalr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gduydndkp.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gtxgvahii.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gxfrorxsc.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gzxmwsmew.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/goabrunfr.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gbesapilm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gparjbbot.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gzkjjgrxt.sHtML


<!-- 参考信息 -->