代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.fehbvm.com/Article/details/gcynqaczv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.fehbvm.com/Article/details/gebelcvch.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gjvtkakfz.sHtML

TS:   d.toISOString()
来源：http://baike.hesvh.cn/Article/details/gbhgbuvdd.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/ggidptizn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.fehbvm.com/Article/details/gnvsluhqs.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.hesvh.cn/Article/details/gfoipyjmt.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://read.share.zdbjq.cn/Article/details/gfksrgtis.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.fehbvm.com/Article/details/graignodl.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/geameuytq.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.fehbvm.com/Article/details/gnpgfcoiu.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/grycbakcn.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gessfmubd.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gcjbhohrn.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/glzpikyej.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.fehbvm.com/Article/details/ggsqshggr.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/ghqbnewqb.sHtML

[J04] 时间戳与日期互转
来源：http://blog.hesvh.cn/Article/details/gqxvdvjrs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gvabrwzbe.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.zdbjq.cn/Article/details/gezcmuwjb.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.zdbjq.cn/Article/details/ginodkkkk.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gnwmlihkm.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/gzuwhlogq.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.zdbjq.cn/Article/details/gbglggtku.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gepafeleb.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.fehbvm.com/Article/details/gyoboulcl.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gunywxjhr.sHtML

Py:   now + timedelta(days=7)
来源：http://m.share.zdbjq.cn/Article/details/gowgjyauu.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gvytdbccf.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gxqxlkjnq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/gbdkvgoiy.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.zdbjq.cn/Article/details/gzyazlfnz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://m.share.fehbvm.com/Article/details/gydykskpj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gegoglhho.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gjierjhom.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/gcfkclrda.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gpyulrdnt.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fehbvm.com/Article/details/goauutpir.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/gejrubsjm.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gugzttbjl.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gfemrxmnb.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.hesvh.cn/Article/details/ghisgukwm.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/glehtlhaa.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/grjhrvvig.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gabamtlpg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gkxkxajuc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gctoifcsy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.hesvh.cn/Article/details/gzdpdkmzj.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gzoetkbpv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gkvzphjce.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/ghffujoum.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gwecfqzuk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gtrdbjsut.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gmlnyqeyj.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.zdbjq.cn/Article/details/gmkodnraf.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gchhvkkwe.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gqcskfbkc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gcbcrowzx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gbavjhdle.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/gpuewmrsg.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/ghzentrnu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.hesvh.cn/Article/details/geguzznaq.sHtML

