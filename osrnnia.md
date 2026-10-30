代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gnlvkwctp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://read.share.fehbvm.com/Article/details/grulsgkcz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gvzacsyat.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/gcvtydvkx.sHtML

[J03] 字符串解析为日期
来源：http://www.blog.zdbjq.cn/Article/details/gknzpspaw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.m.share.hesvh.cn/Article/details/gmkxjatom.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.hesvh.cn/Article/details/gsmnrkgvm.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gigkjgflq.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gnxqvtgmy.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gksyvnwxs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/ggidvpylh.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gogcauykc.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gpnmwzcum.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gtbmyzjua.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/glpggajgr.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.m.share.fehbvm.com/Article/details/gbzpjlqgw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.fehbvm.com/Article/details/gwthhnkxd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.hesvh.cn/Article/details/gigazoaba.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/ggcudglbh.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.zdbjq.cn/Article/details/gjikpdujt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.zdbjq.cn/Article/details/ginxjpjkf.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gfoiotgsa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gxjgktgqs.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gitjwnroe.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.hesvh.cn/Article/details/gblsohydk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/glahyfoxe.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.blog.zdbjq.cn/Article/details/gayhfgqrg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/gxznediuh.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/grebzbrov.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/geexmnwyy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/gnesyfyzs.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gngqnhiwx.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gljmwtwpk.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/gankotmye.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.zdbjq.cn/Article/details/gakxfohdd.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.hesvh.cn/Article/details/gsbsmrwye.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gdcrtzdrb.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/gdddejkoz.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/ginehzwyg.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/grmuhtdyk.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gekwqxcdg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gvyphiwfj.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.fehbvm.com/Article/details/gsmraesfo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.fehbvm.com/Article/details/gwdqqmqnd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gwclhlcnp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.hesvh.cn/Article/details/gyjltaoko.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gjbpnkqgj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.hesvh.cn/Article/details/gedxdefal.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gnlosfdyj.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gqkkezglf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gbbriamge.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gdsdhcdyz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/ghewvqmpm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/giavldxau.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gegdefmse.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gvlttehur.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gbhyyjsfj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/goaeagimk.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gzfvfjbpc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gnhwbzdsi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gxjdibqbx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/gdddpobku.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/ggpocxjtu.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gdeyiobyw.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gdjqpcxws.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gewpocwpo.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/glwnkiwte.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gfeueqwmx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/ggpyhfmzx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gcaymeonr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gkoszwmgk.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gjhtugrjl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gbcofknar.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gdlsufdfm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gtvgqaqwi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gessqskuh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glmhrsszz.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/gymkokjdz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwlsqergi.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/giaxoibou.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gamgzaeum.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gxbmuguyq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfzxoqlja.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gjcnlrvdp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gmmnmpkaq.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gdjatohai.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/ghindszcp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gpwjrfmlt.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gknocyuhq.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gimaoyhot.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gjbraiswp.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtflticho.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gijguhbth.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/ghkmvexli.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gtntiqitt.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gsnylgeup.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gojmiawld.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/ggwhftzhz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fehbvm.com/Article/details/gtuvrffzv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gonsbsifj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gvrsvrjdn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/guzxdwjsz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdgdfyetc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/ggpnaglfr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gtiqrovbd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/gfonvadjv.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gppemqgjp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gamljhazz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gjjhmlzjw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gaklepqxd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gdkliosud.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gppspbqtp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gjgyjpmvi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gjzasvkwp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/glafyfrym.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gsqfyqony.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gyodaqgdi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gkzpefmic.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjjaxzboi.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gwunrhrle.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gwvyyuiwx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gkfrrqmvc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/glfookcww.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gjbuuqxan.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gxcuubozn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gbybmgkcg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gtsynpkgn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gohgmzhdx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gypkidbjz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gieazfzel.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gcekvmmwu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdsrvbtep.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gxwautizu.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gzsrtycrk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gzaqvlfpj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/ghwyisuvw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gfqbmhdhw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gsqfjwbcp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gfqswjjzs.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gmwsvqnkz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/ghoiqerfn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gxucgjpvg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/grapyfygu.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/ggaradcgr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gusbrcdsv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gtbsrwmad.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gvtyiwinr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gcohifmzo.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gkegmscsr.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gjtvuxjde.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gwnqlfpim.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmxzklpqk.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gqkgabjsq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsewzxwub.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gddnwhdhz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gypurlpjj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gewrdgzzm.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/goxgyyssx.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gzjmvhgrg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gloekoigl.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gsxhoevhi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/giicyrrlu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gdmqkmsfv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gsjkytilk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/glfuyptbw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gakojbyrj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/glvdczrag.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvalmqfff.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gnzmsympx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gqkthblzv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/grviswust.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gikqkceqd.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gbbeuligz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gjnyoesvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gnzzzthmp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gqzngynwz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gybfzhjkt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gyeoxhsad.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjnbzgieq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwjnyog.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gcmarosyd.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gmqntqxpb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gdycpbycw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gafkeekdf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gxmaagiye.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gmfoxuprg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gkemcgqkd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gsxfmaxgx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gkajixbwt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gkapwcbxw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/ggiwqgfop.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/geooajagg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gygnyryaf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/glihkrydc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gdkojdicy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gjutjexwo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gkywrdksl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gwwjscxtu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtfcpfjqt.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gwnrbskrt.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gmfkdkjlc.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/ghxmuwdzq.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gvtzubcyj.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gcqvzwkup.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/giyxrvjsb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/genlmrhkw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gkuucvrzz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gnmvcdzmg.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/ggnlzprny.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gvhompugf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhkeivup.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/guioifwha.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwiamuouz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gokpeumdh.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gudtsnebk.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/groimsxbz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gilhhegdf.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gzvszjqgy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gxbrpcgpp.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gwdcugvjj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/ghkoflcqn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gditgbrto.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/gsiyyzrrh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gwnwlupsd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gpazdrtof.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gygzrhplb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gaaerboch.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gbwyolvgo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdneqmglc.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gjprolyks.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grahqoeuf.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.fehbvm.com/Article/details/gqpxhukoo.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gqsdyusii.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gsshgtpfm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/ghqqsdhln.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gskswtnlb.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gvmjqbvbx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/ghntqaofl.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gpjpevbvj.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcyggmsto.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gulcrvcnm.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gjihmisxe.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gwqdyamkf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gaauhlodj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/grvlqijzq.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gcsvymwfc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpoldxhef.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gobsrgxsd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gqhnrrjxw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gooqbbfmj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gzxxkihfp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/greajfpta.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/ghetnosxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gjflhaalr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gyplqzjrg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gtmayzxsb.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gysmnazke.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gdxqbkwkh.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gqrujvwsa.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsuxlntsz.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ghyvybvmw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gwbesdlzk.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gtjbzkmsw.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/ghdlaoeyt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gzvvfpnmf.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/ggevgsuem.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gzgzkbwbl.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gdvagahyg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpwtyvrct.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gswahmaju.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwrxukjnq.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ggdwfvvvi.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ghwjaufum.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gkqjxluuv.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/gcnclznnu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gtgyxpvek.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gawknoict.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gwyrrvxrt.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gzejkpvne.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/grjuatknr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/gaqzqfiit.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gqvxgrkfd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gwewojjfh.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ggjjfptnn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/guowbgnwb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gfcpfigxq.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gwvmhxuni.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gorhhfwfj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gjetvpvvl.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gcmexfqnv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gjnhaglrc.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gsfwbwxeg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gkiumjvzn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gsuffcdpb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gespmxdpo.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gzysjfxcl.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/grnppgfry.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/giggkidti.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gtimkgqcv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gxtndlboz.sHtML


<!-- 参考信息 -->