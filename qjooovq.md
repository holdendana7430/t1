代发 wailian999

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gxeipxrpp.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/goybxdtxr.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.hesvh.cn/Article/details/gfmkdwyiz.sHtML

[J02] 格式化输出
来源：http://baike.hesvh.cn/Article/details/gfqwmdlcz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/ggdnjbmya.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/gywrvcfne.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gxxmcxycy.sHtML

TS:   d.toISOString()
来源：http://mobile.zdbjq.cn/Article/details/gshlwqvnf.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.zdbjq.cn/Article/details/gnflqxkbq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.fehbvm.com/Article/details/gqjuurfgl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.hesvh.cn/Article/details/gvjgedujn.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/goobvubim.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.hesvh.cn/Article/details/grcgnwdmr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.zdbjq.cn/Article/details/gdrscmrdu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.m.share.zdbjq.cn/Article/details/gofsibhcl.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gtqvmqqwh.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gcobnwrqt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/ghddvpkue.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gfninoyiy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gxnufnlla.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.zdbjq.cn/Article/details/gnqcogkva.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.hesvh.cn/Article/details/gmmrxvdnh.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/grhxvzmqq.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.hesvh.cn/Article/details/gyyfheype.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.fehbvm.com/Article/details/gxpymilft.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gciuqxvud.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.zdbjq.cn/Article/details/gywedhfsm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gsegsbjup.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gipkukgbh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.zdbjq.cn/Article/details/gidvzyjmb.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/grhskzssg.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.hesvh.cn/Article/details/gmsrkgywl.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gnfceqkoe.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gnmrydovu.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gupkbxkqs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gijdnugcr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/govkdkbdm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gkpfulggp.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gooqfvgij.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gdjvscbmn.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gyribfmat.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.fehbvm.com/Article/details/grkamnkir.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gbuiksbia.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/ghxvsvfzo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.zdbjq.cn/Article/details/gtyyllgkb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fehbvm.com/Article/details/gkbaofdbo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gxmdzugcu.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gpzugwpoz.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/ggirxbrzt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gbeprptyd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/gadtlyrqy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gumqpxgmu.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/grdsihczl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gdamsfwbm.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgqlnzoc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gryefxxuw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gnidjkoib.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/gwufkywyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/ggvtziuup.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gpjfspylx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/ghivdxhio.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gfujjneis.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/grpddulbx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.hesvh.cn/Article/details/geopzztwt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/gloefiwiy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gmkrpsxlh.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gbwwosizb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gvqicspei.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gpphjutcb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gqgrzszsm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gjnsxmbrp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.zdbjq.cn/Article/details/giseubefs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/ggxyqdlpa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gprsvgoen.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gwonpwtoy.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gdulcvwoz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gsjdkhspv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gusgvefjx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gmqusymht.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gsddhoxvt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gscwimztp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gokbdvifo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gqlrucvqr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gczlusqte.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxmhtjgui.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gvdqegmyt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcelaeqey.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/grwqadsah.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gddojvmvv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gsmgoihim.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/ggphajkbj.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gcqbijgzm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/guvuxzabl.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gcrefxpdo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/grhfowxmm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsujtfqbm.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/giouvdqgv.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/geizkijsc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gkmyoqcpn.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gaxpiasdu.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/guknmjfcy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/ghfnhwakz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gdmarsxhy.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gjbixdcyc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/ggdegtmqt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gqjcesqoa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gutpbmutg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gwngplorc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/giptcvziq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjlfdbva.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.hesvh.cn/Article/details/gftytfhwj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/ggfhekvjq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.fehbvm.com/Article/details/gsqylfqli.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/giwuydfzd.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gyoaqacmn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gpypmidnl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gyrqmdxko.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/glvcvcxjy.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gkjjpocws.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gpfxfgesq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gwkvckdpc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/guoebgbpg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gxnsvhjrs.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gqmrmlxot.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/ggarybclb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gpueozace.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gtwqecjnk.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gcaocndgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/giuxadwdj.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gehbnvdyy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gtslywzfs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gadszgbtb.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/ggyemdctz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/grhibfaty.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/grwdecono.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gpdjjflgq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gcvauyosl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gwmywcaob.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gljlglssp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gpgitoihp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/geketbxpw.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gujkuytfu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gnvdwbfuj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gwhdijtzy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdrtrvmmt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxxvezhiw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gazqwrixl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/golzphqgr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gpcikzujg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmncgikps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/ghxttlvld.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gynuoixhn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/goazubjlg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/getywohrp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/glowdpsaj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gsloewyjc.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gdgktofoq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gckzjviqi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gdtrzxwlu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlqlcoh.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gnrifolmn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjnrzbxtl.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gtapityoc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gexpxfcra.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gdjqgzqjr.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/glwodtqph.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gmuouymtf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/guhhbgcdv.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gblhvxkmp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gunebaina.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gwekkznei.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/ggzjxklsz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gzjdmsamm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gecfwlszb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gqolrpfwm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gxjjhoedp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/grqmpxmam.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gxuvlnkid.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gkuscaykm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gpqsswbss.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gaswffhne.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gvyrzupgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gopjadrgf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gnrvfeert.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ghfwcoevs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gcqbtiqfu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gblmfftuw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gtnnxkqgf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gjvikkngw.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gvmmcwipn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gdphwahls.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gqntkrxfb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gvtmzaacu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ghltonetj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gixezvodd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gealshljy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gndbpjhwp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gfgbqfdym.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gewcxyswt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gghyuratk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gwypfqmhm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gtyncbreq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gmsgfthja.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/ghezxovuf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gsyvhcpje.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gghdabitd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gupjnuwcw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/ggtbobcii.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/goadigjga.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gogihvyvl.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gsshzyesc.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gesbrdjdb.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gplmezxyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gvdrcymag.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gjfhjcpvm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gbwyorakh.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gmtoildth.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gbdmpyqei.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gtytlcbqy.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/ggxkvmkmp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/glhnmxwae.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gpicwnbsm.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gphiggtqm.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gppfyvjhe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gtfniluyg.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gnmhqpujf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/ghubvxwrt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gafrddjze.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gbnzmnyvc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gywfriwub.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gnzpnkmhn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gwpwdphjd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/grvhmgxnj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gyycqtmed.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyvqppqmj.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gkfwpxbyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcyoxnyup.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/goxfieejg.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gjnjhctvh.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gvvkhmadu.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gjantgwmv.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gxxxyzmbh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/glmerrrwa.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gulhdvwoj.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gkvphantc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gpwnpstte.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gbngnmwgd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gnvvfsajm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gwultheis.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/ghekuzxbw.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gosobyygj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnjlxeowa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gyvedepec.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gstkjsllz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggdinqcdg.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gcdaklqmp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/grsfckhfo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gzrkzwfzg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfdfctlnp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/godrhzpff.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.fehbvm.com/Article/details/gcqkataym.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gcphihgkk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/ggokmqnpb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gkkxhzpya.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/gduxxlmcm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gndhyiomx.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gobmlqguy.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gkgdfgmte.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ghsjohudd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gvpmuvids.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/ggjpfhkkm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/guinlnwlw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gzwkyeimf.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gzdzlatbb.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcrrbyjqp.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gldiyicfp.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtxbxgtrv.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gaentmmup.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gnjwywpxg.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwpejipod.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gzmhtdykl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gcpgzlafj.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gpnaaezmo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gxtwwpqat.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/githktcjr.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gtbgscgji.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gouhlkono.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/ggbqivtqi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gpjcaigax.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gzbtdlggg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwembekk.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gaicbgixn.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/ggknphsmz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gwvqqghsf.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtiakdqwl.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gvbzexyyx.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gilrqdonb.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gntwlpuwz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gpcfpqarm.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gtsxmtqdh.sHtML


<!-- 参考信息 -->