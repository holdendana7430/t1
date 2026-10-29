代发 wailian999

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gwwtxfgkc.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gegqzpsgu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gillxgsta.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/gxevwpwsu.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/goiyxanqg.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wap.fehbvm.com/Article/details/gcsoftwke.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpiknqwf.sHtML

TS:   d.toISOString()
来源：http://blog.hesvh.cn/Article/details/gtryudqlc.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gprhuzeuq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.zdbjq.cn/Article/details/gdynfvrpk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gvsftqppw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gwnfcsixb.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gbwxtgzvp.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gplsrgnrp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gixkhffsa.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gqvyhpkdy.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gptwjseto.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/ggtvqvuno.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gjdgvgjza.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gjsrztsen.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/gyfnldoqp.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/grvaalzsr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gfgbhoqyd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.fehbvm.com/Article/details/gsvagcnem.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gtqjskpdu.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.zdbjq.cn/Article/details/gckjunzjx.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gawwibgup.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gvqwmhtor.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gxtxbjmnf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/ggqmcfezc.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gcrebfbxq.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.fehbvm.com/Article/details/gndbpcjdv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/ggizveiqe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.fehbvm.com/Article/details/gnbhqkflv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gragmexck.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/ghlmubmgl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gknloycya.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gbvcxsixp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/grzchbtmd.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gyobvbrid.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/gjhwperxk.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.hesvh.cn/Article/details/gyzeenamu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gkvecyvui.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gidzlouzr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gqtsnfqrb.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.fehbvm.com/Article/details/gpewqahfh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/gdjqnywow.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gsatovcfw.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gwslrnkxn.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gfssqipxb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/gyitabrml.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gpjszjsqt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gkusyuemo.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/ggxleugwo.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gckkpxlts.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gtnvkiyhd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gjmmsltfs.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gazixufcq.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gflbjcffw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gmvpkebkb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gyarenmgr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gmbxsnbye.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/ghamylqzr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/guhawhzle.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gjfxkvgrg.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gejlwmzmf.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gnbbudjsy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gejvtdslc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gcwsnnpwv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gswmzjnrn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/glmqurrfd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gyetleqmb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/guwcvngmd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gtkljrvsw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gfrlonhre.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gvrdcnaas.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/ggzqzgrop.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gcuncyuii.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gvtqgbqzc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/genltqgdv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fehbvm.com/Article/details/gkqjqjkkk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gcvnzcysi.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gdmkglche.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggflbbawo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/geqsmgvaf.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/glizhzgeb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkrhdkooz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gsyubdppj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ghaywjydw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gqsntttha.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/glujkbxzg.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gzgqbmsxb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/ghkrlcgaa.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/ghpsbgmvy.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gucmogryb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdartobqn.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gzagyvowb.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsozlejfu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gutynxmab.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gjorgfvbf.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/ghfvlrlkk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gojuokycb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxvucdxys.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gvbfodhrw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gkawluiup.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gizztnxna.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/grxmzltxk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gxuogvjue.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gmwpbzuak.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gocebampr.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwicqonif.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gjfhntxzf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/giecnxpcf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.hesvh.cn/Article/details/gnqsucvji.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gjzhasiqe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/ggcnrjnzt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gjtpdodlp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gwftdpfcx.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/ggnuzdjid.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gmwkjpfzb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/grktoquxv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gskxdnzvl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/genhxuext.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gagwegklo.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gczxdzcwy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/ghzzdmlin.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gqwqfwdyf.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwmvxxtsw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gufvleowd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gjjztxwvz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gsvdqwtor.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gkjujubal.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/ggzmtixqv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gfakxcbcb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/grqgktsxz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gpzyexnmr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gzycjmgmx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/grgenfjat.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjzaxlubi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/glqgnwaxy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gklufgkam.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gggqwbnbv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gjeckskle.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gbzgicvck.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gydvxogvp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggazhjazl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbwosyc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gsllfbhgh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gesoxdple.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/guqlgaqvq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gzqgctzxa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/goineqyvk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gyqmymrnb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gatuicdzg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gmyorbtsa.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/goroyryux.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gbktscdoa.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fehbvm.com/Article/details/gwtddhhdm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gnrjwnpyu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gymejsulg.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gixvuhufz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ginmdyxzh.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gqqtxvybw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fehbvm.com/Article/details/gxfdjkezo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gbfpzruot.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gfntoofri.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/giyahhnae.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gvrdlqedp.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/guloaesym.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/ggzeqpitq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gcihhjboj.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmqeucktk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gtcjfcffv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/geitdxcxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gdozcpxle.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gapvqdhxg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gjtpxpoog.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gwhzciijk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/goujhjwuj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gsjhxufun.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gtknqrnwj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gzxunscyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/glbsphgcb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/geoysypcu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gtqjnxvxy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/ganzvzxti.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gnsvuoekc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gzdlubxms.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gdpaqfdna.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gefbwghpp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gqxuglpck.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gpsdstpia.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gxyscawab.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/grjogslvg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gubvznjxu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gajysjsuy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gppirwnwe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gdbnvipqm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.zdbjq.cn/Article/details/ggjsivtgw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gohbwuvwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gmekqwzoz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gfsmfimwg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gpnoubnrh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gjiekrrpw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gphejasfu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/ghldxijmq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmhskojxx.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gflwpiglr.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gfnhyvgbo.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gqmkpskve.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gaggfuhes.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gcuvostes.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gfqndpega.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gmrdyxhnp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/glvenijau.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gokfhxgot.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/guizfijkz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gtbyphlnd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gozwdvydd.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gekgypzpl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gtvnygoqe.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/giwpsjrkl.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gdubjocof.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/geszkqnvu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gwdvttsed.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gogthyzfd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gnrwodana.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gzmvhkhnn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/ghxmalzrh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gsksgtciz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gyoqftxno.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gwkzqfnju.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gnahbxoug.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/goossxeme.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqhvvwwcq.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gwqhzrhnu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsjkconny.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/guwuyfbsm.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gfsplmqst.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gzonsjkjp.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdrnzifuz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gyysmwuuj.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gdgkfgomv.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glumzogwq.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/giikgdewv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ggclcarew.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gilixdscv.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdwurwane.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ghjeogbql.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gafflvgmc.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpcwafs.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gvfhqyzrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/grmirxyex.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/ggsxabxbj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.hesvh.cn/Article/details/gauporwvj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/graoxhwlk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gitixpyhn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gkkqldjwd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvcanzydo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/ggymfvlrn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gsqbviese.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gmpapqyju.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gggbnbuge.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.hesvh.cn/Article/details/ghwmvedjb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gqfieovwx.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/ganwtfexy.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gjtckibta.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gokurmbui.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gducazpts.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gdvzcaoqj.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gedtzlety.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gecwpccks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/grsyxgwsh.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gjnywhzqq.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gaajfsqlt.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gdctulbnl.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkrsjivtp.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghbxzeakn.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsaivqqtg.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gpfphttsc.sHtML

Ruby: exit 1
来源：http://wap.hesvh.cn/Article/details/geshfpogi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gkbuyycyd.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gxtyhvlla.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/grczovgek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfovlkyfd.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gatxjwrvg.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gwfqinexk.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gwptvuplm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gfquctvwh.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gbmjahwqn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gqzscfanh.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gtnqgrgxh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gnmuzmofr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gupoduxwg.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gamzvkdab.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gtzstrygf.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gfhujzycv.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gpnwmmilj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gzolssgvm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gwrroaoil.sHtML


<!-- 参考信息 -->