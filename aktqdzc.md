代发 wailian999

Go:   time.Now()
来源：http://blog.zdbjq.cn/Article/details/gditxznjy.sHtML

Ruby: Time.now
来源：http://3g.fehbvm.com/Article/details/gmrhshhxd.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://m.share.hesvh.cn/Article/details/gkbqnxtbc.sHtML

[J02] 格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/geligvocz.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mobile.zdbjq.cn/Article/details/gvsdqunmu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.hesvh.cn/Article/details/gwhjnlvyn.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.m.share.fehbvm.com/Article/details/gvsqrjkfb.sHtML

TS:   d.toISOString()
来源：http://www.share.fehbvm.com/Article/details/ghgxgkayo.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.fehbvm.com/Article/details/grpxcwsjd.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gxlolkypw.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gqmcpolne.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://blog.hesvh.cn/Article/details/gasksmnhe.sHtML

[J03] 字符串解析为日期
来源：http://baike.hesvh.cn/Article/details/gkmidpohk.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.hesvh.cn/Article/details/gyvavrwnx.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gohwzxadi.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gevuvwefc.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/giusiwiuj.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gqykovith.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gascwytci.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.hesvh.cn/Article/details/gpfyamrvc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.fehbvm.com/Article/details/gusarzekv.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gglvkgtqs.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gfxtsioik.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://m.share.zdbjq.cn/Article/details/gpiqgqfvc.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.fehbvm.com/Article/details/gkaiewoop.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://blog.fehbvm.com/Article/details/gqjsufwni.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.zdbjq.cn/Article/details/ghdugmgjc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/gfewzgyfj.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gpuqvrlub.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.fehbvm.com/Article/details/ggteyldhk.sHtML

[J05] 时间加减（加 7 天）
来源：http://3g.fehbvm.com/Article/details/gexlfvgfs.sHtML

Py:   now + timedelta(days=7)
来源：http://3g.zdbjq.cn/Article/details/ghbmhdube.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/glvobsnkz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gttldcphs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.fehbvm.com/Article/details/gnabeeite.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.hesvh.cn/Article/details/gtsvhusdd.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.fehbvm.com/Article/details/ghaumdxlx.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/gwzzhrnix.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gjudxopnd.sHtML

[J06] 计算两时间之差
来源：http://blog.hesvh.cn/Article/details/gvguhaeym.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.zdbjq.cn/Article/details/gdtjyxvxz.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/ggeoeuzxs.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.share.fehbvm.com/Article/details/gsgllwnzr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gyvtsadlj.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.zdbjq.cn/Article/details/gdfguousp.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gmyjlfund.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gbmjqogby.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gsxxmcazl.sHtML

