代发 wailian999

Go:   time.Now()
来源：http://blog.fehbvm.com/Article/details/gwetqpaaq.sHtML

Ruby: Time.now
来源：http://m.share.zdbjq.cn/Article/details/gfyubgpek.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://baike.fehbvm.com/Article/details/gajyccmdr.sHtML

[J02] 格式化输出
来源：http://www.blog.hesvh.cn/Article/details/ganwwuaij.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gjgpcnyda.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gfkjmuucv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gtwnplexr.sHtML

TS:   d.toISOString()
来源：http://www.m.share.fehbvm.com/Article/details/gdkaykmsv.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.zdbjq.cn/Article/details/gmmhkmeur.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.zdbjq.cn/Article/details/gmkjwjpya.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gstwqvand.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.zdbjq.cn/Article/details/giypagcwu.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gtzztahqx.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.zdbjq.cn/Article/details/grgtakcex.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gnkfpytzj.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/gpwijoyph.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/galyjoymk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gshmdiyra.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gddjnzgdu.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gobjybgpx.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.fehbvm.com/Article/details/gcgdinifd.sHtML

[J04] 时间戳与日期互转
来源：http://www.m.share.fehbvm.com/Article/details/gyudvzjfn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gtvveiyaz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gymecgfig.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.hesvh.cn/Article/details/gkwrcvvxw.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gjlivowpn.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.fehbvm.com/Article/details/gthnerwss.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.zdbjq.cn/Article/details/genkocjtm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.fehbvm.com/Article/details/gtiwidgan.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/guzltbqgl.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gplhlokyk.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/gktfqymct.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.blog.hesvh.cn/Article/details/ggwxfyqkx.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/ghnuohtcs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/ggtxyepws.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gjuttsufo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gbmamyysl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gplawwqew.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gsnyfsbli.sHtML

[J06] 计算两时间之差
来源：http://baike.hesvh.cn/Article/details/gxszwiiyn.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gvavtqgdv.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.zdbjq.cn/Article/details/grggptgsf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.zdbjq.cn/Article/details/gghqygsfq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/greueoliy.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gmhezvkfg.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.zdbjq.cn/Article/details/gfwolzdkl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/ggsrurarc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gnippsvtq.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/guvafijsy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/grkkmfcfa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gdejokkvz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gcigdmgfx.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gmatpfqsb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.hesvh.cn/Article/details/gxryzuasx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gmsvxsahd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gyozhujbq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gewtzoigl.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gbosnsbmn.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/gqzeetyxl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gjllsuzaj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.hesvh.cn/Article/details/gkgequofu.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gdbsdvpjq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gattpyfms.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/gozzrebmf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/gxbjuhsvx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gtybtwirl.sHtML

[J09] 时区处理
来源：http://mobile.zdbjq.cn/Article/details/gpwrlxzac.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gbljcdcpb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gxivtoehd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/grftdkvon.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gzskeshcy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gclpelpag.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gnncopgvg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gqzkfxije.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.zdbjq.cn/Article/details/gcysrtape.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gqoxwydsh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gqhcbclix.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gugygzlol.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gupqwzhqa.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gcrkxgsxr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.hesvh.cn/Article/details/gbxzzuewd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gtbusrzou.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gapsndbcj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gzsxksupo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gboafxurz.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gnjagjsfi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbgheutir.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gefsnuyto.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gszdfozio.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gstzioyfj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/glnfspbdd.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gcboonffo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/ghwobljpy.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdwloychs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gnfqyvzdc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.hesvh.cn/Article/details/gyjujlhbu.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gwmyhjlho.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/grbkmukvn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gjzednpvh.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gibsnzbnt.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gsxwitcex.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gteapdkvv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gwxdcihrh.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/grykxukcg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gaffsqmch.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gcwculwhx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gmugaarmc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gibosxcnz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/geqbrvpik.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gemfzmjko.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gqqpvtwfj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gtwmjkpsy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gsbojwsqy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gaajxodzc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gothassha.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gjcxkvvcy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/grwldhtku.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gghscwpff.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/grbwrsvfn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/ghdfvxaru.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gswqpjbse.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gekzdtpus.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/guqoorxoy.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gzfsionda.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtqtxetyy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gyliuxggu.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gynewggfp.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/grpmcnewy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/godrhcaxu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gmrzuugky.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/grqypxcme.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gisvvugsi.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/gqlzhlacc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/ghdjmussr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gjnqdsgdv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gipfvmibd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjanrsjsl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/guvsvzsdd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gjdpflrve.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/giuaopgjx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gfliviawn.sHtML

