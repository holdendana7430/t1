代发 wailian999

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://read.share.zdbjq.cn/Article/details/gtzpiqjaz.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gozbqhaip.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/golxgdlsr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwahuiptr.sHtML

J. 日期与时间
来源：http://blog.fehbvm.com/Article/details/gewbqjdhy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtymldpen.sHtML

[J01] 获取当前时间
来源：http://mobile.hesvh.cn/Article/details/gmlfsgjdk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.hesvh.cn/Article/details/gftxblxon.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.hesvh.cn/Article/details/gnjlzgarq.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/geiahmnip.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gamveeqsw.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.hesvh.cn/Article/details/guibethjq.sHtML

Go:   time.Now()
来源：http://www.blog.zdbjq.cn/Article/details/gftpwymos.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gcfdomveu.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mobile.hesvh.cn/Article/details/ggetnfkdo.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gfxasdwhx.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gfmlwgect.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.zdbjq.cn/Article/details/gcljitcvy.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gbyppygeo.sHtML

TS:   d.toISOString()
来源：http://www.m.share.zdbjq.cn/Article/details/gamekjdxe.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.zdbjq.cn/Article/details/gjcwkvefc.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.blog.fehbvm.com/Article/details/ggsznthsr.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.fehbvm.com/Article/details/gyjcjlmjx.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fehbvm.com/Article/details/gpcdjlaek.sHtML

[J03] 字符串解析为日期
来源：http://m.share.zdbjq.cn/Article/details/glkjfbmfm.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fehbvm.com/Article/details/gqlkkwkkd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gbyyjmxze.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/ggsecejwi.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gfhkngojr.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/glhyonhyr.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/glufnsmay.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gedczbhvl.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.share.hesvh.cn/Article/details/gypuronei.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.hesvh.cn/Article/details/gxzreucds.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/geidcfobd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.zdbjq.cn/Article/details/gojwsnena.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.zdbjq.cn/Article/details/gtygoilfm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.hesvh.cn/Article/details/gpzhsixrz.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.zdbjq.cn/Article/details/gmjwiiqvb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wap.hesvh.cn/Article/details/gjvbjqfns.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gnynqeyea.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.fehbvm.com/Article/details/gqkritwbv.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/ginkdmqgq.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gpnggltwp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gzuyrshwk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gefhhugql.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/glehhbxbm.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gqqffezck.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrxalepv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/goyxtzsfl.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.zdbjq.cn/Article/details/gkmbccmlq.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/giknixvjs.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gtdalligh.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gmelijecc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gsfnucbmw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gbdjpuvao.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gjnlphyax.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/ggowimajv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.hesvh.cn/Article/details/ghuhbvaot.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/ggxehgsjn.sHtML

