代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqsvgkmf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://m.share.fanxiaobao.xyz/Article/details/gflmsyqur.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fanxiaobao.xyz/Article/details/gjvsyxpdp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.fanxiaobao.xyz/Article/details/gmwyqhxgj.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqotphwt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.fanxiaobao.xyz/Article/details/giwfkgbxt.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fanxiaobao.xyz/Article/details/goujirthp.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fanxiaobao.xyz/Article/details/gkxxecbxe.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrliqnrj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlsjskox.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.fanxiaobao.xyz/Article/details/gkewknlhi.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.fanxiaobao.xyz/Article/details/gfzkdtnjq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fanxiaobao.xyz/Article/details/gntekstsj.sHtML

[J04] 时间戳与日期互转
来源：http://wap.fanxiaobao.xyz/Article/details/glcevpcas.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcsowwgd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.fanxiaobao.xyz/Article/details/gjnuidpdx.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhcputju.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjnywwxj.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqyibzlq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gttuosvlv.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjazksha.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnovlrvmm.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwtugirg.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjuvozih.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gcgplqbbs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujetfeay.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxmsqcoa.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmthischc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gjxeluwqc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnbwxexv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkckylut.sHtML

[J06] 计算两时间之差
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkvienfa.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqmhfyvb.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbelsibd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfptprrz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdxxufds.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpritkd.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fanxiaobao.xyz/Article/details/gazypphuh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpegdgozk.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvibjbeh.sHtML

[J07] 比较两个日期
来源：http://www.blog.fanxiaobao.xyz/Article/details/gigugeyds.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fanxiaobao.xyz/Article/details/glxyzwxjc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgozccle.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fanxiaobao.xyz/Article/details/gfmwffhbn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtqnhkka.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcukbozva.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozucnznb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/gaigmbwqw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbgpnbskc.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdenkpei.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fanxiaobao.xyz/Article/details/giwfsszyz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvhnyxz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fanxiaobao.xyz/Article/details/glxhjrmpf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrokouqc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fanxiaobao.xyz/Article/details/gvdknitbj.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqfwyvad.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fanxiaobao.xyz/Article/details/grpzlozvx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhxbfzne.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gamqijvlj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fanxiaobao.xyz/Article/details/gzdybbvlh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fanxiaobao.xyz/Article/details/gofzrxcja.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fanxiaobao.xyz/Article/details/gwhhtqkpx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gewsfidvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gggcqwjcv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkplayck.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/gkqqivzyp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkliemwof.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fanxiaobao.xyz/Article/details/girvuyhik.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtbzxiqd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbamipgz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjpzgeana.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuyozdnk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxgcvcrt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gxlzlkvur.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxrykplt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhbadltd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzmegnwsk.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gwcyngygl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnvqgpvc.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcjbbctdy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fanxiaobao.xyz/Article/details/gieduooky.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcwuwujr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaszohud.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gveavgwml.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fanxiaobao.xyz/Article/details/gtygskjjb.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxnqfste.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxunsauyh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszrrtunu.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeqppqkg.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghwfuvmmz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fanxiaobao.xyz/Article/details/guafhltqb.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcezxern.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gcgwcngzc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsphjmxob.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fanxiaobao.xyz/Article/details/ghxvdkjwp.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gfbhclztc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkxjalmr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fanxiaobao.xyz/Article/details/gdccpdpjh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqfdeyft.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/ghghmudeb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnycoskb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfwqnmem.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnljcuoi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkvcbcbv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gjbgzknok.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdlspwrw.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzibthtg.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geezdfcpa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjhqcsac.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnpydwmya.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fanxiaobao.xyz/Article/details/gjvzwiasm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjnqggwj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezxehrxm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmcrspdx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmlfxuvvw.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbijxwfy.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gtuwogvbz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfkltvge.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemgtyavf.sHtML

TS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/glenbybdr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fanxiaobao.xyz/Article/details/ggwufkuge.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fanxiaobao.xyz/Article/details/gyvcajtod.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/ggjgwnqzv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcfozshl.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fanxiaobao.xyz/Article/details/gnrvpjzvh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpkrrlex.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdbhcatl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gcnzupsld.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fanxiaobao.xyz/Article/details/govsfjwii.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrvcwpyt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gxupmtvmg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gljxwmqph.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gnllufcwx.sHtML

[K07] 进制转换
来源：http://wap.fanxiaobao.xyz/Article/details/gxwovdwry.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gzsyjtvam.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/gksisacra.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmincqtz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxyzaziz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbbghdqv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxoiqlchc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgtfkphz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gadwbnbap.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fanxiaobao.xyz/Article/details/gndsfueun.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpalssnj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqvwfbif.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fanxiaobao.xyz/Article/details/gjxgswqgl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fanxiaobao.xyz/Article/details/gdyhhiwwo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqmnomqq.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwlnjryi.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdqnvgln.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gudywkiay.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guopywwah.sHtML

L. 网络请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gkveswzgj.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpvwwzzj.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvnuzgpf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifxiwqoh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpirrchp.sHtML

