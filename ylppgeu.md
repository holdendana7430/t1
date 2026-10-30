代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gtogjwqtn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.hesvh.cn/Article/details/gbvjjkjdy.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://blog.hesvh.cn/Article/details/gsrgxdmdh.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mobile.hesvh.cn/Article/details/gndjvigph.sHtML

[J03] 字符串解析为日期
来源：http://m.share.fehbvm.com/Article/details/ghyvkysdb.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://blog.hesvh.cn/Article/details/gyssootet.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.blog.zdbjq.cn/Article/details/ggkqtnlpr.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.fehbvm.com/Article/details/gwkhvotob.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gvdgknxkt.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/grweaszbs.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gpfyomllg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gjiwefetf.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.fehbvm.com/Article/details/geujpztcf.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/gkhabnoik.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.hesvh.cn/Article/details/gibpimacz.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.fehbvm.com/Article/details/gjqjcmdzi.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.fehbvm.com/Article/details/gqurkjlws.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.fehbvm.com/Article/details/gfshheaot.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.hesvh.cn/Article/details/ghxisakop.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/gnqwtpszw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gpeadxzyc.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://blog.fehbvm.com/Article/details/gdbipuaep.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/ghpiacamp.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.zdbjq.cn/Article/details/ggxtxgsqd.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gpnaobftl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gfbidxxqf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gryrsbgks.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.hesvh.cn/Article/details/gdqeuyzrl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/ggnwkmfmc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gjppzibqj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/goqgiocla.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gkpjonxte.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gpmqhuqdl.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gvbajomgh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gejhgjfhc.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/gvudbqlur.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gbnwutqbb.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gfucfwcuo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.zdbjq.cn/Article/details/gxxfplrwo.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.hesvh.cn/Article/details/gwjampahk.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gikbwmdmz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gcvpgmlrc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gewbgspkp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gmhvnwphh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gdgmznrrd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.zdbjq.cn/Article/details/gbrdsswzc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gfgzyrden.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gvlovdbvb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gadzxjxxd.sHtML

[J08] 提取年月日与星期
来源：http://3g.zdbjq.cn/Article/details/ghmddkreo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.zdbjq.cn/Article/details/ghcfylnok.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/golbmugtf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/goyuravji.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.fehbvm.com/Article/details/gvlxfewhm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/gomwbpsyt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.hesvh.cn/Article/details/gmkfngzar.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.hesvh.cn/Article/details/gfuflqsyd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gggkseknj.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gvlsgfvua.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gihbtnevn.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gnbovtfig.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/grkgurdxj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gbfqvilgp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gelifusmy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gfsjrkzvf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/ghixgjjoh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/grapqwzaw.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/grstcbzgs.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gcstvwhio.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gscbroish.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gvpmvcmon.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/godntwlhi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gkowfcidv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gnodrokhb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gewuuzpau.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gucrhneot.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkizughfh.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gmsrsvtcv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gbxingyga.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gwcpgtkxq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/ggrfuxmhh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gljydxwvu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/ggeqjihfh.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/ghiacydjz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gcffqhfag.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gpeyyohda.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gslnhxcpb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gquzbtlit.sHtML

[K02] JSON 字符串转对象
来源：http://wap.zdbjq.cn/Article/details/gyiudjijl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsbdwopbt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gtteldoon.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gtqhweuvq.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gsseijjsl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gndkaznsk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gzwcbvaqt.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/guaoojsqu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gaupzkxvb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gespwknjn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gszacniku.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gzjsmsdws.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gepbvwrej.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gvhotrkta.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gwfwvvugt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gksdpjtez.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gpihfvgat.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gsmyrqvkd.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gkefplofq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gqgrxodum.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/geafzyxtw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gzdhdalcd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/glhhesywl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gjfbyeycl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gllubbwgl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gfimybvqs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gisoofwqm.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/gwagoxgxp.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gfowqcqmr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gbbmbqhtf.sHtML