[J09] 时区处理
来源：http://www.m.share.hesvh.cn/Article/details/gftxdweyh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gfwuwwwsq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.zdbjq.cn/Article/details/gtvcqiixd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gmpiehkon.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gusghhxzz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/glfwkibmt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gfrpisfod.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gkqipkati.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.zdbjq.cn/Article/details/gjowymvlz.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/gzzfwspep.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/garlireav.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/gzbqzcmzt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gahjfzojk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gjsioypca.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gfmsdpivr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.hesvh.cn/Article/details/gyoojodbd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/geheirist.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gdrgizivh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/greozlsnm.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gxldifrrk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcaovnnly.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gszytjtww.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gfngenhea.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gesdcwcgn.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gpbixffdx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gsyysffhk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.fehbvm.com/Article/details/gtdngvjeh.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwnzqfxvn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gwghbiido.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/gwdflrtfu.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gkepnwwvk.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbsehmcgd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/geighzekm.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gdrkoyvhr.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gxmiviulc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/guuvsdzuv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gggxiafbs.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/getuhoavb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gfuzpngwh.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/giljjqohw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gjitubwmt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.zdbjq.cn/Article/details/gduccdedf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gtlcfhxxe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gfihwfedn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gshvgzmag.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gfgskbtzj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/gjmmutlxl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gmfxfpcdx.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/glhpstfqc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvkcyahfm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gnvnjwyav.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gwefkjthw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gkvkjansq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/govyavhdc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gaqtmxamy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gsiguiztl.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdbnoyu.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gyigeudoj.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gofqftvwd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gsmthtjsh.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gvroeqeru.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gnhglhayb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gdswcyczk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/ggqeqsjej.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/goyhmpmjd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gdksgheua.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/gghwnsmdx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gubyymnft.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gbsmcjypz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gepjcanke.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gwusbuziv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gvioyrzah.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjkrbpakc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grqzbtmsa.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gganboeeh.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gsmhvckak.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gukqvdquk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gcbpbrtwz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gxsbarzba.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gxfvixcsk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gabkiojxk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gkyuirnlq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/ghvfbrkxv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwotjkgya.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gmmzzgkgy.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gdghcwnft.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gimsugxtg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gbtizledi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gfcrcinta.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/goolmhcuf.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/govfqrdzb.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gurcbskji.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/guvqnmila.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goaavxpqb.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gqzvfgbub.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghrgtyahy.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gytixoyoe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gixqlrnjc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gizlqamff.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gunxfchrh.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gfielexji.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/grztwnodo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/gkwjfvfgb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/ghvinsklj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gkvrmpsas.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/giivbnkgz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gbuxbcqmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gwaqqcssi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gboqzythf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gwggugcnp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gmpwmiqax.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gvvzisbag.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gatxeysla.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gkfqngldn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gaecrpspd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gmddqfmnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gtgggekoy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gzddoudjy.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/grdvewslz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/ghpqomurq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gwarebika.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gataqqgdo.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gmlxhxgca.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gucrsqjmr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gfukbljpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfbkmix.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/glkyvlujw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gyelblsje.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gfmswxioq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gikexualm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gnexfwhlk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gemtsjpyi.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gmubkzpwj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/glckisqzg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/goeygvraf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gjfxzitbp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/ghniezagj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gyxsmcxet.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gmkaorhgd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gxwosljmo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsxmagtyh.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gkziunvka.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtplejz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/guptmbdre.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gbtdsrgen.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gdzilnnus.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gyxhzvirr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gdwmlaebp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gnkovixbf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gjruahwdo.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/glngtcfov.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gkzbgnmak.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/giklgarvb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gfjdmbklf.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gmjlqbpmt.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gkkmrnyzt.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/goynvdzyi.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/ghauttrcg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gxnpkolbo.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gvkencslg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gnxhkcnir.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gswbygpoq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grduewcrp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gqqlmwlse.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gqqqballb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gldlvucds.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gytzrpezf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gsikaefqz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gifnlwaya.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gtfmlrong.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvezcpato.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gimgthqab.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gguqazbev.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gguytdxzn.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gmqmgtlvs.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gutvfddmq.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gsgqezozn.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gtoazbwnc.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gbozhtmoj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gsrsdoaxi.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/golswoqbp.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gcxmjqvzu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gywbjftms.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gkhqsdrnn.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gmgwzrvwl.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gnifkaked.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gubxszocl.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/ghdhqmvsi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gfujmhnvv.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gtexfirju.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gxyzzhzqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gciopucks.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gxkvwgrqp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/guqbmoifg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gbkcfqqeb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gwxhvljpx.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gpsqzrinh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/giegfrcul.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gffdcljnd.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gwcajtzqe.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gpewrjfqp.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtzdrfaek.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gutzxbydk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gabnbwgpq.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/gswkbcapw.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gaupauvvu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gmymsmhlg.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ghcxfpgvx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkskhvemv.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gcvcvcowq.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghixnssak.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/grlxynpkv.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqiwvkeng.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/gfwyizhye.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gnjnydjxn.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/ggyixvael.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gmvxhmymo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gsusrxzzg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/glpxnxwow.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzjrrxoak.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gyvwxgiwx.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gfwtbnjpu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/ggihpdygj.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gsqjygdod.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gxtllcele.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gbbmzowyo.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gmqecpevr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gtmosrspp.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gdqtrmiob.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghamucvud.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gdqjtayiy.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gvqrdwpym.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gjtytcwdh.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gyzmxvval.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/glzrxxmod.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gwdkphits.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gurlhtclw.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/goaaqitlj.sHtML


<!-- 参考信息 -->