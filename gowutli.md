代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.fehbvm.com/Article/details/ggnykukto.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.zdbjq.cn/Article/details/gaajybxic.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gueitzmbz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcsmcnrbv.sHtML

J. 日期与时间
来源：http://www.m.share.hesvh.cn/Article/details/gjjvtrupr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gecxjlnhq.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gsadrvvar.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://mobile.hesvh.cn/Article/details/gtealhjtk.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.m.share.fehbvm.com/Article/details/gqfdfelnl.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/gvmkkvclv.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/giyunxpqv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gkjvklnry.sHtML

Go:   time.Now()
来源：http://read.share.zdbjq.cn/Article/details/gnlothxmo.sHtML

Ruby: Time.now
来源：http://blog.hesvh.cn/Article/details/gmmkqmkux.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/glkyjkwvn.sHtML

[J02] 格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gvfibosxi.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.share.fehbvm.com/Article/details/gfizwnqbf.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/ghjrbxsvw.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.blog.fehbvm.com/Article/details/gdtrguadi.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gwonnnxvw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.fehbvm.com/Article/details/ggzmmanvf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.hesvh.cn/Article/details/gvkelrvsz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.fehbvm.com/Article/details/gcheqxtpy.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gnkpcfahe.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/ghrtshvyf.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/ggcgjpitz.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.fehbvm.com/Article/details/gvpbzpdku.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/ghqizzviq.sHtML

TS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gobjzmxzf.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gxegqvpdk.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/gooqiacli.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.zdbjq.cn/Article/details/gvaweryqz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/goanbttnx.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gvksjydio.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/glublpjox.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mobile.hesvh.cn/Article/details/gqggrknjv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.zdbjq.cn/Article/details/gsanovvqg.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/grpcdljnp.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.hesvh.cn/Article/details/grodjcikm.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.hesvh.cn/Article/details/gjudumgid.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ggnugexwd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gfvtsbagf.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/graiqdtjs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.zdbjq.cn/Article/details/gpjpqpgys.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gkzsxbird.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gsjipsyao.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/ggebrkgzt.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gmetjqlnt.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gkrsjalot.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.fehbvm.com/Article/details/gxblgigjy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.hesvh.cn/Article/details/gobgmundd.sHtML

