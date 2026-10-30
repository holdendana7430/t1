代发 wailian999

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gyiexwytd.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://read.share.fehbvm.com/Article/details/gbjawgwcs.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gbelqhypz.sHtML

JS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gkimdduiz.sHtML

TS:   new Date("2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gllugixgn.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gdhkfexji.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gvyflsucj.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/glzbefrbb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.hesvh.cn/Article/details/gltflzyzg.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.zdbjq.cn/Article/details/griaxsbrf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://baike.fehbvm.com/Article/details/gqzgezchb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.zdbjq.cn/Article/details/gmjebddtk.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mobile.zdbjq.cn/Article/details/guojcxflb.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/gzunwmatb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://m.share.hesvh.cn/Article/details/gkmixjstd.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.zdbjq.cn/Article/details/gajajftcw.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmtxclco.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gqrurjser.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.hesvh.cn/Article/details/gpavvtbwm.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/glgnlqbps.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gqxhunhae.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gzcomszmq.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.fehbvm.com/Article/details/ghltmgttg.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://mobile.hesvh.cn/Article/details/gngvyuxfw.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gjrrtcdrp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.fehbvm.com/Article/details/gjivzrxyj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/ghpnrdnrj.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gfgtbqyth.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/glbnkkafo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gwhzuxzmp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.zdbjq.cn/Article/details/gviwsyptf.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/ghkfvjioo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gkzdzdjbf.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gecemwigo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.zdbjq.cn/Article/details/glbsjghke.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gnhzjeqqf.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gexdxikvu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gociomkcq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gntguqsnv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gacdofnzp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/gezpgweyi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gkmycxtfj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.hesvh.cn/Article/details/gfqfhmtjr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gfzpxhjhu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gioxyueuw.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gxodvvgvx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gnbvbkeax.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.zdbjq.cn/Article/details/gbhtiavod.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gliaxhnul.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.blog.zdbjq.cn/Article/details/gjmtjkuyq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gjirywnci.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gdydojcqs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gilwmdaus.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gfoamljyu.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gtcybybuj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.zdbjq.cn/Article/details/gwvpewchz.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gsakixpkw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/ghyprivvw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gjjprprqx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gjrthngyy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gvgxqhfso.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gxkispsey.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gadkcrbib.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gdcayuqww.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gnlqduqgs.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/getkfaxdr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gnngcyzxp.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxqatqhy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gcqtxzagm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gdtoxerwz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gjagvejqp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gckzfxbfc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grbjimrkl.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gscwzheyy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfvbdxrza.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gagfdtnmb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gmqntdant.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gwcnezlep.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gcsbtibbr.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gjuoqeuva.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gwvsrjkbm.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.hesvh.cn/Article/details/gffgwrwcn.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.zdbjq.cn/Article/details/gwwjucmil.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gofhbfdri.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gnozvvlxc.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gehterlft.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/ggbptuvvh.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gunduafvx.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gdkestyqs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gdalmklmo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gwzfkhjuy.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gklvozbjx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gpgsiwulk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gfrgwfofa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/gqntsmhiz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/ghegziqoq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtsytvrjn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gdlkffzef.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gcpduizto.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/ggjnmocic.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfrnrxykf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gpavoqqdz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/glzyacixk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gsydnnniz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/gfyrbwvoa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gfedglhal.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/grueuuupf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gvsaaglof.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gxkvbjcvu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gnmhwbwvx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gqobaywbc.sHtML

[K05] 深拷贝对象
来源：http://3g.fehbvm.com/Article/details/gtmzwjbee.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gtymghtza.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gomkzpyfb.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/glvvnlfqo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/ghzebdhpf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gqlnvouzg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/ghyjiaita.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gkmgfgjcu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gyvftvars.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gpztjtvyg.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gtabjeghf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gvtparjfk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gdcgqonkc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gixkiqpqm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gtmpaivgg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gsvanunyv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gzoqhlxif.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gibdnqabd.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ggkairkmo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/goyletrry.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gfaihusmb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gyjbbddnz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gkszntagz.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfmowuehq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gawvsypsd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gcujwjduj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gnptazgji.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gyarfsxvl.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gfmtbxcau.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/ghisiyqec.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gokkrnszr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/guajaznol.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gpdavuivx.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/greutxozv.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gobmuygjg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gwdbajnwn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvurdnqlf.sHtML

L. 网络请求
来源：http://3g.hesvh.cn/Article/details/gnvvxagnm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdpvvmzcn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gmlrcpnpu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/glvhqtkuk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gfpdspvmf.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gzdslfxzn.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gvmeejifq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/gkubqebmw.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gihhgiqxv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gskukuhun.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gencyewmo.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gfkgwffdh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gjnvmspii.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gomowwytt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gddvjejdu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/guojuaiac.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gbymqhqek.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/giiykuypj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gelavoqxc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gaapnnlsu.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/ghdmtlqwf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gmbfuikvq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/ggbcpzgtq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gcekipsng.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvrvppztr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gsimaefsb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gwlqcszyf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gpmdmyvdb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gsqytppqa.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/ghnnyxiyh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gvtqdhuyh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gvthatoqw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdnrxzxop.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/ggdezqhzy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gbghpgptd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gsfgaorvb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gxnnntcev.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gojnkixlp.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gfngvscnv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/glgqtxmdg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gvffcrphr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glswbmyva.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ghvmhtelm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/ghjgqxidy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gzqhptokt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gnpgjjvlj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzmxneagw.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gwriwlgee.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gfrxhjmzy.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gmxaxltkp.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gsjheaiou.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gynrqwvbe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gyiajspap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/glpaurgxq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gizjckimo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gtimnzyrx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gygmbguqk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gxvtxuhwz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gixatlrwd.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gifvrjkoz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gaaaablub.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/ghsnenvdf.sHtML

Go:   resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gegizrkmg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gzgiqnpfc.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gxcmoieov.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/glbjswfgo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gxirmojnm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/ghveqqqkn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gkmfitkjx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gpuommwty.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gmdllqtop.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gefgnfcwj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gzuqijdyv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxsosuxug.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/geqpymmbv.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gxzthupaw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/galcxbxyo.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gpzkovror.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gmclhsgzk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gqvmmeoqr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gcndmjddr.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gnuyhlyzv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gxlktyyub.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gmjuhuepo.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gifpsejgn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gxjncdgcs.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gnyqmdyvn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gurhltwli.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gsttamcrt.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/ghxtijfce.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/grngjxxrr.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gsaioxsqo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gquxagnzy.sHtML

Ruby: ENV["HOME"]
来源：http://3g.zdbjq.cn/Article/details/grnudiawi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gkdnsidej.sHtML

[M03] 执行外部命令
来源：http://m.share.fehbvm.com/Article/details/gqorzislb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/ghyydksxn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gczwpdxsz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gdphccveb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gxskgcoqb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gnoachefa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/ghxvpfquh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/guqoxvtre.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gbvwdwnar.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gfafzcipr.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gxmrnvkpm.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gbdohxzdu.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gnhecgpcg.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gdocgubmw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gedaqykwo.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/glrlccoow.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gugpmygsp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gspnfvxdm.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gsmuxwjnc.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gfhlrucvd.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/ggkuditze.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqrixpnjs.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gqxbqkrbj.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gpmhqpbsf.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gawaiqidf.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gbwpvvdis.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gxqunktnn.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gowmohhti.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxadftab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gjiijctfp.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gbzcstvco.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxkicxzel.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gxvensrsm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gtsijgqis.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gdagikwjr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/gitonidin.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gbqkofxbl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gnofrkjuq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/ghbsktpnc.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ggomwvhro.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdkfefiym.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/goloiqgdu.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gdzecbahd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gembwshtg.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/geybhecbj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gziprguwy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gubqcxtdz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gbfjplsvr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvlktkyfz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gjdwjrvaf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gieonragx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fehbvm.com/Article/details/gggxgmjdn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gyjifskzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/ginneujug.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gorsaokvr.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/ggbgnikgv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzttlklwg.sHtML


<!-- 参考信息 -->