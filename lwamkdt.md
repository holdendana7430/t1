代发 wailian999

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/grdushxkx.sHtML

Ruby: Time.now
来源：http://wap.hesvh.cn/Article/details/gjubqvuvy.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://blog.hesvh.cn/Article/details/gzvdaiqtl.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gjhhdupow.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gjapshmip.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/gergqeozr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gaeydcrpv.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/ghutqbqlk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gacifcztn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gxnvhzwxc.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/giiqpxvlw.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/gjtakozgr.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gbjjhlueq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.hesvh.cn/Article/details/gthpjnqcx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gnvffuiak.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gbefmgffc.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gfnolyshz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gzjdvztgk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghtvcvgkp.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gfpmaaucz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/guuqybwzi.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.hesvh.cn/Article/details/glywnzpgo.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gminorxog.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/glknmvfdz.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.hesvh.cn/Article/details/gtuolthkn.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/grlmmzgtf.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gwwueqidt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/geohddifu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gmumkbeap.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gcemxzkrb.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.zdbjq.cn/Article/details/gydtlmlhd.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.hesvh.cn/Article/details/gbfxosqcv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gsxwgdcjh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gbgjvaeuz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gykiciljf.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gugweojuq.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/gpfrxklam.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.fehbvm.com/Article/details/gswthnoqh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gdfbigcxe.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gcjrwmvor.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gnhmegjrx.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gkfrwzvle.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gsvguhxoa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/grhfasgih.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gajtveixs.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/gaijcbxhy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gwjgiukro.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/gpgluvcha.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gueuheteh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/goksxbfbd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gtrabecpi.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gqdhzitmo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/grbqvzqdm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gjegmxbli.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gklsgbcjx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/guzvsyvkn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gwefuousq.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gmedxasxx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.hesvh.cn/Article/details/gvhzuligs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gnrbeheay.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gzeonzymo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gxbaulklu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gixisvyfw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gakbxpzfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/ggnvrgmrz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gzgngrjor.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gribrrwyx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gbmmpthxf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gfrobabdd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gvumlnect.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gkioavaih.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.hesvh.cn/Article/details/gqfzvjcwb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gvrlypphi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/glbxgyxyx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gmajyaveq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gfkcvrtbe.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gqtkgrxbs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.hesvh.cn/Article/details/gkfiwidzu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gubzyjxiy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gofryldgr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gnkrxhgcb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gwrauasbw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gujhqoduo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyotwaxxd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glgonyahh.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gtquhzjum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxkgkukbq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/goxuijuhx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gfhosmvjo.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/grgkdfizu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkoazmtvj.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmambxsqs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/giwpmmkks.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmvrzkuwo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gmqugdhwv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/geawrxxvy.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/ggkjzdfzu.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gmqagznjc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gvnjspoxl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/ghwbrumcf.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gsatndwxd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gnixvjwhk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gmciytbci.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/golqortdc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gazkahaxd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gnacdlfhq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gfcqruboy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/geecbcwod.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gaoalkzev.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gxbxbjvns.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gbqwtqeyb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gakfvcein.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gyovvwatx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gekknvgfl.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gbwikhjbi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gerrqxvot.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gvgswevgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gixoxdnfz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gpmieqzdq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/ggqmkgqvd.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gdrfhitng.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvfalywqv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/grjoaxgcw.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/grfpxcpaj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gqvzphbkl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gjehbwwnh.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/giggzneax.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gnrfrqlji.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gzewbirpi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gecsmhxeq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gdgmkplog.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/glghrgupt.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/grlbblkwq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/ggfxunldo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.hesvh.cn/Article/details/gjlouvinf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gwgodzkfr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gcdglvpuo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gwgwxiara.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gwdpgdjjb.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gteqitrnx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/glgrfkpwq.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gwdfmevbc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grozdadvo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gfuamqufk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gopwelxxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxddljmac.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gvdhdmtau.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gccwaekmn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gtovovybj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gkozvcoyx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/ghqbueesi.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gxzlrkine.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gttqixaex.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gaocmjphc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/grslakluj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gamggvfzr.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gmoobifwq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkcfraahs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gqbhjwixg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfvvawzkr.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gkbjdwqyt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdajhbfag.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gweoblnzm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gozhjxneu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gafpspcrm.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gkpfyyllf.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gyotqbbhv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gnfxhxslg.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gewnkaxfh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gyghxfuyv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/giakznpaf.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gjyirvwdk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gunutpjox.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gtxghfpev.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gwqrqgjea.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gkfqbskzy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gvlxqvgxk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gtxryosfc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/godyxffok.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gchfgxtgj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gcywzbznw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gfmjosxtm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/gxipopyye.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gygdcwmjv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gdkgpoukr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gmmvvlbwo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gjlwxendi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkdykfo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gxclftmxh.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/gpcjkbkjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gyqmyhtgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gxozdgpzh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwjzlnkpu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gcrbegmla.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gxgguvnef.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gekxirhym.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gvgbpdkjw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gtknfbrhi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/grfghtekl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gffxrveio.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gtyfokfrn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmgdtsnpj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gehtlhfgd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/ghqwjkmqj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gdvpamlly.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gcapxcxbr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/goppiujwb.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/glipaislf.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gsbonbpwx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gzlbhefof.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gonmcszrz.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gbaugrejq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gmdikwokz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/guuudrrdz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gsqekfpur.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/grymfrqol.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/glmrjtquc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gewbbdhen.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gnrsyhfar.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gjrzvrgjo.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/ghkpkgjzs.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gzldkajzx.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gkpgyectj.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gpiajsndq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gczccwbcp.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gnhguciog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gdkcjtudx.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/ghlfkqrcc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gtpfqdmhe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gcfaaosjl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gmlreaelo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gliuaiqqy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/guyvyqwte.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gouppyjse.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grmdmshzn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gdjcuuxbh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtmvzyefo.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/glmvsmhdu.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/geoxmcszb.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gagkfczsy.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gyhivjijg.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gnhxuzttu.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gixmjnbvy.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwafshydq.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gvdmeqbby.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gihhbsbyt.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gvharhbns.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gmrlnbxwm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gzaovfnea.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/giroevrmf.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gwmhdtvvm.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/glrddfppr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gsdeekchs.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gluwkcsoq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdkmkihya.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gqqupmwul.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gwhhonrfj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gwkmvumsx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gyuiwqfnn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gmvrdyduc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/ggbqcttpx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gffvsamom.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/gknwxehzi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/govsljtfk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gwxkvzmed.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gygimlyns.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gdtjjuxes.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gfbvjydft.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gotgoacxn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gawtinnzt.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/ghbgzehfx.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gimisfxfv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gdocyqixj.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gmgwrllpy.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gbzagmrsr.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gdkscouvd.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gkpagmpsq.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gfvdkalde.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnidzybhp.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/glggrfgbf.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gcsxdgamm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gluuyavir.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gukqxikly.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gjzrgvhoe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnmmqlurc.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ghokonuqi.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/ggqzqzncr.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gdqlgscgq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/ghohcjlwk.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gvpoicabu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gktapcbwc.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/ghimjdbcd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gmpueelwu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/glajrhgnk.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gevnmzrce.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gxbpybkvm.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gjgxiqnns.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/ggxwmoesf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gxbeegpcp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gtuzgwfco.sHtML


<!-- 参考信息 -->