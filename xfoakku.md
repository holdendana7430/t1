代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.share.fehbvm.com/Article/details/gdmlqecnm.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gtvbkaxzl.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.fehbvm.com/Article/details/gkamigdbj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gggorujqv.sHtML

[J03] 字符串解析为日期
来源：http://blog.zdbjq.cn/Article/details/gtzzjhwcq.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wap.zdbjq.cn/Article/details/gyiaermwp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gmiwuwnnt.sHtML

JS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gmaaahloy.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gozdnsemz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gcxmmkkdi.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/glztzlwoh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/golojdwng.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.fehbvm.com/Article/details/gmthfadvb.sHtML

[J04] 时间戳与日期互转
来源：http://baike.hesvh.cn/Article/details/ginoxcaej.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gvireclel.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.fehbvm.com/Article/details/guvxwdati.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gtyphpjsg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.hesvh.cn/Article/details/gkztblggo.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.hesvh.cn/Article/details/gejighiih.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdmqoanse.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gksmnlawu.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gvppzajsh.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gwhmcbfzu.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.fehbvm.com/Article/details/gtifncmrh.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.m.share.fehbvm.com/Article/details/gctaisghl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.fehbvm.com/Article/details/gztzyoipv.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gquruflbb.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gxyeeyuhk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fehbvm.com/Article/details/grqtpfbuc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.zdbjq.cn/Article/details/gfhsdveek.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gmscffiuy.sHtML