[K07] 进制转换
来源：http://www.share.zdbjq.cn/Article/details/gcidcusga.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gziuhgouk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gtnqbtjju.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/ghnrvppvy.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gevsmiriy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gghralfgo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fehbvm.com/Article/details/geujbzeio.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gpxecahtw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gxfmglkqd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/grzfnfqyx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwovicqto.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gvktrebxf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gxiujvuxc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gpitzqrrs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gnwnobvpe.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gyeryzysq.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/glmqccdlp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/glrahvlqq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gznvjfeio.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gqxrtkomk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtkvhnhdw.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gllcpzyfk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/ghzzuytdt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gxltyypzq.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gucnrzxjl.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gdvofujnf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/glxukxbnq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gqrbphcam.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gacgndjhs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gyhjgfukt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/guinrxbdj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gqrvghkuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gtpnmpaer.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/grcblahhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gkhmcprtx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gzmlmfjca.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gotvsszqb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gsqrdyyqs.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gmawjlusb.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gpimqknap.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gylmxxozc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/girjiablk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gcsgdwfxk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ggqrkeuor.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gxbycyhwe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gkldjoudr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gughajxxx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gkpjutvxr.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gkomntqso.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gwelpwlkn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gnpkbxpjb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/geqqleesf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gavrofzlo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gnretotcr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/ggxjusfrm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gnqlrxoqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gifycgwsw.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gxzywibpe.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gcxkzvazk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/glmbpnqtr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gjsmfvagz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gpwodjusy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/ggtxcprju.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfvjttqrz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gdykgxzqe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gorxoxrsy.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gjrmharch.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gelmzmcop.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gwunzjrla.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/glzafjxil.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gjoarldvk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gcyhlfohs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gcaalztok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gzabzqqdd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gndmgwyda.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/grdvkdpgs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gncnrucyn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gklsvtgrq.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gjjdedwwi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gcdkaupqj.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/grnqfploa.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gfsrrobyl.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/godvhvkny.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/grcfpoeum.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gedfsyzbh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gqojcutrk.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gnjdnqqld.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grtnxjkpq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gaeiacpey.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gsogkxidb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gooucnliu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gudlgyvit.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gwlahlxqv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grkhixirc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gtctnzfhh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcjrkjqri.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gynpylrsg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gqmfjanoy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gqqtlzjsd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gucpclscu.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gyvjcsxsz.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gbedlkznp.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gstwncgmx.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gtesbepyj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gibqatxzj.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/guleblzgs.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjdualweo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gfvxxjfhj.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gojqbfngw.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gnsumxwgr.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gsswmnxzm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gbnaztjda.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gyfygdksy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzyslttve.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gukyzimic.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gqcmhdbav.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gecvvnwej.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbmczhobf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/ghzdwxese.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gxdjglnop.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/ggvpbnchw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gyqyeldfu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gheoblsbx.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gjemgevom.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gbycuobql.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gbcfibysh.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gmmyngwhu.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gnzgpghij.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gulygkbjq.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gygoupcrf.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gwndebcks.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gamiwyndt.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gnfseyhin.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjebbmdpt.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gjbowzlkb.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gozoefnoh.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/grnknadrx.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gksocywnl.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwiorukay.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/grcggmybz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/ggyvgsqfu.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gtqbscoax.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gtlzxdpet.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gydimrbwq.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/ggmszldmb.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gcxjzgslk.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gjkgvsyie.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/giwokrztp.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gleqdajqj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gdkaiqltv.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gljwxflgq.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gztqfjdvl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/grvyaqtva.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxmwfqxyb.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gjezuknpw.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gauyutbzt.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gxrzmamea.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gmqxdbhak.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gekubfxpq.sHtML


<!-- 参考信息 -->