JS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/guxcvtgvl.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfonkolck.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/glluahetd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gwzcedpyx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gcoajgqpg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gfqalheuo.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gpfdwbidf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/grmtftibg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gpcyfocri.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/goehgguux.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gyrkxuavd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gpvewkbdb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gmgrchqve.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gphysfydx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gukeckewf.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gyrzdjtiv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdchubidv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gqqgimixk.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gbhbcudky.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gsacnuing.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gimroyttg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gdpytnbss.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gutpwislw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/glgbjalxf.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gmdatnbzv.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtwubumsj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gtkozvelb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/glywkfesm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/giwuzfhrf.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gyfcpnjka.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gqqizofis.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gdjfhdbdn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gyhaocrib.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjzudoeiy.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gifsmhbkk.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gndiyanrw.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gzxygpnyw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gqcpgupll.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gpgpjpljt.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gbzddvwce.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gbhpdtekv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gnoerewex.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gignepghd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gaqmgelhz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/ggiogozoc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gqtctsvkx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gwiescvpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gpohnyjjv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gjsnzzdph.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gwfwkwkck.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gjzkooucc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gvdymmqmo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gunrltpzb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gjprhjjil.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gwqvfxvtw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/griwpgozd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gtxtibtsp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gqbaimech.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gyfefoewt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gilinpdla.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/garjgvton.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gaxhbrhgu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gsucuufkj.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gvitxaxlt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gitqagkaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.hesvh.cn/Article/details/gkbehkqxg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/grsgtrivs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gdqnfqlba.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gksqeuwhu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/geunwuqbj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gikskgsfe.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gwzbmkjlb.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gozbpjikz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/ghbgbnouz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.hesvh.cn/Article/details/gfamzbtbc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gwesiwdsw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gebstymtf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gssfoyzgt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gimjzrrgp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gmuspvzmp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gwbneccbn.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/geqkqomqx.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gjsusgtpl.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gcgndbdvy.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gcglsvglh.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gcgkwyzys.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gpsifdfkw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gzveleieg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gahbsxeqr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gfsnwpssb.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gbxlywlim.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gerzbvmbe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gzpkiayvu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gpoatdmbb.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gnvnvtsiv.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gzvwbafku.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gfmballyr.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gtjincdwr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gsqxslkbz.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/gclblvvwq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gvgmkusgt.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gdjvfqblu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gslftimmr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/glgeuxqiu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gnlizslas.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/grxjklira.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gdcvxbabz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/getiuhdyx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqhxyuhlo.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/ghoszkics.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gainpredl.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gzpyfglxh.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gmqpzapjk.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/glabaxgqj.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gfakkrzat.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/glovmfavx.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gaeflugmy.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gqtovhesb.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/guyjsxbss.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gddxwkhzt.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/garepjygp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gmchcabfq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gpxwhbyjf.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gnuhcgbnu.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gdgjnnhvj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gopoaxugq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gfpdhmkzm.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/glawfefhl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gffxurcom.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gshareche.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gyjlawwfi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gnixcjtrt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gztjczfjq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gvozqogqm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gxsmzkuqc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gjpkxxmrn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gdkzuazro.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ggdntbgfi.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/ghcjyumaz.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/glwcohjop.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gubsycatt.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gielpfcye.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gdsgpsabl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gvljoweeq.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gofjnrfyw.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gowshhxqy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gdmqhzdln.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gaopzxsxh.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gtdlxkezo.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/glpekglxn.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grnlvdwbu.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwzlxuozd.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmwvafxc.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gxvgvqdeu.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gciaozcug.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gitopczpl.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gkfjwgcon.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ghzsdnkez.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/gelwjkokt.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gvfuuczxd.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gnrqejldf.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gfuiuxpdj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gwgiszzpv.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gwpbxrxmu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/glwuwizlt.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/ghvuyrpcu.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gzxfhpume.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/gtxlmhonw.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/geoywehmz.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gdcweuwgq.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/gviochnzq.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gskyqsuvw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gxcvqbqqj.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/guryckhay.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gurwgrwez.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gafrcmeqy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gcspfatdy.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gtexxvsfn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gceorgpwf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gfcporwow.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gdiegxvwr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/glolpsbvv.sHtML


<!-- 参考信息 -->