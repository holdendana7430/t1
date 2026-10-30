代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.zdbjq.cn/Article/details/gmojvfjjl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gsngoaxdj.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.zdbjq.cn/Article/details/ggygxibnm.sHtML

TS:   d.toISOString()
来源：http://www.share.zdbjq.cn/Article/details/gvkiknrvl.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gjwfeuhpv.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.zdbjq.cn/Article/details/gvmfbmdiu.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gjxmvdjuo.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.zdbjq.cn/Article/details/gqmeuohdd.sHtML

[J03] 字符串解析为日期
来源：http://m.share.hesvh.cn/Article/details/gwrxgvfjn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.hesvh.cn/Article/details/giztaevbp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gsfpdhqxv.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gfndhxfdo.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/ggxcfytab.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.zdbjq.cn/Article/details/gsczczpse.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gyidifcrv.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gjnupjkko.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.fehbvm.com/Article/details/grfnpkurf.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.fehbvm.com/Article/details/gqjbgsvgr.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gaqxnlxvh.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/gizacgzro.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gegfmbraj.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/gfjbabyhu.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gibwwvdbf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gdoqeumzb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gcyibfxdz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gmanzfpmm.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.zdbjq.cn/Article/details/gtpdyefwj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gcezhjylw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.zdbjq.cn/Article/details/gqfufzowd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gcfjbygcf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gicgdbgss.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gxpzjbfyz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/gkqgouqqa.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvadmer.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gkwrdjexr.sHtML

