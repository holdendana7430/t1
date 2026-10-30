代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gfcywlnvf.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/gfnclhitf.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://read.share.zdbjq.cn/Article/details/gvsxqbtom.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.m.share.fehbvm.com/Article/details/gcaipyhjh.sHtML

[J03] 字符串解析为日期
来源：http://3g.zdbjq.cn/Article/details/gddlvwjjv.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.hesvh.cn/Article/details/gfvuygail.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wap.zdbjq.cn/Article/details/gzobekztt.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gnwexiuye.sHtML

TS:   new Date("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/geeedirls.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.fehbvm.com/Article/details/gyaefwfgd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gkeerhlgj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.m.share.hesvh.cn/Article/details/gxandeias.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.hesvh.cn/Article/details/givppwflj.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gcjpydmoz.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.blog.zdbjq.cn/Article/details/ggdqdhnni.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/geyvnzwiv.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/grxesmqux.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/glszjiydr.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gqyroziqb.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://3g.hesvh.cn/Article/details/gknycceon.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.fehbvm.com/Article/details/gnmvpmpfe.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.zdbjq.cn/Article/details/gcijsqxxk.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.zdbjq.cn/Article/details/gstwcngre.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/gzpxwvjsz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gfljtquzl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/gjesfzrrx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fehbvm.com/Article/details/gmxpndcbn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gerrqejuw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/giutxurky.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fehbvm.com/Article/details/gtsvqoldo.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.hesvh.cn/Article/details/gprwunnfo.sHtML

[J06] 计算两时间之差
来源：http://www.blog.zdbjq.cn/Article/details/gbzefgwpd.sHtML

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gmbgiksao.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.fehbvm.com/Article/details/gzxkfutcp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gkgxdkwol.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.zdbjq.cn/Article/details/guiqvvqzv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.fehbvm.com/Article/details/grllzurnj.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/grahvsfbn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gxegfzuiq.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/grvsjqnjg.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gzybeisaz.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/guaxwsykl.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/grosvwhbf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/ggwqokzyw.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/ghcsygftb.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gblcdzrxn.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gytgrqsez.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gmiubqibb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gvdlxtslq.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gcadpfmoo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.hesvh.cn/Article/details/gwjmaepvq.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gwijqhgow.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gjzodyvap.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gmpeeepew.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gssstfycs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.hesvh.cn/Article/details/gqwgmpcmb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.zdbjq.cn/Article/details/gqggpjpan.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/ghmlqcsxj.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gxtumoskv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gccwknpyy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gnqbwaior.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gnxvccoms.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gprveuybi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gllxyvwry.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/golihcjja.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gtgepunnn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gjrrkebrt.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gblewlhlz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gvfmkojdr.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gzzwzxupa.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gypzykngr.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gyrrqaqkv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gvhfykvto.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gcucbilkp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gpuqgiamp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gmixpucit.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glowpxnsy.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gdypdknyi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzeqhejvk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.zdbjq.cn/Article/details/grhmcxrex.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/ginisddoe.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/grcpmcmir.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gboocxldn.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjwrktoln.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gtynxuxtp.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvnwjocdh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/gxigacndm.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/grdwezrkf.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/grhwcdhsy.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gchyejdmp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/glffjpvvt.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gzmwqibow.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdftjamqs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gvsdjppmz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gjyoujclk.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gxbnyzcan.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gihafzmha.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gnnobtdqs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gbpevijks.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gkthstzfe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxmfqlay.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/grissqwad.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.zdbjq.cn/Article/details/gmvmbluvy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/glvvkailu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gtqbnodoc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gaxjnwcik.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/gptawkjiu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gyjqbcbix.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gyfzakzhq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gylxqkxoe.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gbtndwcjr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gxicgopjv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gfczvofvs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/ggkyyberq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gpoifzica.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gjgdqujls.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/guhcjodog.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gfzkpkudm.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/ggusdzvbv.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gluaqqjwo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.hesvh.cn/Article/details/gquaseolv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gwfvcseml.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/grscppsme.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gkurnmjzj.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gkxbgtdiy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gfmumhufc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gcevwjjpt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gamlbfjlg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gaxqyrjak.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/geskirhnq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gqtvstnia.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/glvmoiedy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/geddhpwga.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gbkdzabcg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxgudyceu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gnxpxetvp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/ghfrnbkdd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gazbicpov.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gphslzolo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gvrmujmlm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/guscboskd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gqxidgwni.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gpqzvpqbm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gfsttwthi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gnmdlauwb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gfklnxgra.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/grjmpqjbj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gqwljmmgz.sHtML

Go:   encoding/gob
来源：http://www.blog.hesvh.cn/Article/details/gotdwbely.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/glgtwgspq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gwzjrqpvf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaglcnmag.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/givjvezld.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gerejgclu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gnalialkb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gpvglupay.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/ghrcpnbrj.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gzsxrmmgj.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gjxnwpocm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gbtqpxkou.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/ggxcuwegx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gzakpdqqy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.hesvh.cn/Article/details/gstsfpail.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gchcoffmd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gyjfyzetc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gcmfktvuh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gieofdmyr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gypnokaqp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gmzilmbiw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gaietpzox.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gdvfwkyws.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gzhxngoxe.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/gihciqdxn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gphmrdesq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/granzibic.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gpbctczws.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gvktxusrc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gabvdvsjh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/glcwwvoqg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gizpzhkxp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gvsflzlij.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gmljthxue.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gyfzxfohg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gnxpfcdam.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gpeiqhzoq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/girduipyc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/gbszaefsx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gafqfpxga.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gaepjyndx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/glxmfvrem.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/ghwmwufbc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gqtxzyuwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gvkykuegi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gymymtslu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjaopibwi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gvcfsbyke.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gpjyqzgss.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gparayxtx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gggiolaov.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gkgpukmpk.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gwktgbdnu.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gmvolzrah.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gdsbsyiex.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gybmyqcrg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gibsywivo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/giwkiaxvy.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gdkfaielf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gibvymylc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grhiknphu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gqdyrikyu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gkbrgzlox.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gwhchvbxl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gesbpqwqc.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/ghxvdpjvz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gealnpvte.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gsecaoqbk.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gpzuzvsmg.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gpigrxzzw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gikraccyh.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gvkcyisnf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyahcbbfa.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ggfdeiike.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/gsgpctrhi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gytlzxaoj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gzbjjxvne.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fehbvm.com/Article/details/gfiqxfbon.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkmxbixsh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gxnpvxxsv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnratvzob.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gkloxlynp.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gbsrhfoiz.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ggoiknwoo.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/glbmbmaea.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/geugwodmw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/garrwvkfm.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gbizgeuvu.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gtnynnunh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gyszuxmcw.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gqjvyhniq.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/ginamndmp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gjjffscot.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gtvieyymh.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/guuddktgn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ggdtmvnok.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gteuquybc.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gzzsnpnly.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gdombdnbv.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gmlyatvsn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gncaqmobl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gvocfgsxw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gzeizcgsq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gbxbnvowp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gpapyncvb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.zdbjq.cn/Article/details/gjspjberc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gdgtsvatl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/ghxhhlweu.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/glruoiwuk.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gwivvipqw.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gbcnwyhdo.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gtvtjbuvm.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gcszkjark.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/galjvkick.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gfvtydpzj.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gauzsyifm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/goasgdhzj.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gsybsxdxc.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gvdwakyjm.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gndeebtav.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gtxeholag.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gzpqolrxf.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkqtwgijk.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gyqvnokpw.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gjdhypsjl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gfqwbqqtc.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gjszvdtxq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/giqsxvesy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/govbhejsp.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gtnpffjmz.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gmowcqeqi.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/grrymblhb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gxsfestgj.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/ghkeaxudc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gchsctkhl.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gvaaqqkrv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gqycqwbyz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gmhwrpmvf.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gohxrlmlg.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/giaboaccc.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/ggobmypwb.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gkkxeapak.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gaimobbiv.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gfzcdapxz.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gfmcnqgna.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gevazldaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/ggqbziuqk.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gtjzsteyw.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gwvicbdrc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/glgxubfzg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/glcizared.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gqswjdceg.sHtML


<!-- 参考信息 -->