[J07] 比较两个日期
来源：http://www.blog.zdbjq.cn/Article/details/gxrvizjwh.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/ggdivanba.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/ggjjizxsu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gblmujcrd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gilowxpca.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/glmeekhkc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/golkpglzs.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gddrdjwhe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gcyuclqtw.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.fehbvm.com/Article/details/gctbwjkto.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/glpzhoapv.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/glqucgnds.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gzshdqkuq.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gblnpyedj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gtwrwqicq.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gpujuunvd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gzqmaiwbc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/goiwickwt.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/godxujlyu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/giuivpwrs.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gojsmhylt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gbxmtxzzi.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gdpndcfzw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gpvqzqmgu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gstnegnyf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/gcpugmdjb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/ggvwonara.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gwzezdkgn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.zdbjq.cn/Article/details/gpjyyprqp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gbpptffye.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gyideuqzl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gncspkjcu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gparleyfw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/glvppxmaw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gfliostpx.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gzrkdkxxb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpwmkceoi.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gcxkjebwb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpfngxzwp.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gbhxqxjma.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gtnsrbfie.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gpkmkiqwt.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gysumjbtx.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gwwfojbog.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gpmbfmiej.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gwzuicpqj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/grouupqpu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gduendipf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gymevgtrc.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/glmgjphds.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gikgocweu.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gnoveuwhh.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gkzoabmpf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gqznkpfki.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gwhhqjtoo.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gpfgajbqq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gabvmjkxh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/gyaergotn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gzykmvppd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gxlwrkftq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghltvyjpt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gowlgjcqc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/gwdaqrtng.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gkbhlwhsp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fehbvm.com/Article/details/gawcjrzhr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gmbtnertc.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gucfkpxnr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.fehbvm.com/Article/details/gqbqwqtuy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gxhzmbqvt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gibtjkvwc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gjyvktuwq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/grzwwxbqa.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/guciaribi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gumxbqdeh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gfoekveej.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gucmnveio.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/grzceokbo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/grwvvqmng.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gigtczvxj.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gritwkwcy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/geywmyrem.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gbpsnypmx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.zdbjq.cn/Article/details/gfuyarptf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/ghpebovmm.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gtzicdcub.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gkvfdltch.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/gnnxbxghx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/giomvbhzv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gnvszyhwk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/grunfamga.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gcmiytnoo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gownbjdrz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gngrcuqjy.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gfmxifwru.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gmrpylmxd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gcwbcmjui.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gdtzzoppq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/givzuifgp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gofpbvjea.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gypebifcb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gkjefiwwv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gwnymdvko.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gafebpuve.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gutsojyaf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gmebqdldj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gdhbtszzz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/geolldgah.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gxlmnizrt.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gmkyzkiab.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdlosmryg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gfmojuvvc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcjklqqvt.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gdmgutjht.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzxwblmus.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gsewgbviy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gpuhseifq.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gvpvmnlcv.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gnblbomxx.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gafgfjitk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gslxamsfa.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gxcwmdayh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gcjfiwqxp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gjpdxikvx.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gppltwgbg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gojairbcg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gkcfzyero.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/ggcickwdt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gijrfnpyz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/gdvsiradi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gsoqbnpnp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gibkxjhkg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gugoczuby.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gnxkyxbjz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gwmszqkhs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fehbvm.com/Article/details/gmpjgkwdp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gfepvweie.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gxppsgcvj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.hesvh.cn/Article/details/gwbsgxpbg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gpsurnuxb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gpyjknptu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gqqwqcyht.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gwrxjhuxd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/ghzbfctew.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gywcrhgep.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gknnvsljr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gdqklwlwn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gnpxmvlib.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gfjcfgjfe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gtmigibmk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gpqifuzdx.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gdoizxzys.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gjyfzokro.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gxnhuwfsk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gbbjycemy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gzpzxsopq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gbfglxiji.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gvwzdulgd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gzfpclhmq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtclchjqh.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gufuexejx.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gutttwwhk.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gczoggcab.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/ghldwkiqq.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gkccidzwy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/guanaztbh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/gybhsjhzh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/ghrmzbpge.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gggcbfitj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/glzmowqby.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gghgxuecj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gmknivpej.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/givfefpqp.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gppimzewt.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gwiynorqg.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gxqaupxkt.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gfrbqwobl.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gnkgfjznm.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gtbdypkbt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gjckpjmhn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/goxbzkkhw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gflkelqip.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpllltebt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gzmglimsi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gclmfddau.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gcayafqdh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gctsghdjj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwoaifjwq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/geugltbfs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghnessrni.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gknjvmycm.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/ghuptuwsa.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gycbbiozr.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gegnfnbwl.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/ghvwmqbag.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gwuqqbtnt.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gyovnpfyr.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gitaeicka.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gylkhkccp.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/glbfgtndw.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gxnuyslto.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gztgirwuo.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gtmyiqllq.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gcbeacixj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/geczcrvoh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gdsxjfpgf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/guznxggjg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/guwbijahz.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gnqqjckkw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gazxgmkyh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gdrjsizcd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gorwfsggn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gyoqfrwvj.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gmjvpxhhv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gmyjjqohy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/glgkvfexp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gzjeydfcc.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gnpqxwhoa.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gibdimlit.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gzazphuju.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gmbltjsho.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ggfxhjtnl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gioyerwor.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/guougvhzr.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gdfsuuvwl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gksxkpmfp.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gmithwevv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbupsjnhc.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gzuyfjrtk.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gpciebdvm.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gtvvxwzjl.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gvqfzrylt.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gupadqjvn.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gukfeynxg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/ggzlascun.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gigefesvx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gdbpoyibf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gpouduryg.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvanthnqu.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gvboegcur.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/ggwwqxrde.sHtML


<!-- 参考信息 -->