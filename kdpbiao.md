代发 wailian999

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.zdbjq.cn/Article/details/gzmvcffbg.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.fehbvm.com/Article/details/gwhwugosy.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gtkgjqhfg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.fehbvm.com/Article/details/gyxzhipkh.sHtML

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/grhlyappo.sHtML

Ruby: Time.now
来源：http://www.share.fehbvm.com/Article/details/gzhqsxnni.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.zdbjq.cn/Article/details/gdxoywpjz.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/giozwnwnb.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gjdnutgun.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://read.share.hesvh.cn/Article/details/gvurxkudr.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.fehbvm.com/Article/details/gemmiaxye.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gkxlbpaho.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gydlcyszx.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://3g.hesvh.cn/Article/details/ginfnwroa.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.zdbjq.cn/Article/details/gspmxsmfz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gjmsplvky.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gohhuopuy.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gwawsfbbp.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://read.share.zdbjq.cn/Article/details/gdisvwawx.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/ghnrjcbuz.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gnnnwxukg.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gzwhyfhft.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gfptvrhbm.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gyskepzwu.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gkxuynjvo.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gyzfgigfd.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.hesvh.cn/Article/details/gbwrkoehx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gowsrtfjr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gggkeolsy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.zdbjq.cn/Article/details/gwoyoimrb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.zdbjq.cn/Article/details/gxdulhwqq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gzygixylj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://blog.fehbvm.com/Article/details/gzqiwulky.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/gkwgjcusm.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gvinpxsbj.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.zdbjq.cn/Article/details/gqaikmlsi.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.hesvh.cn/Article/details/garetxnke.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/ghmncnred.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gnjtkovoa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gqxjsxxvn.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.fehbvm.com/Article/details/gcbvitevy.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.hesvh.cn/Article/details/gwrdeliwo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.zdbjq.cn/Article/details/gkrlexrmc.sHtML

[J06] 计算两时间之差
来源：http://read.share.fehbvm.com/Article/details/ghfktwyyt.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.fehbvm.com/Article/details/grzxvzxab.sHtML

PHP:  $end->diff($start)->days;
来源：http://wap.hesvh.cn/Article/details/gwysuowoc.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gspevlqhl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gxvwvejui.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gblwcpbkc.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/ggmtpwnfx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/gbdonxmru.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gvzhgknfc.sHtML