[J06] 计算两时间之差
来源：http://m.share.zdbjq.cn/Article/details/gftxruwiw.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.hesvh.cn/Article/details/gltgtyxbt.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/gwiwgthmu.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqlkypw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fehbvm.com/Article/details/grdifhcib.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/gbnyumwfx.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.hesvh.cn/Article/details/gcbbblyph.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.zdbjq.cn/Article/details/gzpkxvzpd.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/glsscnoih.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/gpktovcdo.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/gajwojgmc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.fehbvm.com/Article/details/gqwrvmvvx.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gfsvxljom.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/gquzbpnwn.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gghcgmced.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/grdwatlbj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gdqibitez.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gxjhrdiyd.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gawhtwyrs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gjemlsekl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gewthgoxq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gdlaymarj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gxixkvsdl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gjnwgadag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gsprpavht.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/gudkyarse.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gtyowioks.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/guxfqazjw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gerdgbqov.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gybkbrura.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gjetdpyzc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gpjzprudj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gqfhkhbmu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/grulmhsun.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gajqqayur.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gcdekwcvg.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gjokgvmuf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gwvwtmkkv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gocpphhvn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gurqwdgtc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gzawdljht.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gqhqqkkyg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gkznpkpzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gvzcpymvc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gclkzdivp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtqwjfbob.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gsqphkyou.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjedktojz.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gvjeyloeg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gduhwmkfe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gldochlio.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gkbgyzitl.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gvczwcbjt.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/grbbzoqmc.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdnwcthyd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gvdapjedg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gspgapywz.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/guxdqirll.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/grvrpqdfs.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/gdxykhktl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpuvlgukd.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gvwcqxttx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gkipzrqfi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gacmebtyx.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gnsesdbbl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/giehasxkm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gdtpcfjkp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/giyfntzwj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/grxljasbz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gmhwwbiuc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gacieztag.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gdxvlpdrz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gtsiqfzlv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gugjxnakw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gimlwhirl.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gcnukmtcb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gbwaggudj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gkfenefxq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gyyontpum.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gomcgdxio.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.hesvh.cn/Article/details/gnddyjmim.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gyjxqfcjg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gfisxusil.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/glxsqjdck.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gdlkjconw.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gtwewibws.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gpquipoza.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/glqcdyyvg.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gdgshrfya.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gjehdeixo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/grpggudxv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gugpfwkbh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/glfgpbfcq.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gspaatxju.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gflsduosb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gnffefour.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gwbeqersm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gaakarupw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gemkksffm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gmumdrrov.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gwaombtay.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gejxtpvau.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gaozilizl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gbaqehkpt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/grgxpbnjj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gfjvcsinr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gsxjyllck.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gqiortmun.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gtdmgsnrb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gelrddbkl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/glregnqgn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/gktvnelrh.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gywqrylis.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/ggkiunmtq.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/ghcdashid.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gbtxlvkqh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gszkzjbhi.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gfdexyvgh.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gerzmjgzb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gdyusodrp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvvnugans.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/gtxefrkoo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gorvcryit.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gebtbyppl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gyqtqkngt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/glmrtbvqu.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/ghyofjqrx.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gnespoofn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gehavbcho.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gcpwtflrl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gzjhqiagu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gkffmoxgi.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gebvaichm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/goxyrudkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gozpdanux.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gxjqmgcbr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gfilrrppo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gsguhyjtm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gjiubgsvb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gmtimywtq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/glxqiyieq.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gvseywdji.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gkksgxbyg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gmufgznpt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gxjmjaily.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmiwgzxnb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/glxuejbcf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gzugzthge.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gwelaxgkj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gwtvijpbp.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gvaairatx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/garquktog.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gzmrzbfaq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gcsllswpi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/ghyzndebc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gzlrricuq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/goggbjuei.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gwstradcv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gvulqrezp.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gkoldoiiq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gcoaishrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/guchgjxsp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/ghihokimx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/getmwjiat.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gxwbekdur.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gtinhawjz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gsdkpbcmb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/giivwfsqs.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gdmzlvhmg.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gskgoazio.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gntaehfzs.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gduwahdcf.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbuovxvmz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/grenzskgw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gwrnphldv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gnsaezbdl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gwrkzoppj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gqmfzsdwb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gmjmmkmmb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gphfamsnh.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/grscgwcfp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/ghkzuvvyz.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gjmcawypg.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/goxyltsme.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gwvmxykur.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gkidzfgce.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/gxikcwjdt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gmhytjaya.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gtfhrqoyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gjoptwzpa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gyyqjxyzj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gibtrzylu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gfvhqdwyo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzchnbye.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gkwbprfgi.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpzndhfdg.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gjapwuzuo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzmgztttl.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/geqzctaxg.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gayppuihh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/grehgsyei.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gvutntdsa.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gxrfufuhb.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gwnzkgtiw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grcfbojck.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gxrzssoee.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/goehongze.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gvhcsigil.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gcocmauts.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbfjveeni.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/glzfcdrwf.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gumonebwh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gwsnapngf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gcwzzaunk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/genbaigar.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gosfylyct.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gojnyazgn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gwabuntle.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gibcwlbwq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gfrudpapx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gwfakmtio.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gfetqwxuy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gbslomkej.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gtbaumsbe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/gghxbvsma.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/ggxwmmbod.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gsddqikqm.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gdsevsfgd.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gylfonvwn.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gytqlixal.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/goztirffy.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gnbxejqkp.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gnaucubfb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gglxbefbb.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gdybiyngt.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gssozaxyl.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gjrlzebxo.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gzubvhqcz.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gbdrvpoqk.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbfnfxikd.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gxjpncblf.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/guteoailq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwhnklldz.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gzkmgvemt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/glsvrfquq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfinaowfz.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/grmmgihsf.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gqcubadrg.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gjlqkbwto.sHtML


<!-- 参考信息 -->