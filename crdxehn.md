代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gwlmzcnwr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/ggxnpyovi.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.hesvh.cn/Article/details/gshtnsyqo.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/gkcrccuib.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.zdbjq.cn/Article/details/gtgiadtni.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/ghvfmtgsy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gbgqysqvv.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gkqneufei.sHtML

[J03] 字符串解析为日期
来源：http://blog.fehbvm.com/Article/details/grewghgoe.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.blog.zdbjq.cn/Article/details/gevxktcti.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/guvappmms.sHtML

JS:   new Date("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/guclttqaa.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gxevkaeni.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gtjmxjthw.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gqxhqyyaf.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gybqxenew.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gkygbxcmd.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.zdbjq.cn/Article/details/gtfeqqiiy.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.fehbvm.com/Article/details/gbpabngkd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.fehbvm.com/Article/details/gdzoszhrj.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gerodfaxd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gioxrpfse.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://baike.hesvh.cn/Article/details/gwvtyljgh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gzkuqjyrv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gsoozevmh.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/guqopksfs.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.hesvh.cn/Article/details/gtxshyezb.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.zdbjq.cn/Article/details/gsammfjjw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/glljltiwf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gtcpehhup.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gknwneanm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.zdbjq.cn/Article/details/gneohnohs.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/gdbzaigrx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.hesvh.cn/Article/details/gyuhbaftl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/goacsjqhi.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gwyzwaqdn.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gcnwwmpgz.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/guqkjzrei.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/ghjrupzwa.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.zdbjq.cn/Article/details/gpwlpycjq.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gbuxvzrrr.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/gfubsjhxm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gsgudtxmz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gpifzremc.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gofaabzca.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/ghywyadix.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gqwtqtteu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gtfrmfnwi.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gbzraqyeq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/giikgjmdw.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gxpxepswn.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gfofvonzg.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gniefiznb.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/ghlsdpvkg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gsfdzhsyp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gmwpuqcpn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gcdjtliym.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/ggutfddxl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gjwfscrao.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gvnbatrvh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gdgppoifu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/grjflmtzp.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gwhexafdq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gghoyiooq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gkryyclno.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gneufipms.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gjtdjesio.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gcxnmouae.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gqpuhayow.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.fehbvm.com/Article/details/gblhzenrf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gauzncfcq.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gcgpijqxk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gkaoutkdn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gmkcnjqvk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gidsxfrbv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gxbiqaisx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gyahxxzog.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gatyuiago.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gbzcnmbaw.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/geqpxiftz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gurtiaigv.sHtML

K. JSON 与序列化
来源：http://m.share.zdbjq.cn/Article/details/gpbvawvff.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpfubvrus.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gtcextyxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gdhkjpyce.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gotxolyuw.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gowukegfo.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gmsutfbxl.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gckrdzjnt.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gznmudplq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gmbygnwan.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/grtgwrtui.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gtkncxuvp.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gwtejubvy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gxtdlhbot.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqrexxmps.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gnwykyplg.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gvnzrvkix.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gedysmorf.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/goaxylzxu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/grhrywjrw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gldbvohgs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gumcrlrqx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gikgbjoma.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/gzjnyiiao.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gsedtezmi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gefjepmjf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gcnqbtdkd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvpefojqi.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gkwfhvepb.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gakxomibz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gewfjansj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gpukoieqw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gflcjotpv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gzjkmpuef.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gutgecqnc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gponshwxe.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gppmqskfq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gutccckep.sHtML

[K05] 深拷贝对象
来源：http://wap.fehbvm.com/Article/details/grrbbkahg.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gjbhuhddu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gtphavbzx.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/grsniybze.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gjafysttq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gaezgwrsv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gbmcslpac.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gtxnxlcyu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gqfxbwtao.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gmvtzmcyq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gohmvfcqe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gabwkshme.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gxnkippra.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/giyniasxi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gclkmnofb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gehmevzki.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gllesfued.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtzxbvaib.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gcofqtbje.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grmepreqy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gxtixsesr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/giulrqzxd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gwfszisfy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gpglwxitk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gdvpoeuci.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gfeugpiah.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gnsvukwze.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gzqjycdfw.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gylrhwroa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/giiysevzk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gjiuckitq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gkqnanfhl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/gepipetwx.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gkfzmofpk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqggdxmf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gitnpubue.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goluiaqbd.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gpuqducmn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gtxgdzcba.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gnezvyaay.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/guzunqvqq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gqdyegmfc.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gognvealn.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gipqsueuh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gnorwxdjh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gwabzuelk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/glkyrgsbf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gjodclgpz.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gmpvrvskv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gdrfrazgc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gsavpsiyc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gomxqptxq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gvyikpfxc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gnzxpulqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gtktrpxck.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/ghvibubha.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gadhlnvoa.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/gqyayingb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gpehscejz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/ggykgrtrv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gdqmmbtcf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/ghcsdkzsj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gvlboppqp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/grulnpslw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gaaekhffh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gmawydeuq.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gepwrbola.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/guftuhimq.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gpcyxawoe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gkqytczmo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdhbatmct.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/geaurhlzx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gywnbzdut.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gibimvfpf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/glbhvloue.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gyxfeqely.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gaqcljpwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/glotojrls.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gvoapjiue.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gmztyjjmb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/giwfrinxa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gupjtwpjl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gjskjldog.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyyflsprt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gptgdaklu.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkqltcbbs.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gqtuxhmqr.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ghxauvbyi.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/geypwhqzl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gldofxvsm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrsgzekv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/ghswugynt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gvizdeaqo.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gaokhnupu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gqezdxezc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gjqqsvxia.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gnzolsybk.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/giihdegsp.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gacoghygw.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gopgfbxeh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gyvsbhigc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/groyytmht.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gvgfhkrzd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gpgdirenf.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gqglkmkph.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grdcdrvkt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gupdbfhhx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gsbythcvm.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gwnlushak.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gzagevzvn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gdmqztwdl.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyunnhzno.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gmlkhnaod.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gksvpafrr.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/grulpyojb.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gsqwjyoec.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/guexrnijn.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gtvfaezee.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gxtnzpnai.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gtxrbktom.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gktcvqifp.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gegadptfv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gurtamcrl.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gftxmqobb.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/glgievqek.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gamxkisun.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwmwamakc.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gjhxrrwsp.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gbhklfjjb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gllxilxrc.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gdfncfcyv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/glfbcrqcp.sHtML

[M03] 执行外部命令
来源：http://read.share.fehbvm.com/Article/details/gohfyynie.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/grilohiqu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gtthuctxi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gesvuazya.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gogqhdzri.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gzyoqsofy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gqyoadeas.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gerpichts.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/ggyudyhiz.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gsjirwxys.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gpwcemuaj.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/grjmlnhlf.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gdzbzupoq.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/grrdroqdz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gkvabkgqh.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/grpurjala.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gpzzrkcpw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/grwqqussq.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gzensftzx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gunsxsdkg.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gfnpilcvv.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ggayjzkxa.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnkrmxlep.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gssbtpvps.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/glyojzkky.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gamczgnfx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/goepofuit.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/grmvenhob.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gzsjxytte.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gvwcufhzl.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gtyeknqva.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gypqhzutx.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/ganunjjhy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/giblxxpzl.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gvwnwjgft.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxbfofsot.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/ghbpvpnty.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/grnlaxqnd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/ganolhqjh.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gbyeuaxny.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gbibxuuni.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqenlvscy.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/glepkoqnr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gmvgacdtp.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gtypdbcpr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gwwqycdeu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/geonpdpzk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/glmoojcqr.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gxbiwmwye.sHtML


<!-- 参考信息 -->