[J06] 计算两时间之差
来源：http://baike.zdbjq.cn/Article/details/gsvqzmauh.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/guwxoalte.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/gjfsudafj.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/glidrjomm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gelcxwvek.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gyuerejru.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gmuetyoyp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gyehkntgu.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fehbvm.com/Article/details/giavbpplv.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gakgdbtcj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gjuwajdgi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gkunjzhkq.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/guxpzuvhy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/gtofcprnp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gpizapopj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gefnerlsi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gbtaqijhp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gskxfgear.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gubirufar.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gcidouscw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gekwiejpb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gjwxrveom.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/gzhzpddin.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gvbaaxcrx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fehbvm.com/Article/details/gctwnlozy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/ggngvrxby.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/gwbihkcsr.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gxqjgjite.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gaymtcodc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gznopnuhf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gduncaauc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gftsvuxnz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/ggnmodxeg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.hesvh.cn/Article/details/gwwovhjev.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gqcxwdatm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/grjjpaybq.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gsnxpevmh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gfvkbdvbt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gzepybyqh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/ggdwbptlo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gcrrizsvl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gccjwwprb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gptetqbky.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gmqwxlais.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gmbquxqnb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcqbbwvdd.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/gdkoyrsol.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gosdbebxg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/guahrgbzd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gpvtkhwzp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gsiwparcw.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/ghcpgxrql.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxrjxyrdu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/grgvwnluv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gcfhayulx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gifgbiguz.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsnhgrjks.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/gsedguhqc.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/getpfpnjk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gcsdmosar.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gyedyhfqw.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gohdbgptn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gthywqjln.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gpsvgklrj.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gawyizoxt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkdulefvp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gafexfmvx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gkkgyprfy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gwoydffst.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gjugyybwx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gwhesvtud.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gkjfuqwok.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/ghtpmkerb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gvjjmaaqo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gzshoknpi.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gkqxqzobf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gnoaeqcnw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gogrtqsmx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gwsdckqdr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/grhccckcz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gimewvsfp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gfylzmtgr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/geqdngbuk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gidqolcez.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gfdzohfyo.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gnmwiqdlx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gegboqsrx.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gnimuarpc.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gsojkvrdq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.zdbjq.cn/Article/details/gppsidndy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtaihtq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/ghudgqsgo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gviiwghue.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gspyahnjb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gshslqxih.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/grcehbcng.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/glpzdvcdw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gcvbdmeez.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gxyqyrxpc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfuyttwcw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/ggukfwxxm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gsygobblr.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gofcieedv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gupoovbke.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gcjatjoca.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gcxvrcgup.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glfmpvgvx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfikzeyil.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gmblwqjwl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gzalhjovx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ggxtrsqtk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/galzqbtwm.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gykjhqikd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gmnubbuoy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/guicmmqoj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/ghjwxrlli.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gilzbobav.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/ggnjnspbe.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/glomfxumi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gkewmfknr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gseghaqyg.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gkrwfspsi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtujpmobi.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gusxazeye.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/ghukeqyig.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gbqioawea.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gcchhycxi.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gjuvwxone.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gyeewoxpv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeljaksj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.fehbvm.com/Article/details/gifcoeemc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gspmwktfq.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gcwoykcep.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gflvdcelr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gkdhqpuno.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ghpisjamg.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gryqyrags.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/ghpfduawa.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/giibjqrxp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gswdvxvku.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gnipucubj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gjqlsozjh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gletzqrcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gbposyzqv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gvffvqfwm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gxerhsbgl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gufcqmqml.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gbwmtqpub.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gbgqatttm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gswojcgmf.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gqujftuig.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gklakqiyk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gyutaaxux.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gaffhaelj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gaiyskpjh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gzytwrxrh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/ggjusnhbe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnbofzyr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gtansgswb.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gqywqoasg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gxgruqhib.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/glydyeprz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/goxlvqdvd.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gefawjvue.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/ggeowbpms.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gbsjpqczs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gkzyjnvkc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/gyssvbyvx.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gqjxylanf.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwxrdtdrz.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/guyqcfyiu.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfvoopmtu.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gsfjoyhoh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gedxkkvss.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gkuelupwe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/grzrexuhf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghejmtvkj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gisgpahwr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/ghcjttnac.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/ghsnwfxkm.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/ghnttsdgn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gxmmxtdsc.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gtegsmgdg.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/grrravnqr.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/galjpxiqs.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/goaiinixd.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/grnkcohys.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gzxgdduyi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gvjfokqse.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gsryspscv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghaqtzcci.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/grorirvpe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gfnqhpvgx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gpdfcmjkq.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gqswwavfz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxnuxtrar.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gcmeteqlg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guplrjxao.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gitmkeuzv.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gxdcadvdn.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gacxrosbm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/guvuycqmm.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gucgrtiom.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gyhrbaknx.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gqplkftua.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gxewlschj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gbbhudemh.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gchdqzrkb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gbmiqmzpf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gmyhactdk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gkjqtbupt.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gmkjxkxap.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gslsnvcen.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gntjisump.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gpdvnufjl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gajrplotf.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/giodilhll.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/grcjbgwol.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gslbucdum.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/glsfiprvb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/giylurosl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/ghcjogany.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/geilmzcbx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gywnsdael.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gaqjhnltq.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gindhssau.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gsgewralu.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/glfheznyy.sHtML

JS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gtcftkryt.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gvmrwqvqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gzepqhtgh.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/grsylsgkz.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gnvmvtgkw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gqglehrpg.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gjrglqkpa.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyypegxzq.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/grdwrdsnp.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gmmycbogl.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbyvpudgk.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gojojiazg.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvymmxxio.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gemyfwfrg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gzjadirbn.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/glfgfognd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gzgwncjzw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gembyaahz.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gdzlpzvfh.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gkfxavwkd.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gwvylwlzc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gfybqbqfe.sHtML

Ruby: warn "err"
来源：http://mobile.fehbvm.com/Article/details/gdsmettgm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/ggmjkjusg.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gwycvluwf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gdusumoxt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/grhszffrb.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gpzbdxarc.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gakmljqlj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/geryychmj.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gcxjllhnf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/grujcaiqj.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gvdjbfusc.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gqegxpxog.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gcoesykdi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gxhegwgyo.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gwftidajc.sHtML


<!-- 参考信息 -->