[J06] 计算两时间之差
来源：http://m.share.fehbvm.com/Article/details/gxkmjvwlh.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.zdbjq.cn/Article/details/gucmefnnh.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/grvuvjtxi.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/ghnbedzqz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gnbybzpqj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gvkfqjgez.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gyddjunin.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gfvybpdiy.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/goyiegycj.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gqewxxrvt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gwlneylxo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/ggadfoyva.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gbqyecvda.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gejtbfkfg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gprfkwgan.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gchpvimgg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gmjbmudet.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gexpbrwvx.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gwzvppalf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gqrbydqzi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gttbihzzw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gwuyahrkc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gwsuvgvhi.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.fehbvm.com/Article/details/gwftzavms.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gouginlot.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gbpgqwbjq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gtspvqiyi.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gbeiaptns.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/gjbqijskw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gxpmxpyxs.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/glbzqzhkg.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/gfzymzyak.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gfcojicgg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gmofhvkge.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gdbfinjyc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gxjxpezqy.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gaxfzuode.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gsgasgboj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gkeomaxvh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gnjyzebac.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gklkbninp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/ghtwmqpfe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/ggpdqnmrr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/grfgquada.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.hesvh.cn/Article/details/gxepadtwi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdycajuic.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gsyvgkrup.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gygirqgaa.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gpatdgalr.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/gvpwxeoiu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gjnktkgzn.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gjhanngok.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glxnlhqnu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gbvrdcvdc.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gkzlkrumx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gurvsjxdg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gtlbbcbtx.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gypahzmsy.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gzmenuepn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gkyishrvy.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gofnxgxwq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdgzabtpt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/gpocbuyhe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/glxqpaoqe.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/geikztbip.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/ggmcbobcu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gvmhvanyn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gbiwuctii.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gtxgfmhcx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gwzqetnyh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gtzcarjzc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gpvpdrfog.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gzqtjurtx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqltzcyec.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gxhgzbojc.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gopbblnld.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gfsswtueh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gubqjimkr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gtiwxfvsw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gwjkzjyit.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gbhxsajzy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gypyatbvm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/glzbjoytw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gwmrxcjzw.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gdynpegmk.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gobbkqsto.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gfirmvqzf.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glubjlnej.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gusmpynaa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gyslspwuu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gmikfcpob.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gbldxnxsp.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gwfqnpler.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gqtlunyjy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gioioadga.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/guyttitmm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gczlbcfer.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gmgyfiayx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gmmyujhpn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gwcdbksnm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gebsaymjq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gjanjuxct.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/glvtenksm.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gvjfepvrl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/georukadq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/giowjgncc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glmmzhadm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gouybgxuj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gqmqanqfq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gjzzdbwfi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gstwdytcg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gsssbradg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtcojutuk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/glatbqhha.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gcowctqoc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gappasbvd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gguwkgikx.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gvqttpxoi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gmeqhxrlz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gowpfjecx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzfcernxd.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gcwvaxdbl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkhxtoujt.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gvutjzmxu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gswaxvlkb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gzefgfwni.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/grnqwqzuv.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ggbusxsjb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gidyegnfx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gxjtvdela.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/ghobamhqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gxgdnsagt.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gemavvkga.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gxbmwyjfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/guyejbyze.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gybzipmfs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gxliuthzy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gmbjhqjme.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gazotuopq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gttvmznwk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gjpjmbgkj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gueixlpru.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/ghcysokyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gegvpnlht.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gngjrcdtu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/goaqiryoq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gdycuxgoc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/grgpnhxth.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggemxhgsv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gbpjdampo.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/ggnyaavme.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gwjedtckp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gphoztmqs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsywswlut.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gnutfhdbt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/guihczmfv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gnwramvoq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gpzxuoxto.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gtpikpnew.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/glxdroztl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gfdgqabiv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gqpkrcksu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gvqqdwmqt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gjsnkqyki.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/grrbgjdza.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gteinptes.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/ggvuqercb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gekogblch.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gkfoackje.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/gpqtoygks.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/gjjzsudol.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwedrfkps.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gcrgfpwrx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gbjqhqodx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gdpymwgpz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gemjhguje.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/ghelbdesf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gdcewnjqg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gtzzjecnu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gijaunqyr.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gnauarkue.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gvopqkanx.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/giamjsyay.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gbznhdpnc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gcofwsdqx.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gbohldudr.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/ghxvqzsqk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gpfzfcugz.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gzobrbwtv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gpyncbfuy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gvewycitv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gfqwyuebh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gwtnrchfy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gzgnbldts.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/ggntaxjkx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsjwdolgp.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.zdbjq.cn/Article/details/glghlvwdp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdnnddyps.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/glcmospep.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gvmqbipvv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gumyrhdoi.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gllschrkm.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/givferjbf.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gaqsldvva.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gcdgtsnuf.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/guwfzspcr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gzkosshrl.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/geauivaus.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gecmptdrb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gyiinmiev.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/ghyuspcdt.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/glwgtmyaj.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gkxnufycg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/geeynoizc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gwchtrjaj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/grmwdkrts.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gfaosmxyg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/govltzfql.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.hesvh.cn/Article/details/gewjxvbnr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/glmaheszt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gihiblzac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gfkhqsfzf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gjuuntuql.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gasrhsite.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gxytuzvvy.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/ggrfobxnj.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gipcdvwou.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gthjtqqta.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gkazorwcp.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gsgbxdnyq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gmhawflwo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkkbaozji.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gjvnzqxqo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gvxzpkveb.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/goguualgs.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzumhdrdn.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/ghukueiff.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqcecdjyh.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gxxwnvxjw.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gouwukdhn.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gpwdloblc.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gkurfxcko.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/gditgbzay.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gzsacfccv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/geaxeozqx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/ghomxsxiy.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gqktohiyr.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/ghpcynotx.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gnbbmxawg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gtywdlogq.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gldmanzlk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/ggftdwele.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/govognbjc.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gibqetszz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gjmhwlctk.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grpvulwsz.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/glyumeiup.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gieqvskei.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gkmjfxtsn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gerxzguic.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gretsgvtn.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/gvbwvlpac.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.fehbvm.com/Article/details/gzldoltsi.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/grkgnbltn.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/goldwwsxu.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gpphwjdmw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gwostydbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gljlwhccq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gmxhrloqn.sHtML


<!-- 参考信息 -->