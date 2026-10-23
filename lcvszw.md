代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3bmtgifcq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3sbogtdaq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.52xcode.cn/Article/details/gt3yphdbojn.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt3nmhdrmid.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3fjdiumit.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3hnfcuokg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3awrdswze.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt3iudvyxax.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3ytowckeo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrgjawm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3cznepgpw.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ktvpbmku.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wtnvzrtm.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3syvyjwfh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3aicwxsnj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3sfctwycg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3krlovohi.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3yoqrymqi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3ikjvxaek.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ikijqhnk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfoljrf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3uhrgxhnd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nthkgbvp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aumzmtvj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3wclsbjpu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lusnsvge.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jzrmgdaw.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bjyisebm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3boxngngx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaeuqqf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3geympass.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ifjvdnxm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3koaaryvy.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3kmibzmud.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3xloyleoy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3krdhuvar.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3pqpahula.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3bkzycuuz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3cvobgjdo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3pylonxkc.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3zmnwuqpo.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3xkfmecmv.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3jahdlomo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3ofbgnzgp.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3aqujfjzt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3fepimimw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ilsqrkax.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3cwpylooa.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jgaiylkt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3otcfqjqc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iztjvgwj.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ohlbbnfm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3aqjxpojf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3ehbloxzd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3oylydrgv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3zyzuvbij.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzmhbq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3vqvvtvzh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3jnlgphkb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3rihavgue.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3qljznwgb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3jnpruzvr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3mpomiuiw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3qffkxdic.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3piwnyhwd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mgwsqwjx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3mcemayjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3kqwlekls.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ummhtlxh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3taieibjg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3usmuklmh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3lgdwgswy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3sqisiygm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jmlbgssy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhlsukhu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rbkhfwzx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gyuetpue.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3hwhzwxbv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3rcllzerd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3iiqbaulj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctizmfsm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3rwbjkzas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rnavhxhm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dmbxpdwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzllcnj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zbnzeqfa.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3uvndhstw.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3wlqastkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3jvwgaydy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3mmyapkaz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3cihzietj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3zxkenynu.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3elmntyxb.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vgybpgtc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3jxfrbrbf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ytwfcvbr.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpwbzfm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vahbuuid.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3plccaxea.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3scxyecjp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwpflgxp.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3yctdokja.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gzgtjmci.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3gkveqfeg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3dqwfgfkl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xrbohpoy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjzhuii.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3dpcyxwaj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lofzoepv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3ikhbnhvm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kykyostf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3okawcoou.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ypdtinbo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wdbzvofh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vosbjlns.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3yypdqpny.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jamdnrfi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3tujpuajz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dawdufnu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3nrpdmlrq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qeozrzml.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3fibcsbih.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3xluofist.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qjxsmjhd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3evtiwnur.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3iojdoecc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wbbbmbez.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3tjnubhmk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3daycthvp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rkgbkwmx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3koxxobrs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qumjxhfv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zkfrvyws.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3dgfhmydn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3biwljypo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bdsyvbai.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xfphinpd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3rpfozosl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mzolzytr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3vixlksde.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qccrmwqw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iyhtklpa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vpjdbulg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3fvjrgtku.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jojgkqbp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rmafprms.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3dmulucyu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iafamekl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfadsxsa.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pykpukfu.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3rkckloqb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3voucsoxw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mhntggzx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lesmnmut.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3okskwsxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgtoxyxx.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3vojvyxkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpmycsca.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ojfzknrb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3fxenowap.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3hxogdoub.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkynlsi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vssiddqk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3zalxusdd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3noiqfaqf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yyjtletk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ggkmcsbo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ipcnkrfv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3odbvcjkj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dqwnuhmy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3cxjirqpj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pyridrnq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ehdmvxgs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yynkwfjk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3tjugczil.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3partqekv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3egrkmrpz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ijeztyxq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3zuwdjfpr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vbtmyshc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qilambef.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sppmqexu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ukqyxzhb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wklhbzhf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ghdxxnrj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gcbblbbx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lruxsiyb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gfffphvl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hattjogc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3jlbbhjbe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3alvhgkco.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3tfvmrasf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3sapdlqho.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3nlcanbdm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3feyyphnu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3obmhqemz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wixumulx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rnnlfdge.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mbngwexr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xkwkrbov.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vrydcphk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3qmvneltz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfsmafwb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gqmylrmr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zcqgmwnl.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3arjksdnn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vvkmjuwh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bagachky.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3dhpccyne.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ctgfgond.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3xhxfutaj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3iemeaeis.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vuzzsrmj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cuuvvhpm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3exexfvws.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bynlpttl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ksqwpfqk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3vtiprkdz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qhemkrrk.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dndsajqf.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ubfphbit.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3vgyaoaju.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3sqzuvuun.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3eehfwogm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3rgieuxzh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lescamgl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3algtzwpc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uhhawgtd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3aalwgxgk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3byjkcimw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onoilapv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3rtgymxzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gwbgjxpg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hptyqeoo.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3afddyrsg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pedbmpmj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3shsxudus.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vcggmrri.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hkgoonhz.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mqyjwmlc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3asfsufzn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kysughes.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ntunpzjf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hvkcxkok.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eyoblbxi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ncggzjbg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3xaxmubjg.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3neuqgbot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dfdcmxun.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3dojgsiyz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yyhdnnxq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xgmndxxh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3eavrmoxp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3yfqkhoxi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hygmbqht.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3adklwphh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dlfoesrr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3xdpjgysn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3upgmugul.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ykmdshli.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3slhymcpd.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3dluddncu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3hkwrgqbt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mlwkjjzo.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dhkzwavy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lrrauras.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3trczzbox.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3dqfjxfyh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3frowiywg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hyhdhsdy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptoeccks.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ialsqfph.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vobkomkn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwiydztz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pkilclns.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fyxbhvvq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hrskisqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3wpvwmswp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gzlorlyz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3eauglpas.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eurpxifg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hcvfarau.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3iljpvdfe.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dnajpltw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qeodmwba.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3moiomwvy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jjaderte.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3vuoxnggb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3otmpnfhy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3stvkpscf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qnjtxaub.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rgoeqwdi.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lagucxad.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3hoylreos.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jkzadkdh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rsvuuyup.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jlenejfw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mrhsfwpo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3mizzacbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bjlrilci.html


<!-- 参考信息 -->