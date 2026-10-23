代发 wailian999

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt3jpgseajt.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt3sfufcuzg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt3hmdtzjzb.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rmawqgfh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3oucgcmqs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt3gnyqkwkd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3rkprniky.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3gxwkpwac.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt3qxaaancq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt3vypjjmvs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3osebmegp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3vwlehwez.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt3rlkqsjyi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3bcopaqwb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt3oxmvsfjt.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3tztcokpp.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3rhldqjlj.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3wjynbnrl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3qkrfumht.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3jeaesbyu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3djztofix.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3ukrreajo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3auvmjxbb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ynesgirt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wbfeuhfl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lubxtunl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3utuvsqzr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhqallg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3zwjsnggs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3nftunpxf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3kiufsmgh.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3bhjeimgz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3eqayijqr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3myocxcde.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3petfwwlr.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3hyxrigwn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3npfxfref.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3ufxcedcp.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rpspnazr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3vwozojtq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3fbhqlocb.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3akmcrvow.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3fdihrwdh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3qxmumkgl.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vpkiofqi.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3myqjxgtu.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3akhfphxx.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3crgrfbrt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3hjhgsnuh.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3fstyqsja.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3gjrqvfzi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3tzztzlyu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fasaxiim.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3orknqaeo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3iduvljwo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3unxppewq.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3zqygwshv.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uabtebvl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3nrpbfbso.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3zckjgrvh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3ttwnahmv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ruipliuy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ocgpbzla.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3xkbsgpjl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xztrnxml.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3pcnzpdgq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ufovdikg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3hgpoxxmk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3kirdemuo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3qfjazxjn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtkdtkf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3jlllpwwu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3agdopgbh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3mdvlfwrp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3lyrnchvk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3kelfronb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3zqaomsew.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3biyplyhe.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkxctel.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fqpelnvp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pvoimvub.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3fflyanev.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3ryffltdm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3mhtvnyrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scmjaipg.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3pzwqimog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sflwbkiu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tauxjoes.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kipxsnfv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vwwegpxy.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3gkqpigij.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vamjwfzp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3ghnezgce.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eatfvcpj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3qnybsbct.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3znzjnxhi.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3hrqdopeu.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3vltnmisv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3fvpfesoj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jpdezplk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qqxuxrka.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3sztpzhbi.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3nxkunsac.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjhlwrwe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3qwhljjzg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3cxpsgshs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cfvvehps.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3niutghog.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3tcsaixkd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vbtqenpg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iesnqiza.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3yiwdhqqo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3xzknfwgg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3sjgsngzt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gmbijaay.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3dyakprii.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3fuxymwcp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmmxezyr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3zwdjwspl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vpelffns.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fbymkvih.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xbnwjjbx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cudnjmve.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3nhogzeex.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3whlahcwv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3iihhzzth.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qaczsgok.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zjsrblhy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pjyuuoaq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3kehuhcff.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3eolnlcyx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3yuwlojes.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xftartns.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3olhfjqnw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qlgvamho.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3nnpulmwy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xjgmmxad.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mpsqccse.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xgzsizku.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zuzhmlrr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rsvsogem.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3tviszjwa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ggazjefu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3hjibqobp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hmpkbysi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hidvcpri.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sleyivlj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3klotutlm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mevmwfbi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3beztvvvj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3vvgmepxd.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhcfnmr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ahgmizmp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3juhslnbx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eurtcbcb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qaecggph.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3spqjfsvc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inhybkwb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dpkzzvht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rouyaqch.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3okadiywr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xfcfalpi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3bleiziad.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3pycxripp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3prmiivbn.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vhspctgk.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pajhogda.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hagjkodr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvxnlfr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qtignltm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3msjuyrab.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ytlesmpe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jcbtyjiv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fgplzqux.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sxehltfv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zcxaobtt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hzrjypgn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3yjfeolbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3zpzfhwsq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3phgjerrv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wvynlrqn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vwhpbfyq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pwuqmldf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dyvkgsyp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ylwfedat.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lhpyxutd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3atgqvpaz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3bxqvaera.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kifqbwjj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hsqyzuyz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3lrjkrhgf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mbaprdhd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oqnaccbl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3mcuxvmmu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tzxcxkdg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3spxzuylg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jzoikpzb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3llniikua.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kjhvbvlv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tovtljuw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3befvfdtw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jniazefe.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3laysxxma.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ccoatdeh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yjvtqrxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3poygfpqu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfvkhcaz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3eektdgyr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cbnunugx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ezsoaaxq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lpiaocov.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zhfbbkow.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nnohjhzd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3boblgcrd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sqbqmill.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xvsyyrmg.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tmjwgtkh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3tgpbdlmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3uvzwxcmx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ggsdpczc.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wtqweqoq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zmugaezt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vofkhhpd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3eiaewjjp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lotgryjl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ydhuhymk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3aturfoei.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3origajgo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xxgcacer.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3doeztgrr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xwhcxkkl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3icxyspll.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fkfayljs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3otrkyypn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wtumvqpe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kzoxltax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pmrzkvoq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3kowuufyk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3rxnhmkny.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3vqtcdywo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3yoifxtep.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3wzfgjhvy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fzdveckr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sdugwrgp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3epopuize.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3yfwuhsbj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tfkppwyy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wcutejvr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3znwfnmlf.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vqdyybcg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3cezjdvsx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lslmctee.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3szcornqe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3amsygtcx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3suhvdvxi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gsjjqoij.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dtgevxbn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3rliwsohp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bkfyjlmi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rflmhaku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3djolttcl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3vghdvrcf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wjekcvgo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3adhhrlds.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hvbfduwk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hmjsgzzm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ynitayhq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3orxlogjb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eoiudrvd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aqnueatl.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3feyngbxv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kyuyuuru.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3mirswigr.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xpyxetwc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzkuxrvj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3eyhgonno.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wvdcrkyh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pdkqsgik.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jptjzodg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdinzsyw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ergdztvx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vsjwfuux.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3iztvlaxj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3puhzbupv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gelxqwsp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yrboggde.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sbvhhhqt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztguqxyi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3aoiwnrtx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wyrbufxr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vbzqotdk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3sxdcmwqx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jwmoolbi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hcspjmpa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qldopemn.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3buykvblx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3idsmcnrc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3tcwccshq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cmubdwon.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3rwcukbuw.html


<!-- 参考信息 -->