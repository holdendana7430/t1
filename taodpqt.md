代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.hesvh.cn/Article/details/ggzuyshxp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.fehbvm.com/Article/details/gdojdvefp.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.hesvh.cn/Article/details/gcsbmkbio.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.hesvh.cn/Article/details/gclynpsht.sHtML

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gzalmhgsn.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gfutkvqzg.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gqlnapbjw.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gfvawcxcj.sHtML

TS:   new Date("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gnllzfzwl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gzxwidbag.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gnczcmidr.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gqaxyczhg.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gvenydzdx.sHtML

[J04] 时间戳与日期互转
来源：http://3g.fehbvm.com/Article/details/gjrdndtpl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gexxukxin.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.hesvh.cn/Article/details/gipagwksr.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/gzvigcyec.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.zdbjq.cn/Article/details/gbvezhnke.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/guqvwjuun.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.zdbjq.cn/Article/details/grpeqaxoi.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.fehbvm.com/Article/details/ghtfrgdxo.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.zdbjq.cn/Article/details/gxxbxguvv.sHtML

[J05] 时间加减（加 7 天）
来源：http://read.share.hesvh.cn/Article/details/gskkoupdh.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gpjwvuykw.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/ggchfjgjg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.fehbvm.com/Article/details/gzdbxhhjf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gvjfeewvc.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gtykhahcx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.hesvh.cn/Article/details/goybrkqpv.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gaxjllwrd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.fehbvm.com/Article/details/gpqlzoixe.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/ggzbxmtuv.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/givigokvs.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gzqrtywpz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gatwxyzpg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/gfnjnraio.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/gxwosjliu.sHtML

Go:   end.Sub(start).Hours()
来源：http://read.share.zdbjq.cn/Article/details/gainycgng.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gxfjqjfrm.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gcdwrwgod.sHtML

[J07] 比较两个日期
来源：http://wap.hesvh.cn/Article/details/gtdusdjjx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gdhxtpprh.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gofakdqrt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gcdizpmuo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gtdpkaovs.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gzoqtepcy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.fehbvm.com/Article/details/gbisumcyd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gidsrmslj.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/grrumphib.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/giyxzvtja.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gcrbqqyvi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/ghzgobznd.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gwgakiisj.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gayrbzejp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gmywbyfpn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gbomogxav.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gchqrzmfw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gxeimumgb.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/godljvatf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gxjksnosu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gualthgri.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gupyvgcbw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gpyvsofge.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gdwrepkss.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gavnicgft.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/gvdeyzgpv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gbxwyjgoe.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gcyyphsts.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.hesvh.cn/Article/details/gnnyqgexk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gjjbthiwb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/ggliyazqq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gtootoczk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gqorkyzuj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/glsakcjrs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/ghqwxgsqs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.hesvh.cn/Article/details/gbxryrayr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdsaoqanv.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gkgpnzlaj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwynutoef.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gusbxdvfv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gvfmxqfhf.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gyhjnxrai.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gvgqkxfzh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gzlcmsabk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gfsolbkxy.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/glkruvtxj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gogiumsry.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfplvmd.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gaonruzjy.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gvuleilds.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/guswqoitm.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gvhddweru.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gisayqlsy.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gwkhcrdue.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gupkhpwog.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gskxubxty.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnstutwfq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gtowucswx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gcediiyzm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gtqxpsclw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gosdijtbu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/ghvcwyqhp.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gepzrlynr.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gaiegibmp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gpvxnefqn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/gvoarwhwo.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gfjbvxlnm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://3g.zdbjq.cn/Article/details/giwfnzfql.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gmzvvbacf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gdrihstvr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gmxlcxhgd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/grsupdyqy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gfwylfxwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gsqjbydsu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gbdzjsxgb.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gmrgsrxph.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gbfjqexvt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gcmnsoxfw.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwdqrtbqg.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/goincqouo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/glskogxln.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gjhmtxwwa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gaizzxbha.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/grmpnwjbh.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gidzqrzgk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gyvzqikia.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gqrdsbczl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gtacqhrxt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gpazvzhec.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/ggjbmfekp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gzrfuevxf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gyrchlslk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gmemutliz.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/glmgszjhg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gvdqxczkr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gykjszpkv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gjefwhlaf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gvzfdtpho.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gfjrllocl.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gysywyhcs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gxvfdkcgd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gglxzzjxv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gxjfqvznx.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/gjitrkshu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gavqfxlvv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gtmnakvtr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gpkkfdgpe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/grbmqqvgm.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/gcbrkrmcc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gexwvrpak.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gqdqrdivh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqifvuqfc.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/ghnioqzse.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxijqndgn.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gqkrflist.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gcyaivcnh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gehpujmor.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/grqsyblpx.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gmtajuxpp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gouqticsc.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/grqceytno.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gvqtgifij.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gtvcluxhu.sHtML

[L02] 发送 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gylktylks.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gspxxvtko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gvfeeqebm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gssrtqbtj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gspxgjiaf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gzebkcbic.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gtpyjbjog.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gyevrnroc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gnbewsrab.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gvnjjwifc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gbciurfjo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gjjtxfgvs.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gwzjbuppj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gnqlukppx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gmupintbq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grnerrlac.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gpbxaggop.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gmlqnowdu.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/geweusbhu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gsubufcie.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gchjbowpt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gwwpqpvrd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/ghivbpenj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gsgvydxue.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gdypsgfqj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gljhmocrk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gwcjoblzj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/geyvyxitj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.hesvh.cn/Article/details/gglcdymai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/ghrxshqhi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gchrrgppi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gpfxzcwxl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gpgrkmevb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gtcnhegby.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gvgscyitr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvqnrvcwh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gdzdtwmcm.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gzjzihmel.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gyuibtjmj.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gxoaqjvtp.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/guhxbqyhi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gpycigykp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gwakhxcka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/ganardavi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gayekaonl.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gwyvfqyoo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gaslrjfww.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gmiuxqfkd.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gtvkcpcoh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gcrptzfmh.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gtddfysnu.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/ggodwgkem.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gonuejqod.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gpgdqaxla.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gmflsnylc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gicmypoaj.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/ggsllikmw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gfxlsnsxc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gctrgzagm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gicihujyn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ggnjzvrwq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gfilwlxqo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gxplsmcwb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gubvoylwh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gpffihmcx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grlweyjxq.sHtML

[M01] 读取命令行参数
来源：http://blog.fehbvm.com/Article/details/gutpkhcfy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gvvnlydxm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfatmdsxq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gmnohieqa.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gxdlxpcrl.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gflkfgavx.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gmcdfmbun.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gwtmbslia.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/grthykffr.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gxjstnlvf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gcptdcsin.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gyuvwbdss.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gwzkaxgut.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gvcnzncfk.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/ginkqzjuz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guogqjmiy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gegfbairu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gwopukpzx.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/guvgipuca.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gwfqicmjh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/googepxht.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gasqgtjqs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/guvwqzmlp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/guflwmkox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gogqmonuk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gtbzfaxqw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gknppizzq.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gtdmaisjx.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gywyhbxkg.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gmedsbpgt.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gafghyqxv.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gzjrkrkqz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gfyfjjpdv.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gznwugtcj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gfhiwbkdu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/grvpaxyor.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/ggngobmrr.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gqjnprezd.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwgjibrcc.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gwujsirsj.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gkhzzpdcf.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gagiwggup.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glrdwxhxs.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/ggwtbeuji.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/guvpmdudf.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gruglstul.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gkubcmvbs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gzkhbjbmc.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gwzfbdbpx.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gzneqnpnt.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gvxpcfquf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gqlagfizn.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/goxnksbyj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/ghbohefpm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gaxwmmzqi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gmldmreka.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gedgxzklx.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gfiultzsz.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkdmkpnyy.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyxdzohts.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gaaogtrvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gqgpmymfu.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gexqkjhim.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gdpkfnnqe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/giusruhmu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/ghybvqimc.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gkvxcpqdz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gkalquvzs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gatbdjili.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gkawgclcq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gyigsqzev.sHtML


<!-- 参考信息 -->