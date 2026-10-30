代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.hesvh.cn/Article/details/glverynoh.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gimhjdorc.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.fehbvm.com/Article/details/gnwnqniot.sHtML

TS:   d.toISOString()
来源：http://wap.hesvh.cn/Article/details/gnjvtrwoi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.m.share.hesvh.cn/Article/details/gzqqhazxq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gxuflmonk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/ggpzaxwxv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://baike.fehbvm.com/Article/details/glrdptsnj.sHtML

[J03] 字符串解析为日期
来源：http://read.share.hesvh.cn/Article/details/gwvlhlbfo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gtbfuekgh.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gtlxgeamt.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/ghtbedfsf.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gbipnduvl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/gkdkuccgp.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gqzprimaq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gbpnvvkcm.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.hesvh.cn/Article/details/gupulblpq.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/gdimckbrd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gcrieewdz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gvqrzcjtp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fehbvm.com/Article/details/gwfagljez.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gjeznghxb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gymnyomvp.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/grmwyxaxl.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.zdbjq.cn/Article/details/ggxyndrnq.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gprpipuwr.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gjvqfntzk.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gmlggtjoh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.fehbvm.com/Article/details/gmfadjkgd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gzydnfbeo.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gmsqzebiw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.fehbvm.com/Article/details/gwjcektoo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/geiyapfit.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gnhgfuplv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gheazjcat.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gbmvoijao.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/gmroocxyl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/ganfmobgp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gumrveluz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/ggkncynhl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gynuzhmlo.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.hesvh.cn/Article/details/gnkxacacu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gtwmpwwwj.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/ghhpdjsgq.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gseqtaudo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gzxdsmrre.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gtowjdkmy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gyhnufqck.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/glkwrvfzx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/guridgbuz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gtexpizgb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gjctyemcj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gwemqvfxw.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gwktoucpb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/geqonabci.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gwjmpfslo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gxzzltpnx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/gxxheqnnp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gioxrxdmn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/grurlpqoo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gbvfbltos.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gjeafwcoh.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gfobmbwsd.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gprqjaiun.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/ghyfhwvvn.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gzfsejhyj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gsthueiue.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gmvtboiut.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gbdawlnak.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gfqshyvow.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/gvhejmgxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/geytirxhl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gesboiwie.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/glxljsbjv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gfqfgbntm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/geetbxxci.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gtdnwuzof.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gmeerpcla.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gqbfkmlnk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gbnfmybdu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glgkazsgv.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gewoxkvjk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guzlekvvj.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gdvbqgppg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gkqdszkrf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/ggmrdufty.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/ginfwtzmj.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gnewtdsny.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gslhvjvob.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gexzrkiud.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/ggpqcqqhj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/grmyyqhsr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gzqzxkuok.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/ghieuefyk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gwwlyevea.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gvncphvbv.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gyomqxmty.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gushacidg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gmjspzbnj.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gjpszefhw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gqxlxklqp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gykpvpjkc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gpzubzznw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gxorzaesa.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gidxpnmng.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gykxvmycs.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjdbidnsp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gnoqxgiip.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gtpbfpkmw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gcnifutpu.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gyqlqsefj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gynpvwczl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gtdwzacqi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gnnlijcys.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gqgdfvhur.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gahurkpri.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gvgehyjoe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/goimgrkll.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gmemjwfwo.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gxfrtngrk.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gwicfnhbd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/ghrwdxvbn.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gvyalqlhg.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gdgtcvaoe.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/ghfwqflkv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gmgcwlxzy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gskiywzwq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gzighbopm.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gkuywjnjb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gpokfhhqb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gbnqfjfrh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gvtyzttjs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/giyyfwnzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/guelaqodp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/goemntiwf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gwdjwjinb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gfgqcplud.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/ghpsylivc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqrutrtte.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gdlwgduuo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdliswzyl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gtdshfwhs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpbpuzmue.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/grbrqxygf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gnnrdhwtu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gvxwpziqf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gkmyrzbpv.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gdajehtwy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gbkmbafjo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/ggoiwpwel.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gcetgznnp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gixyikreq.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gzwgfosnb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsiawlkwa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gegfbtqha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grjdgruay.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/grjazzpjm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghqwuwhas.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gkwqyuxqx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gpjbbenmd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gscyuvhct.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/ghqoputxh.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtolekwxr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/ggnotwozq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/grzxvqhov.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gvpncnmvc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gleqascgk.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gncvxagmr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gcnbqkbgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/ghpzfuzli.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gzxlxyavj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gyoyuwqsu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gpfadrruw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gduxkkyuk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gwtjttssp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gxhuasnky.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gpuxphmjs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gyysbznmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gsqqgdcgf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gecinwksl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/glbqnlbzx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gslqnxocs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gfposexfg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gewevhadb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gpbgfpcpi.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gubkdvfpc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gxzilcxpq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/grwtpfjcv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/grctffwtr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gwsnlatlk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gpxrhdqui.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gylafvfte.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gkyanqtcb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gemqvwxzj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gjyigaghi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/gkfunpecv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gzvfibwhj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gpmbzdgpy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/geseesutp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gtavchqfl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gqjfvtuou.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gutakksmw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gmbzzigew.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gtovvrezy.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gqhiylsiv.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/golzzhmmg.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gszemuigd.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gquklyxny.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gwpjadagb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gfwtpgiem.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/ggxxdxjvb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/grrwtqtro.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gesyiwkco.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gmmggcdcc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gtvovzvtq.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gbnbvibpb.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gsokyckpp.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gssrnelyz.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gdiojpuzp.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ggrtvpurj.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gnolcozvg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ghbmhbrdl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gmuokulkr.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gavqkydnx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gonozjwuq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gyzwfkbam.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/goklqxnrs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/gdbcoexgy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gxtmkysrn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gkrbhirut.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpgaqytfu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gaayfjcvo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtatchogi.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/ggtktcpyn.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbwqkatgh.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gtgxjrydi.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gaoqcceii.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gzmnmiaqm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glwtjslwi.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gkgrpjkvo.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/geensjcch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gzasofytj.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gwuznaccz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gdgaapyiv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gbseahpgq.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gntxecalk.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gyalwdfxm.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gdijbgaah.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcmnbdrec.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gkhowxqmt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghpqslrux.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/grdjjxpxc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gynzrztem.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gqqhyzqhj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtmjzhjat.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gztbdkbrp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/ggmmtbyvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gkbxbnwgb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gruoozxon.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gqkvjbfhy.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gkhnqivxd.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gyvyrxiym.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/ghzgeiejg.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gcpfmlzrf.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gdbufoepk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gyjhfzhco.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gjttrpsew.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gjituwajr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gwvvxdsjj.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gfexjqwca.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gybaldqrm.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gmfirdelx.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gtzevqcsk.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsfeiiyrb.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdrgvobdl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gjbderfoi.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/goczisdwy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gxupskdda.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gzfiijzce.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/geplxfjry.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gylfqmfmk.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gklavonad.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gdgkfkygt.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gutyippjy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gkayxwasn.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gaxsfwkqp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gkdzzrrkf.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gbqrcspjp.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gnxkeaiwf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gvdqxfpql.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gksxdvxrt.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gtntdcgsj.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gktdhlawp.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/grwqioqvd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gpyxnqvxm.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gosihauuf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gtcdljtmg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gypbvftxd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gagdzuyuw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gplwclakh.sHtML


<!-- 参考信息 -->