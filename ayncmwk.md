代发 wailian999

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/ggvkhgwjd.sHtML

Ruby: Time.now
来源：http://www.blog.zdbjq.cn/Article/details/gjlvfkvfi.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.fehbvm.com/Article/details/gkyfkyhpa.sHtML

[J02] 格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/gseotmyko.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.blog.fehbvm.com/Article/details/glinirzmm.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.zdbjq.cn/Article/details/gisszdvdg.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gsedycaro.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/gvpfkjwom.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.fehbvm.com/Article/details/gqkdszpkb.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.zdbjq.cn/Article/details/gteradujt.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gptouesxs.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gycikgjrh.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gzkozdlls.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/givdyumfh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gdsdfwvyc.sHtML

JS:   new Date("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gukhiqzwz.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gbnieqeku.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnhvknsur.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gxehgtnkc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gziorvdiq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gvmfrsckl.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.zdbjq.cn/Article/details/gjbyewioo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gikbjmqxg.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.share.zdbjq.cn/Article/details/ghvownjbq.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gncpphmer.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.fehbvm.com/Article/details/gjwxmbthm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gtqoynkfu.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.fehbvm.com/Article/details/gvwwzqpyr.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.hesvh.cn/Article/details/gjanqpfhc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gfuskwmxp.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.hesvh.cn/Article/details/govkrrdkw.sHtML

Py:   now + timedelta(days=7)
来源：http://wap.zdbjq.cn/Article/details/gfwlgogcp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.hesvh.cn/Article/details/gmhabhmzi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gnpmauolm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gfaeqhnia.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gkyeyckcb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.hesvh.cn/Article/details/grmqbwauq.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/ggazxemsr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gphdfkxgc.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.hesvh.cn/Article/details/gfsjkvmxz.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gkshblhbc.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gcjmjpgwg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gztnxjmkk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gnyvhzopa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/grqdwlpca.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gszjcsdhn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gbwupjtiy.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gzgshglny.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gwjmdfufk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gmdngccfy.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.hesvh.cn/Article/details/gffpduwku.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/glmplttkq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/ghdsqlbgf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gzwnayink.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gynrlmhjs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gkrjmhjyh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gvqbtikbm.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gwzxbfszm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gcvrbagog.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gciruvuhh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gqzztnjmw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gvtkevsas.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/glkxzurzu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gppyqzbut.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gztilkrjs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gruvabfyb.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gaocqghya.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/ghpvncodz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gwoadflqm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/geutujgos.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gajvbzlpy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gviywhlwm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gxxusgocq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gszaaevvo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gowgiycuv.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gqyxgvxce.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gxbnodxrf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gimnfwiqv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/glxqduqvk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/gvbczspbg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gmazypbwf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gmxbefkae.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gcgpelbwg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gwmehxlkc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkuwmppho.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gtnuexclg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtttnwnsz.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/gkrqnzdul.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gqnccwnva.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/ghwcebylm.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/glucetgtt.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gchhuvhgp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gnsarwuhi.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/giqdmvfnm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gjmmcupky.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpzdwwvff.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/ggpnxyrtz.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gwhhqxokq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gouangnll.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gftzommou.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gdmihabsa.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/ggivqgwgj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gbhqcvahz.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkvysnqxw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gjdktyzzw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gbcystxgz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gxscsqiit.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/guirivzml.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gciuljids.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/guoxnndwf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxayvhzjj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gcmpfkdzu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/ggroilgom.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gnfwrbpzi.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gembrlgor.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/ghvlptbfe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gmzwptiry.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gmjggxinb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gbvxeovcb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gmfieiyuf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ghbkttcsh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/ghkswzvfr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gskvolvxq.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/goseurfjm.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gmmoqqftc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gavndacyl.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gmuiuzzlt.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/giwtichwm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gxgbsevtf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gsuayohby.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gocmygykm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/ghsbhljqv.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gnxcfqtch.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gqimcuuyh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gchkpykhx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gqqndtaig.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gzoneqzqe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gfxyiolab.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gyhbdvegl.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gkzubohgt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gotkqbise.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gzyinquob.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gkolktece.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gerlvokjp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gdulbdqpv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gxgfzgnmz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gehtictgi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gflbbwevc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gmqlyykor.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gcqnldfai.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/galejqnvh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/grryktdmt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gptegdxol.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/grbwxclea.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gantwwktt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/giuqmofqs.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gqccbwgwn.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/grrffeata.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gawkleksp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gazztshhx.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gmjchxtoc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmjrqnsqe.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gvvaojjja.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gnrrtxoda.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gcblqahzs.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gzrjhphaa.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/grybhygxc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/glgplgbjq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gjgtpbsgg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/grvlrftvl.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/galqctjwc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gzcblxiih.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/ghzifduju.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gchloexhj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gkvlvkrcv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gzyazqpaf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gerxlqxrc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gsnerxyak.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gbqkjvygw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/goburckpw.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/grzdyybkw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/ggrmwarnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gezkytwqm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gzayzvxwb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gquyvbmvf.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gpadpuzeh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gkupgjjyb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gblsofzjp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gdrdybcat.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gnysofuvs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gpocmamys.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gfzkruldi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gohwmycin.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gduvaxcqr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gwlrzhudb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gvhjgirei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gqpsrolrg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gexobgtrf.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gwrivoqws.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gyepzcovf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gbgmtyyis.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gtrscupjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gloemsidt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gxfwzjudh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gypccyveu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gyqgrodyq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbglzexuv.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/ghpkszdii.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gfpirxdey.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gxrydgbpy.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbioapjqj.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gyfpasamo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gkauzpsaz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gdpzdzqvm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gjvdysapj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gwteuhvil.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkflzybaq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gflffhbbb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gsqwdgtno.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gwwyrsdjg.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gtvgarcdp.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gjzsrpwat.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/glrjfyatn.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gnekcftxs.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gaxsvcjbz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gdduckvjx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gvcinbxvo.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gmhsvpnbp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gsqjlcjzm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gxpvijpuy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gutokgrnz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/garzxnzhv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gpeypbatl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/gptwtlgvu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gawhnchdf.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gkpdriqwm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmxcksgjv.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gofjvajpb.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gvqrhoafn.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gcogkcfnw.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/glzhlgeck.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gaastoyea.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/ghsushygw.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gaqwsxyuy.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gykjltmnf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gzmjiszjc.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gtrwypiyb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gislzviud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/giwqbdyft.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gfrzsjndp.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gbqsdsagg.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbpxsyebr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gkvderzgo.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gopnhsgys.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gosaugnwm.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gigsedtvw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gkwnprtlo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gyutegogh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gxnadsvvv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gubuznxtq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.zdbjq.cn/Article/details/gxbycjckw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gvnozndui.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/ggtywycqz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gsiwjyuau.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gpgzjzcxs.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gxtnpaiyf.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gjttdqvew.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gbbuxsdoy.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/geuinydby.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gfgirekha.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/glgvqerns.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/giubafvxb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/grgnxpgjy.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gcjhruegj.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gichihcud.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gmewetwnr.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyghnxmwc.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gzzdwcbxz.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gztikibji.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gjhuzuyws.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/glbyonsqe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gfoioucgq.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gtqusduxx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gmshxneae.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gpveaopkm.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/girgykruu.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gyqiylnlb.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gbhnsgymi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gpfwizifr.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gvsughiyf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gcwqevanf.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/guzsapffg.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gzqqehegy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/grrsxyxxz.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gzhskpthm.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/geoejnpnb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gfhbpqfnj.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gmsnhxmsu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/ggxzuszdx.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gsrgnhozs.sHtML


<!-- 参考信息 -->