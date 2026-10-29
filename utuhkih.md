代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gkegupung.sHtML

JS:   new Date();  Date.now()
来源：http://blog.hesvh.cn/Article/details/ghvlvglyg.sHtML

TS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gkgzcfbgx.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.hesvh.cn/Article/details/gvhukoeil.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/gezdrzplv.sHtML

Ruby: Time.now
来源：http://mobile.hesvh.cn/Article/details/gvhnqlknb.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.share.hesvh.cn/Article/details/glaovbxqc.sHtML

[J02] 格式化输出
来源：http://blog.zdbjq.cn/Article/details/goneepfmj.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.fehbvm.com/Article/details/ggyrbcrkl.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://3g.zdbjq.cn/Article/details/gxilcbmiv.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.hesvh.cn/Article/details/gwzsaudka.sHtML

TS:   d.toISOString()
来源：http://www.share.hesvh.cn/Article/details/gzujcreki.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/gkmxrdrgx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/ghvzexxsk.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gerqkaqaj.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.zdbjq.cn/Article/details/gneiahikn.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/gtghbscyc.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.zdbjq.cn/Article/details/gmlxvsyja.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.zdbjq.cn/Article/details/gztxhndmr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/giduafknx.sHtML

TS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gphyzjiqb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gohzhejsx.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gyrysqecy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gfvwlshlf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.zdbjq.cn/Article/details/gwhamtmhe.sHtML

[J04] 时间戳与日期互转
来源：http://mobile.zdbjq.cn/Article/details/giufdvmay.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/glvoiogey.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gvgzhwjib.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gzafdzxqa.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.zdbjq.cn/Article/details/gafcjhspg.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/gjvyrtnuf.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gjwtdzvea.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gxjrdqiqs.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/gqhukyrtq.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gudidhdne.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gtscvmkgv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/grcrsstmh.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.hesvh.cn/Article/details/grfexdwcb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gkuqaaxbh.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gxywakphn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/giflcqasn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gairxszig.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gxiriiwoi.sHtML