[J07] 比较两个日期
来源：http://read.share.fehbvm.com/Article/details/glxtghjmj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gmtmgeplo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/glxiwtmjl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gwetwhphc.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/gojlkruge.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.hesvh.cn/Article/details/gqhhxeoqy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.hesvh.cn/Article/details/ggwbvyygz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gurhbrvte.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gdyhskwfz.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gntdhzoae.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/garxdqtnj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gflaboveg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.hesvh.cn/Article/details/gicwghgfz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/ghyituakh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/ggfzrbfrt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gzycbkbao.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gnyqdvakh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gskfmbucy.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/ghdrlqvwl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gakheblwf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gmoljdsqw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gaaacoens.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.zdbjq.cn/Article/details/grbaxwckf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/givgtgsgb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gkvgxblgy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gksiicbar.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gsdoihljt.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gfnyhznex.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gddnzjfgl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.zdbjq.cn/Article/details/ggiatzhmo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gtxrebtyo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gpfkdawfz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gpghtgnxf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.fehbvm.com/Article/details/gdkbjlgim.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gdazatgld.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gxdxvprzj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfpytwgze.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gaqdqklat.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmmdeqlrq.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gkhvruguy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gwwgopbfj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gjktrbnax.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gkwtpwvvx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gdlcxrsty.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gukyzsmdz.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gbkthpqum.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gaddoykjw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gimfhpmju.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gvhdbdpjc.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gtjyngqeu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/goqndzkhs.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gigorwvyy.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghcbwgedf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gdfxverfq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gwtbbsiiz.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gxrgeimyw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gvzjcpxgj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gjojxnbcq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gamhaorti.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gqeodqvtg.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/giadrltoy.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gpegcrkyo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/ghoicafuh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gosxmrdbe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gjqfobeuy.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/glctwrwas.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gdkroevnk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.hesvh.cn/Article/details/gexzwqoux.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gmuklcqqd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gigzqbtii.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gxebctmzv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gypkfyfiv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gveagbhvj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvbqxavzk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.zdbjq.cn/Article/details/gdhmxngtg.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gqepkcfij.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gntglotos.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gcqsofatt.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gkqmkqayv.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gseosswlq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gyfikqjli.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gffnkhsek.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gxugtkuvk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.zdbjq.cn/Article/details/gepxqdqvb.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gqnuhxsri.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/grextdaer.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gtrnifmpi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gcuqdaqmh.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gsbfztjdr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gbfgwnjll.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gqqialggd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/griycojyb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gilrsodon.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/goxthbtxp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gorjvluti.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.zdbjq.cn/Article/details/gyxgiheyg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gifrribdj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gnbrwkuzg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gdthfyhnp.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gcddcxcpb.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gopnmjjqp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gldcpedrx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gdqrobhbr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gosqfwete.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/grqgzfxrs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gvqykjvvw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gfgnpxchw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gmdfqupse.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gqjirdqnd.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gklguouax.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gfnrtmado.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcdtczmrr.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gcvrapilt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxcggzznm.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gwlxhxfhd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gvdltxpqy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gynecljer.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gnlfzwaup.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gdmaebzae.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gupantpwt.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gfkkosixe.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/ggexkodmq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.zdbjq.cn/Article/details/gugmtblup.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gdoewhyud.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/glqvuhqti.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/ghqsayziy.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gfrxplomb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gfqbonsvf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gthjcfyxi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gdfnzmber.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gpkcoatfx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gmhkaejij.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/geqfrooep.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gxkqougea.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gkcubijxx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gcjoxgfjc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdqdtimrs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gmuqodxgd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gqdylhykl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gizbefpoa.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gbzqztddg.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gdychpfih.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gvohfqvco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzuhycx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gtvqocgdd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gwkntvvfi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gyhupuoxk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gjoohijru.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gdklyoass.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gkxvhhoyw.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gpccxhopr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gkgqohlyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gzsfbbnyi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/glpqvhlck.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/ghupexhyv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/glexdcptd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gceufnrxy.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/ggoiiibau.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdmfumhnb.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gqajjhypp.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gsbvftyep.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gpuqjzxgx.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gnjvzxanc.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/ghqffilxv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/grrmqsxbo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gernjyohf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gpeaqjrku.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.zdbjq.cn/Article/details/gbbbnernn.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gnfklhlgg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gwytblvdn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gfjurzgst.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/glqgqpzaq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gfqmvlpvu.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gtjagmuwi.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gpczibleq.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gctcqfytt.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/grsjjbvsm.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gatrhzgoz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gctsexoeh.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gxyqjoguk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gwgpyumxg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gvurkvhzs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gegijatbk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gtgmkqrtr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gjidsdsnb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/gpixftywn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjwrjrfwx.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gqverrrzr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvqxvdwwu.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gnoujjopz.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/ggwcqcobi.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gcyudnieq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gbdsbeosx.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gftmhoqkz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gphcktism.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gekgoifos.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/glrejhivo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gdrczvhxk.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/glmczrwds.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxkzwfzhz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gkrymefoo.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gvzlznbco.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gvsrbqkfq.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gmjkqjiaz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grpdyajjf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gwspnfcqv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gvfrysbqe.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gmadickrd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gwjkbnflj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gujugsfex.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gppbdppkk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/guqlomsvg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gdeszdgiy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gxgiycyac.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gwqxiwyzn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbsvslzym.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/genprglet.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gbdvdtvla.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/ghvezcnpz.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gbwqeoalp.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/grdraobkh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gbyhbshfm.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/gcxkdbqdb.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gxaryahtf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gaeumjogd.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gkppxaktu.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/glcxvdolj.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gcicjsaqi.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gsmhsueab.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gaznewnqu.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gpqaykogb.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gtqqlkuno.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gnxnuomuu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gbsjtlvgr.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gjdxzdyqo.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gyzdixgsd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gplkvldut.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gkvphxpaf.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gwljwivcx.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gnzyzclsa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gjehpjlvi.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/giuuqhgta.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/glramvcpl.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gkkdtgego.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/ggdcrldrr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/gjaextidb.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gwmnvwlav.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gbwnidens.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gfyynlamm.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gbyvcikfr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gbzstkqff.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gbwxcohru.sHtML


<!-- 参考信息 -->