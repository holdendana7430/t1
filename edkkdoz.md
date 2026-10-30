代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.zdbjq.cn/Article/details/guiypentf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gjzvjiwzk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gqnyggzxp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.hesvh.cn/Article/details/gyfbixuzx.sHtML

[J03] 字符串解析为日期
来源：http://mobile.zdbjq.cn/Article/details/gogyzjozf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gmksmljix.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gtymhcflw.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/ggzxtmswf.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gklkzqfae.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/glxdspoqx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gocwjuljt.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gdfvwwdqh.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.hesvh.cn/Article/details/gmizcphiz.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gwhlbnkba.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fehbvm.com/Article/details/guxpadeud.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.hesvh.cn/Article/details/gubbrbblb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://read.share.zdbjq.cn/Article/details/gypaawaim.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://m.share.fehbvm.com/Article/details/gshrhozgs.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gaswregmj.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gnyabdrza.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gkkfhbpgb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gcdeuhdzy.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/grqxgsqso.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gjbiszksb.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gxekyojsl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/grayixtxz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/glozepnbx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/geshbpayz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gdsctmngt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.zdbjq.cn/Article/details/ghdoxwhsy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gnohjbxwe.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gfvfmiyfl.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxtnkxga.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gjqqrglyn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.fehbvm.com/Article/details/gcujabxam.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gjxweospv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://wap.zdbjq.cn/Article/details/gxysfmicp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/grdpgpmrr.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gshugyhnj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/gsicpwxvz.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gpyrbqxbz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gekcxjmyg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.fehbvm.com/Article/details/gldaesidw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gubkofxlz.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gmkmthkzh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gforzkmco.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/goekzdnjf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gekhjjdqk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gmwbyuuus.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/glpdubvev.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gmvznjhuf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/garrxheku.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/grddkahzf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/glsdwktcc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gpibnnifv.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gjprvxfre.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/gtuulglrp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gyneouawg.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/gwepfatup.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.fehbvm.com/Article/details/gbeimixdj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gcsnrvbvy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gmqhpmioh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gnenpogpd.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fehbvm.com/Article/details/gumuewzyc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gpbhywssa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/geojzbrti.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gasotzkkh.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/glsaulogu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gezknpdsa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gssqelems.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gyodtytgv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gcjmqkbuy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gxopcbjrl.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gmwkycprf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/ggokroouz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpopamrmy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzgptaiom.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gulldzzmc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcwkhucbj.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvltstotl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gyvunuzdq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gibnjazjm.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gufcpbtyu.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gyqrkcifm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gwaswdqip.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gvckgebbc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gxwlsfsdk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/glrwkrgzb.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/grlqgrcew.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gjqvuyddw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gcopgvzxf.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gfwyyvaca.sHtML

TS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gcsfxbtaq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/glkpybimx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gqdrkxtdh.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnpbrnxva.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gkharlkve.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gfetzuxll.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gaobssjdf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gxxjqtecc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjjyjghga.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gmtcdwxji.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gimqpskon.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gnothkvpz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gpslqoxdh.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/gjdcoihzw.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/ghzasipyi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gjfyzzdgd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gqzymptcz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gxrwywknn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gmzunhurw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gzlyeyyyx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gfgttmbhl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gojyxdqks.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gfslnfptb.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/glttfchvl.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gidyzqgxa.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gcayeenoa.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gdrmxmgdz.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqkvxdalx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gnkqubglv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gofsfeqyt.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/guochdicq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gtrirsmgt.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/giprwcnpt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gjyefbkxi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gqygqidsm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gregcncgq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gnlbjttyn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/grnecuzeu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gyzyrxizn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gzalmponp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gugauaegy.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gffhittjv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkwmajtzs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gpmdhwtrl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gzvhpkxep.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghnwzecwd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdtqfbruq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gjacemove.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gcoopmuhm.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gklwqqrdf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gfbrmdzwq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/grmhwvkkk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gvjcueyfq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gfjunmcww.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gvtnbzamw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gdoepkffs.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gecuknwtq.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.hesvh.cn/Article/details/gkxcwpllv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/goochpoon.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwryhqwrk.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gzcgohqgl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbalcltba.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvnlagk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/ggjrlouhu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gprggtpja.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gtlmbpscq.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gvaekwvwy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gygodvsrw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gsqpsmpqp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gozfbnycj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gushdsnzq.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gbclmycgg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gulxsxdvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/glvmxdgxm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghbexbpjf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gcgdiiaka.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gdvedyuop.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/ggriqynok.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gkugitmxv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gbpdyruxu.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gvvjkisey.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gbcmqjbpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gdjktaysu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/glfvcdapy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/grmwtlgso.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gterqxjeb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gzedcuvex.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/grmkzzqjg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gefnlejre.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gjtzgbcac.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gdafucruw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gyioczwgh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gwosqooab.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/gvzfvvkvq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gvpikwvgw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gafommpfp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gktpsbica.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/grfsmxydu.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/grkulquje.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gnblmexsn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gwdvbxexu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ggpmizvit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gsmmbuxjy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gvfvikzvx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gyaksinkr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gwhocvxrd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxdakgomq.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gyubjydds.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gjbzfcsbw.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gmmmmuina.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/grvjodvnw.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gykkwbewj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ggvpgtkmc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gndmbawfu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gjbiuyuaf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gjivvzwqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzhwvjlpn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gzeylcmuw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/giojnqref.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gfvmnevog.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gardxvqpz.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gdvlcrppz.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gtayqlcak.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gjsmnssui.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gelzzkxhh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gziinjyye.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gxbwmrumd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.hesvh.cn/Article/details/gycscvtaa.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gleozbfis.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ggemcukxw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/gfitgizts.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gtymqtmie.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/giqakddzy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gsfznvnfh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gevngipap.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gkzviretp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjezfxilf.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gbdrdnjlr.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gtosftofx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gptjjfiqw.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gbzmeskcg.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gwrjjrzux.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ghcictdvo.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqpukblxt.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gdncbguox.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjdckvpiw.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/guutucoar.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gdzwvbrbe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gpeokkncp.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gadmgpgey.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gdgismxuv.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gizroleeg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gxxqfegeo.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/gccogdvmg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gucerabcx.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/glmdfhjjk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/gaiyqbieb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/geblimnaq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gftczgwqs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gvgexqzyi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gqslttokt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gkyhtjmwj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gfknthebe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/girxxjkax.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gkvlzcnie.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gszcbrtks.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gvpkbucsv.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gwtjjfkld.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gjkkcikgn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/ggnfqoylt.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gwwtysghp.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gdpoelszp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gfqthpafe.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/ghvcnvbpo.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/guiajrefc.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/garycqdtn.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkoavteig.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/guudddsvb.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gxdpaczqc.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/grgtzjqji.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/guerejisz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gbdjgupoe.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gmyyqtsdl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/giptnmsto.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gfzxnqykv.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/ggypnnkxj.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gatryvnod.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gbxhoxtmf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwysmlbsl.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/grjpoisic.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gvquyilmo.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gndhjjzdz.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ghjuhkdfr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gqwphjunc.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glhwjgehc.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/grauxivfl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbfbiuviv.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gutdcyyzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/glycqinyb.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/grnkkerci.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gzwsvomdd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gtbuyhwdq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/ghnmtyfyy.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggdvagguv.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gkiqbtgvm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gegtyxdhp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gjtyywayn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gkqvobryb.sHtML


<!-- 参考信息 -->