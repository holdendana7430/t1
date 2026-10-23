代发 wailian999

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt3seuazchc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qxewxamj.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3qzzoxfis.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3mnnulsiz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3ngulqyiz.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3wcljcmiu.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3uyhsbipm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3cfwdwhip.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt3pekvtsbb.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3loidwhyb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt3qqekmfij.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xtbcizdu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3csbmwvwo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3tejeayxu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3domcisfp.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3tfbxcigj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3ejqhewne.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3gbbhqwye.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3filuohqo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3dzcnskyw.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3wwxpdvsp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3rksiiurj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3yashayxa.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lswdhdaq.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3pkhyeewv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3kzabndwz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3ydvijnnx.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3zhgekecl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3mkavrozs.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ldhyjjla.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3rdybzpbm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3dbempjhp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3uaxwxibh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3jiqnybxw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ornlfgus.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3fsumskxs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3gbooulxe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3pqilfavl.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3fudyaubx.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3zrmzfjrn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3oefjpnnf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nywzqmew.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3tsckbxgt.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3otcmepox.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3ssvjuerm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vkpnfpdo.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jaziwosf.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3jtfptiqs.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3xtjqilgv.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3vptvzsaj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3espdaezv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rkxtaicc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3eiuymmmv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxgpiks.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3wpjqzjax.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3bmplgpri.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3smqrzzyh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ahfwzlqe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jphsrpzu.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3arzbtvxu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3uyfjvdwc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbymqcm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3zpwwjgvz.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3bbatwjwi.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3aagotxdd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3xgojjugy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3qquwtakr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3jjscywjw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3lqqqvlnu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3tlhmxpgu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3tqpvqcld.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3ilaovhsy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qsqjewye.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3xmkmdoie.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3uxdbgbre.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3mcogpylq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3niuoagaw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tqlkpdpm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3arwxoujb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3drrpnjzn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3nbpcrbyc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3epchtggk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3fyyedhhi.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jytpjxma.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ehyjjjkb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3bazwlvqe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ceojchrw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lfdmckmq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3wjjmaifz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3cbaivhch.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ttpzbbwq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3uniifdnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foufaxkg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3paqeowxv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzbryywi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qvavysih.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3eklkyjvy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3agxuutxm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqvtvjyu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hwpumzjf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jualcaps.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3xinqkyuj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3jcwcctbv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3luboxwde.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3bqztcsem.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzuprznz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3yuygszwf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ihpqebbi.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcbtujuz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3oqsiqvhj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3azcmwvyf.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ktrzccna.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3dnyfhjtp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3fovtapjr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3gjqvbpea.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3beiifmcc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3rayfeonp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3mmgakutq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjhrhvm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3daxrutqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hoblnkdr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3gluixrbw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nawbxcej.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3deegnfkg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3hrqjgskf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qrvqndeu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bjjtbyzx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lntczmjh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3idfrmoqf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3gtnkkafb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3vyrrdskj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3wtziyxmu.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zhqnvxjl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3srtxjfeo.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3zlqqtvvv.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kydvlmbk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ovyfmuwc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3oluknyxd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3spjaqdlx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3eiippkwm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ldnopikg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tyxwxpbv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3odshykgr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mrwyngtc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rbjppcts.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mhclqsmf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ipnoseqj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ujmylufo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mvryuhuv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcdeceie.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wftezryy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3whqsraqi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uxywwazp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fazztejh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rwbvefkc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ledpzlxa.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ilpknwsp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qyaxrzhs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3otibgfjr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxcxynmo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3dvrbgiwx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yrhwhalm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ofhinmdp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3jutampmv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3gfkpxxll.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gzjmswry.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3lnzhdkze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nuqyxfzh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ulcmlsqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjxoqnfc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ltyffkql.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3glyoeyic.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3rgfnphnb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3krjzfuru.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3cpgelvzh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oimcbhpi.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3apnywkgq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3cjpostoh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3icsrkthe.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nfheltbi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3omlqjfgl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3iqebqevp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3qljxdndr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ivuperds.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3krnekyed.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3noyrlfnh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3nlavdtpa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tztzlxql.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3aytnxakq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3czvohmuu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3hgvqkjqx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xzunkuxh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nsbsqcfy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sbqkirqt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nvurylwy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3naaclgwa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ysjilhdl.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3brjpvavx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3dilswpoz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dchvigeb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3weawugiv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qhdismvb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ldbiujje.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ffcdhhpu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3zkorjlef.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gnwoidfh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gesnmwvm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tthzxpmk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wgkxtjtb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zsmbvvde.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gvktidqp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3hnxwwwzj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3scnwuyam.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3iswhrkdg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijuccadx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nqfnblsd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dcrglaao.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3duvztzeh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3flddplrj.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3gtcbsgaa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pqvhcrvv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uieaqkvb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3clsfvdnx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nnibpgvc.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ozaexmaf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3drcnfcqz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3gvuljvfb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3yhodhwpj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3noeghzbg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mbtelnxx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3brepyvsr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3coopbdxv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lifdfqjx.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lxcldhrx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kbxlpxac.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hzdpmprp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ysagsttz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vgpoaieo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rlhejkcq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3bhmcsjrk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kbcqudsl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ivrlrnco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxakevhc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dtropjtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtvjpwaw.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hguylesk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3nyqkputu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qfajdpqr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wddplkbg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3irorarts.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3wagqktuz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3aktlvfdm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ihwhuadj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hjgmjjxa.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yvjybzaz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iulzfnxd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tjnybnbw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hgydbycv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bcqlzksk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsldljk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jrhlwary.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3mvraklau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jtsiuypq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3oktydicd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3itcjztvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3cydlfcgi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3bdfqawtu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3sfambwih.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kovgatqd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fmorhzey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qvqmgalw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ntknwuoz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jaaxzpvw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ebawvgla.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hcybcdnx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dedawkns.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qgqdshcw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ysbiigpt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bhszvtme.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nbqmhsdt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jyhfxtmq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fwutfyxq.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uirdghwf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kdzohlid.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vxyemeet.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tdjdmnby.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ausnxlhl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ahqdfbmy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ftthfpko.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lmeegnwr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ryjkfdhh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mikmjbcn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3wyqwdxop.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vhznfmng.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3naybgeri.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ewhamdqm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3vsfphcaz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3xyypemwu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3mdkkbspd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3itotpxkj.html


<!-- 参考信息 -->