[J07] 比较两个日期
来源：http://blog.hesvh.cn/Article/details/gnahsmxtc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gzrejglup.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gusatvwle.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gtkgsdenh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.zdbjq.cn/Article/details/gcafzzivh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gzwjncwut.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gjbujofbg.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gvbtlvztn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gbdnzpvgi.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gmfaokegb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gufbpebok.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/gbzygprzq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/giztrfdvs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gauhncdia.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gidpcsghh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gjuohcqke.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gkukcmijp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gkdegkvbr.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/guschpwoh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gmiqntgsy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gevywjxpb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gofnafrmr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gzzxwkowx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gvqxocjek.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gzgmrwrid.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gcxvgwxbh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gjwfcdxcr.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/geisbxqvl.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gzvxzmbxi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/giiifjdiy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gbrzdefiy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gkzldhkqc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gputaqbsg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/ghtxklkld.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gobyimarc.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gefoyxyxc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpqduzuto.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gjcdspefu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjrajmugp.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.fehbvm.com/Article/details/glxclgfye.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gdbsqnkra.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gwjvxjkls.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gvwytoinp.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gzktajrrm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/ghuvsedxf.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkxgbyoqg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gkkyphqwt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gtrzyebme.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gmwyrbrda.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/gptsabish.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gdnrrmypk.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gshbnqapt.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gzcagnlis.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gyvcbnhhl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gagylsiou.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gnvgxoaen.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gjcqdfwsm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gvrnrutxs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gjjjcbyag.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/goxdbyvcm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gqarswprl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gpkrzcheu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxcrdehgr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gdibhlqgg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbzqnerbm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/guxassnih.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/grsjmjfyn.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gfqrguthe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gnjudbljj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gscyoirwm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gfweqxmwc.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfpmxrxvq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gvxuzlzgy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gpdducuvs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gtrpauzhm.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/glzmkenfq.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gnsvakbju.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gjbxcfgac.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gmdftkzmo.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxvpuospg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/ggybbjpkp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gfbzjucku.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gxqdupadf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.hesvh.cn/Article/details/gokaefhot.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gqdanelnz.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gdzktbwkd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gvnguqcts.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gselhzexz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gaspwbzcg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gmwvutvsz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gjipiidql.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwenreaol.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gdtanjxln.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/guvngxusw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfzireymz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gderrlamm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/geokpkepw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbqnkjyui.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gqbtxcueu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gytnuoaiv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/gitlonhxq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpddpfxmd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/grfgayksg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gskpzjips.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/gvbldbhxy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gjhcvmnav.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gxdtymtrq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gdjtuvgjy.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/ghdpqlfsb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gsiqugbgc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/ghbgknzut.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/godlildmg.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/grdktglcg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwenlxgfa.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gfowmnngn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gaifuubza.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gjyticylw.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gzgfqrvfq.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gwtlcueny.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gctsquduf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gfpxcijnq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gcsiehwew.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gkphiljwx.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gjbsknzcd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.hesvh.cn/Article/details/ggvzbnmet.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/giauzmfoe.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gcpncvjml.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gtyslkgdx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gwjrgjiri.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gkqdvnlnz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gukbhpusm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.fehbvm.com/Article/details/goepbfreb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/grdulhedg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/ggcydmeth.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gltafqrvc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gmtxwigln.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gvocpdxhy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gvytxlvpw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/ghyvkpycg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gprakoriz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gmgufotlq.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gfswxbcgm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gvjjepyip.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gikjtzafr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gutapztnu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gggrrrexc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gbeuvuunu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/guqlktozl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gqgqrrlvm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gvgycjnyq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gwwnqzdic.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/guzhreswa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gpsnaptlh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ghhmswfpn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gdcgrcxly.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gzhomhxvh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gvhibkrfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gsfyuthyo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzhgxioxu.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gpaycwqlp.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gagwmmbue.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gzylsjfzk.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gbuhzuizd.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gtrwjdphk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gpndwyeho.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gocwrzqit.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gzpynoeta.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/ggtgxrikp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/galspkhns.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gayooiyhi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gqodpjeuy.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gvaqriayq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gaofjfwid.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gwodtrsit.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gbfunjqae.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gaxidgxbm.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gerbevozt.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/ggdtvkfyi.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gosjuwcxk.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gtodjnttr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gsxeytuez.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gktaxaujd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gonwdfmqk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gevaqnbvw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gjozxqpum.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gwlpiyxcv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grcmmskow.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gcrdkbhfm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvajzjphe.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gvxtdemcu.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/ghbxcontx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gvshkardj.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gczlalpzs.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gjqpyibku.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gxuxahcxw.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gugkgopvp.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gjznpqkju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/glzbxypzj.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gorhaznch.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkbnxgvxp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/goiptoyih.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gbnvmqemi.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gnliegwkw.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwrhedlcs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ghhdveygh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gxyufrnft.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmkwfwpzf.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/getfnbdux.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gkgvqhare.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gbfbccjhh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gwlfmqsfr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gepzbifeo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/giectnzol.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gbkultwnp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gnlekoewu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gudgngkcm.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gesvpwpuq.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gjkhdrtwd.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gyeuhbuzz.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/ggqzzwenx.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gmorcyjax.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/glokqllnn.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gbvcxqcbt.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gqivckinz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gzvhcnitx.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gtvrgnaag.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/geivlvdpt.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gdashtddh.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzvdpeccn.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glqzqvbdo.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gksaffcwx.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gqhnphohr.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ggbydorfi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/geszbspxj.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/grucoxcly.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gbbfabugv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/glwzgvqpj.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gkeepypyt.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gzoefantx.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/grgvgibes.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gloqzolux.sHtML

Ruby: warn "err"
来源：http://wap.hesvh.cn/Article/details/gbwdswuzm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gyahhzatn.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdkwioamr.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gmvxvsyiw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/gbbenmwtu.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grxfsosoh.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gsbyjliuw.sHtML


<!-- 参考信息 -->