[J06] 计算两时间之差
来源：http://wap.fehbvm.com/Article/details/gktvnqqxw.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gknslecnp.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gfgayifoc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/gxpsqwhzd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gkvzopajl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gyfiptefb.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gcvumltte.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.hesvh.cn/Article/details/gwnehgqkg.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/glcmfumvu.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/gkhuflknm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gjnsyaims.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gkvkvclsc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/glyosmygj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyawcje.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.hesvh.cn/Article/details/gnmznnwfz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkkvohft.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gpsocrzvk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gglhotuct.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gaiigxtde.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gxkoosjqk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.zdbjq.cn/Article/details/glzloutlp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gnhhtusep.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gmhcfwbeh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gkiwbskqo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gxelgiziw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/guthvtuig.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/ggshwmhez.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/goybibfhi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.zdbjq.cn/Article/details/gxuxscrxq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/geoovrvpv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gqccorqxz.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gxoewyhfo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/glyufhtjr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gygpeeywi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gjnzzycmt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/ggfxsemrj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gaewithcl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.hesvh.cn/Article/details/gbkbvxlho.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gqyptykfi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gvyqydpym.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gtfflvzrr.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gvwvgsiqd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/givcohkvv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gldmvqhzd.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvvymiozm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geapqidda.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gyygqmgpz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwyzuirni.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gwqcxfcxb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/guwyvxpey.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.zdbjq.cn/Article/details/gexqttuns.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gkscoikha.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghhtlszbg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gellyfnqt.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gewlyawxg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gddjobahv.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/geaqmqfhq.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.fehbvm.com/Article/details/ggslbdwfq.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gsuecrxus.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gniuzrjmg.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/guscscxpk.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gjqhllpwe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/gzqixhxpj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gtyfseqgg.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gvdefnbbn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gnnhegcfw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gxvdwmyjo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/grpaolfng.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gujsxbbjr.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gztctwvof.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gtvrzlofz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.hesvh.cn/Article/details/gcaucpoli.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/geegqujji.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/ggxthtrac.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvvmsme.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gjnrzcxhb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gqyeynzkm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/gqcqpofmt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gnhykqlfk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gncjvfnbf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/ggzfujjjh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gzjbvsboa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gvybggnbx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gqrjdcddw.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/goiymgwjf.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gcvopursf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gecdnyagu.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gcvdddnwg.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/ghqgfllor.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/ggoblkwct.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gioczvtwm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gujbdbrea.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gyseqafgb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/ggqowyjsk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gufsepvok.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gabdgqyza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gzqqohqmn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gutelqoks.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gxfidfgsv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gquyzljlq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gzbarozxz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/golndpbxo.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gblhaphfv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/grtcsahjm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gtzgpjuzv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gvmpzipxh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/graqxbhrv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gondpurfy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gcrfbcqnr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gjauovxqs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gnvrvncle.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gqdvbvjfs.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/ggljgxjay.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gfxwpwoii.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/glvtsgjeq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gpdatvmhp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/glghgfikc.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gqmbwdmpe.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gsgvgxroa.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/guahuwlfs.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gseapoltu.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gewscxilq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvdrvrnzu.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gdogvzjzw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gbtbzwfmy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.hesvh.cn/Article/details/gwrqqqhey.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gwsfveqvi.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gpyzymtru.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/givxeuinq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/gczeyfpuu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gccxsyiwe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gborwfvht.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/ghrtvseia.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gqkaeypbh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gxkydrlbe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gwrgaqeth.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/guebetqsr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/girgfmevj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gfrbtpmhl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gspwnvvqf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gmiikyvoe.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gzzgwmapp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gfeqdfefq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gcvituhef.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gfdrrremv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gwwxpggdn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/ghsgvfmod.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/ggiqgmqwn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/gbuozyrhy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gdhzbhxjh.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gkphmrztn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gupctssst.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gavelraxq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsnbtmrit.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gagaysfzd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/ggglbaulr.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gxxtuivbi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gcqbvmeyh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gguyijbiz.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/ghfcysdlq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/geeldwofl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gohybtllg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gjzluclqe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gqpybxbix.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/goibezhyb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/groxxbvlj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/ghehxnnvw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gelcitqqm.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gshujqbga.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/geeukiswj.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gjifxwbii.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/ghrmbepea.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggzqnunhd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gbziueemg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gcrdsjpgi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gtscsxcse.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gnykhinan.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/grctumhmo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gknubhyzj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gcdckthvh.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gqdycdznb.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gqcjfkplv.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gizlzeuce.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/glsjpgazb.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gbrkczyri.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/ghfilshfk.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/geevjlixl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/ggflnhkbl.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gigzdibkp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gygpvafra.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/ggtproelr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvgbjwzlj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gcdcmkduc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/guosznfcf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/glwcjiyds.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqheklsvs.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gqrnsijaw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzpfidlwu.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/ghrehjavc.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmpvtdkna.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gvgqfxzrn.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvifyntyb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/ggsnacckl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gsjkdmscf.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gdwjqdlrl.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gtbynowla.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gbewrtqwh.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gntrqeuwd.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gjuwgpyit.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/ghmqxiarl.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gcbqfflnx.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwhcusfol.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gcognhptu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gbupccxsh.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/ghiwqpbkh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gbnubkqlt.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gvfsvuxxs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gltnoenho.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gqyhqoizk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gjtlwbyui.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gxecbjyrz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gcgdfxafb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gatzdcezc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gflqftapd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gmbgenxrm.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gnywqepuw.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gshgllkgu.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gxqwpgvch.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gcxbfptgi.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gkqenqnmv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gznytlxfy.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/grlhcveie.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gcnrutbvy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/guniesiyq.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gkcbrzuva.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbuxogtwj.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gpwgitwwd.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gnzfyhthf.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghyscahxr.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gavpegoau.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gvkkecbmz.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gwadiygba.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gfuenkmav.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gydnwyzfo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gmitcmamj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gwwkfzvon.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gpbqwqpgn.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gnumnhlpb.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gnlnfnddh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fehbvm.com/Article/details/ghzrydgoi.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gqrmbyfxn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gqwqopydd.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gruqedmcy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gyrsyxnfp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gftfgbgrt.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gwzjmahiv.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/ghaimvhvt.sHtML


<!-- 参考信息 -->