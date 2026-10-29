代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.hesvh.cn/Article/details/gfmywmtqi.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/giqervmog.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gxvbipokx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/ggeiukhxx.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/gdzeufuoo.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gxfytrgdt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gyzrvlcae.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gvddaabyx.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gttyaoluz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbuehykn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/grdwfcodq.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/ghvnwouhj.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/grqgyhigl.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/ggjmqprbn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.hesvh.cn/Article/details/gdxrytimt.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.hesvh.cn/Article/details/gvflhhhwt.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.zdbjq.cn/Article/details/gfmhgcyxv.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/grhxkfilg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.zdbjq.cn/Article/details/gbrlintwz.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.fehbvm.com/Article/details/gmpumrvpb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fehbvm.com/Article/details/gxskdqetu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/grmxywomm.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gxufgautk.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gcevovgqm.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gundumwkm.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gxbwnlqcg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gtczywlpz.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/guwxgfpci.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.hesvh.cn/Article/details/gccwsmsak.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/grvhdciqv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.hesvh.cn/Article/details/gycgmbhho.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/gqdppupcm.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.zdbjq.cn/Article/details/gfsurcywf.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gfkpessaz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/geyhlgzwv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gzfwnpspt.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/gtyjnjnlr.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.zdbjq.cn/Article/details/gshgskzeb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gksmotvdc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.hesvh.cn/Article/details/gaaghrmya.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/ggdiwcnrk.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gtpqcmucu.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.hesvh.cn/Article/details/gaawpmohu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gcpuzrqol.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gukwkilpx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/glpsdbktd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gdazsszjs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gsfctajho.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gtpeleqvs.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/ganjawfuu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gmvodsuug.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gaotgkywg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/gefdxvhij.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/glryrmrmm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gnvidyfkp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gjdwjgoqn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/guydtyfra.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/giuvruhsy.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gefgfdhkh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gfzfbdigy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gilzdsvtm.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gqykvznyg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gjqsszbsp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gmgdtskjw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gosywjcuc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/guvyoqeje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gzuphlysw.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/ghvwouayq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gekivoibf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gzhszgwzm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/ggtvnlfmd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/giguqoxgf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gmbpxcyob.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gvgbrrhuq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gnocyynmq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gwrmrolln.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggfndudte.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gxxhuclso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdmfeywre.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gvpmojksg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/grlxrvgoz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gaewcbzbe.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gifcvlddz.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gwwhyklby.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/ggyxeliba.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gzqycpxuc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gyuzkjblk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gvruheejj.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gyonboxgs.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gfdljugnc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gytigsjzv.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gxkpambfy.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzagfkzei.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gsggsrtxl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gsgihzjmf.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/genugvxph.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gokqlluvt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/gklzlgedr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gbadpiova.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gaddnyvwk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/govgaeylo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gasiiexgz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gidtjrmac.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/guvrgexkb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gziedemyx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gmfomwfcp.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gjviktlvk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gwjxkvmmc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gjklmnbcf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gnlzqqrbk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gjjztzocs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gyzvfroqr.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gktzwmkwr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gaigerdfz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/ggzpqzlvs.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gxvafreut.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gisqkgzsc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/grioilgpn.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gtsrqhxls.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gcxjjtswr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/goosioehi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/guaohhooe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gkketcvyw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/ghqneiycg.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gkcfneqqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gkphpbmfc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gfwnizvgk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqejxnwm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/grmeqnqmi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/guvdisajl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gvxjuntgq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/ghpwnxuel.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gepealuap.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/grqfacggy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwbusaqtg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/guqokzxyv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gjtomencf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/geonkywhe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/ghhxofkbj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gmzjshemo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/grermnmvx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gklmwpruh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gbtzgflry.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggyzockpq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/guepsfwyw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gsonczoco.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/golfjejby.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gdwivcdna.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gkpmnhkwl.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/gkhbtzaqs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghqygshxj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvsjukhmk.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gvzrmmepb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbavfhsfp.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gioexmnhb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gkspnkcxx.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gttabvpgz.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gmkzkaihm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gmopuceej.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gncnmochh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnoznmgge.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gnyvjjjxr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gmyyfigqi.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gvddxdhvu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/gyaokscdv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gkkwklnra.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/glboxrzqv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/godwqrnmi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gitoniyww.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/ganiuyzai.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gfokvehke.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gbxwhszdd.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gldocvgsq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gdhpmnvuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/grlnwwqce.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/glmyrghpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gwgzwmrlp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gnwovzcdk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gtakcqmhk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.fehbvm.com/Article/details/gmcqmgwzt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gesjbafaj.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gdnafajax.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gcnjjeqmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gfygiomdy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gnjtmadhk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/goinvavza.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/glejnfdkb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gtdddtyew.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gnmxoxudv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/ghdhqcaim.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/ghjunafis.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gzcgzmayi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gnivjlmnh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gdatykcjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gjnpadhlv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.hesvh.cn/Article/details/ggwvlalhf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gisarqidu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/guzgzycyg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fehbvm.com/Article/details/giasxdlhl.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gedyoqucv.sHtML

Py:   resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzwyhutyg.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gkilwcdoc.sHtML

JS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gzcxxjivj.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gavjbzlvp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gazygvtyu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gharmriki.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gwcesabsn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/gaehuqhwg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqhbaplyz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/glesiekgz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gywewyzpe.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/geezqmpxs.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gfqlsxnoe.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gsoozqmhr.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gwlwzifcb.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/ggweqtjwm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gtcwlbzvr.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/glizexdsv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gnywpsybu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gylufarwg.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/glvkrmmfn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gkwpwzhav.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gbugaenki.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gexlgopmb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gpdywanbs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gnljfddso.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grdcyajvp.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gumpjvezf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gsnnoxbrv.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gzcpbydnl.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gsogeychn.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gijwckjbw.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/guspjkaem.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gzxmlrbym.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gbfywpxdo.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gqslcqgsp.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gxpedsyzo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gzqealdiu.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gmwksvjiz.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmnrmrutj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/ghgibtwiw.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gdxglbotc.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjgashfqf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfsaaipop.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/giqdwifmc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gbzoklnxz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/grwxkducl.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gfuxjhhac.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gfxfxbhnp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/giyjcobzw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfyeazibo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gtzwwdocx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gruvclahj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gaqsvfboa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gjnmpsoyc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.zdbjq.cn/Article/details/gjjjkecsd.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gkimcelkw.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gvmtevmcu.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gunawbsnu.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/ghfvumjgl.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gautbzdry.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gkglhrytc.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/grrnezlne.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gfupnsizp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gtisgkldd.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gjizpgksv.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gdxaigzux.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gbxgtwpwk.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gcjnstwot.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gueahirhe.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glkadfzkq.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gpqwgvrid.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gqdrvoohn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gnaenyryg.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/ghjylrpse.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gyvjfvkbg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gecdrtqxt.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwepkvauo.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gbuupdsut.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gbzgpersq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gaygyquoe.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gufvauqwf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gtgnzwuzl.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gnqiaantm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gyiuwmzyk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/guuonllzl.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gudaupmpl.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gxosybpgj.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gmvcyvlqq.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gmxutsffs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gpkrnstpi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/guwvputew.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gqycuhoqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gtbqtwtgr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gpzktlrjw.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gnckrvruk.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gbyzfrwko.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gfvfrjwaw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gekxlnrdu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gcfjsibzp.sHtML


<!-- 参考信息 -->