JS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gemaelvni.sHtML

TS:   await fetch(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwibkojr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fanxiaobao.xyz/Article/details/grhsgbdfk.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuxjctlb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fanxiaobao.xyz/Article/details/gubmbdyel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcjaviwx.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gccblmxxy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glglecmpm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkijzqor.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gxqsmavxr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/godagemoz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggnzvovqx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fanxiaobao.xyz/Article/details/gsxllaqrr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fanxiaobao.xyz/Article/details/gysxhyrkd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizpivgii.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusxptvus.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvlzmlxs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxnhxsau.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gpyxdrkoy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gdvlymtlc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdofgral.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gawyoboqm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gsdxnqeob.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fanxiaobao.xyz/Article/details/gwegsndlx.sHtML

[L04] 设置超时
来源：http://wap.fanxiaobao.xyz/Article/details/gbqpmnjcr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fanxiaobao.xyz/Article/details/gbywjzpaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgcojzuf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/gnazygycw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gedkepbnq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/gmjhinwvx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghhdygz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/ggbcspeqe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fanxiaobao.xyz/Article/details/grigxmxiz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.fanxiaobao.xyz/Article/details/gdiaiqxmr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gsxwbfmim.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fanxiaobao.xyz/Article/details/gkyiqizvs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/geuwflqad.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiffawpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvuixagk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtaxihml.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbzvtlkl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/grlkctfnk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gtgxgghyn.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbnrdbyc.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdazsfwdg.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gtjxtlcey.sHtML

TS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlbvzkds.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmylqueb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fanxiaobao.xyz/Article/details/glddllpjk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gxivvwqag.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gdcbmniaf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gutgmmwbx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuiujlrm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqmzcvuv.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fanxiaobao.xyz/Article/details/gcgphaavy.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gqafxhlgr.sHtML

Java: resp.statusCode()
来源：http://wap.fanxiaobao.xyz/Article/details/gisqtdmqe.sHtML

Go:   resp.StatusCode
来源：http://read.share.fanxiaobao.xyz/Article/details/gtspvsdvc.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/gglicxqba.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpnjtpex.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvvnwjdh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fanxiaobao.xyz/Article/details/gllmuxcla.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fanxiaobao.xyz/Article/details/grrmciytm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvfhyzsy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrgwzbas.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsajsfld.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzrnpjgw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskpkryhz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbkvfvrp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvcmmmwo.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/gjpjrdldz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrdymemd.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjznzxju.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gtczfbfbx.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrkdsvmq.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/goqyykauu.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gasjbmqbh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gohnjnnbm.sHtML

Go:   os.Args[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjsfrza.sHtML

Ruby: ARGV
来源：http://wap.fanxiaobao.xyz/Article/details/gbkfruwtq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiusadsy.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gffptafgb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/ghmefgqkh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gngjwhmnt.sHtML

JS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/ghrxuujih.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxqxanbg.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/ggduzijsd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gnkovymai.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmxtozoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxrxvwwt.sHtML

[M03] 执行外部命令
来源：http://read.share.fanxiaobao.xyz/Article/details/gszhyybor.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fanxiaobao.xyz/Article/details/giafdxfhg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyaqqkbii.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwawaqar.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsxkbbht.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/grnrtmmeu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmxlvjwb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fanxiaobao.xyz/Article/details/gifnnxwvl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrsanncr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbgctevo.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqyehun.sHtML

PHP:  getcwd();
来源：http://mobile.fanxiaobao.xyz/Article/details/gslkbolfl.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/glozveamt.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gbsbnymci.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fanxiaobao.xyz/Article/details/gkgefebtj.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvcdcdxc.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghosfgzao.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fanxiaobao.xyz/Article/details/gsecuwllz.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbdztgii.sHtML

Py:   sys.exit(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gznfjfzon.sHtML

PHP:  exit(1);
来源：http://baike.fanxiaobao.xyz/Article/details/grovxmghg.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaylpuevc.sHtML

TS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkgusbaz.sHtML

Java: System.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjihqjuz.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjturpqho.sHtML

Ruby: exit 1
来源：http://3g.fanxiaobao.xyz/Article/details/gunjbxqsc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbxvfptq.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxevkrtp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fanxiaobao.xyz/Article/details/gymqcqocm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuwjzahk.sHtML

JS:   console.error("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvipnadj.sHtML

TS:   console.error("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/glolugxwn.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggejdckhz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmiagkef.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gqulpjmbx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gzsuplzdr.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvqiaizb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gssbehsed.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjflxbnyq.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gimhfyxht.sHtML

TS:   require.main === module
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqwztsqz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtwhhasn.sHtML

Go:   func main()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueafuwgk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgboqwhr.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtezkcpx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gmedisorq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsftlqqpo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvyzvfjv.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gseqprqus.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fanxiaobao.xyz/Article/details/gguqxewbg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/gtvqxvvyb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fanxiaobao.xyz/Article/details/gwwyazzzt.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvnubbbx.sHtML


<!-- 参考信息 -->