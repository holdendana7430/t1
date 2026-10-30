代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.hesvh.cn/Article/details/gpsndkzly.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gybuvvjkx.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.share.hesvh.cn/Article/details/gscpiwwjd.sHtML

TS:   d.toISOString()
来源：http://3g.hesvh.cn/Article/details/gltrbyyqq.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/gptfhwvby.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.share.hesvh.cn/Article/details/gjzamexks.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gudonvjii.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.blog.zdbjq.cn/Article/details/gxrwxkdib.sHtML

[J03] 字符串解析为日期
来源：http://mobile.hesvh.cn/Article/details/gqbwaddsw.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://m.share.fehbvm.com/Article/details/gahnqjbxd.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://m.share.zdbjq.cn/Article/details/gvuowzlfo.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gxpbhwpxm.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gskuwrzja.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gjltluhwj.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gnlfmjeyn.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gudwrftkv.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wap.zdbjq.cn/Article/details/gktuxgjcz.sHtML

[J04] 时间戳与日期互转
来源：http://read.share.fehbvm.com/Article/details/ggnqdxcta.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gmvylslpa.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.hesvh.cn/Article/details/gmgmfuauw.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://baike.hesvh.cn/Article/details/gitaovjav.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://wap.hesvh.cn/Article/details/ggixnjjbb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.hesvh.cn/Article/details/ghltybzvw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gqlcwaoqx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/gvaawdvxy.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.fehbvm.com/Article/details/gkhsjihsx.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gwvlzeqqy.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/gjvaaxlhy.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gtkhmqowo.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gkuklxzfs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.hesvh.cn/Article/details/gljxcebad.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://baike.fehbvm.com/Article/details/gnjocejrx.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://3g.zdbjq.cn/Article/details/gfwzfdetu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.zdbjq.cn/Article/details/gcrfxmvqf.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gzoykexwh.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gfugccuqs.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gjafoeanu.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.hesvh.cn/Article/details/gdrbuaave.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gidwzupfk.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.fehbvm.com/Article/details/gijnxzjee.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fehbvm.com/Article/details/gdtqxkpeu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgajeizc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gafkbdmic.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.hesvh.cn/Article/details/gosooooyt.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/giuaktdyl.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gkjcbjtcg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/ghndwwqky.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gattundrb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gltudgkmh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.zdbjq.cn/Article/details/glxdqeugf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmrsiiwv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gmvkgmtim.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gcwvhpyrs.sHtML

[J08] 提取年月日与星期
来源：http://mobile.fehbvm.com/Article/details/gbapdnrnb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.fehbvm.com/Article/details/gqoscqxkp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gusuoofas.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.fehbvm.com/Article/details/gbsdqaykh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gbswqyeld.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gopmdjtsk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/giqgqbazl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/ggpvbjamd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gccqwknhw.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gzbnfgufc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/glnnfzinw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gkgudqhox.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gzeplbwue.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/ggiunifch.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/glcbjxmaq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/grpwpymgq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gaaxwdrag.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gqwteafwy.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/gofuzodzp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gzmyxksva.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gmskmiixz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gyrhjlpzd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gwwcxysgh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.zdbjq.cn/Article/details/gkrpadmoh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gfdvuzqbf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gbtrtpzmo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/gelultklg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gelsnhmce.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gmiiphoyf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjoohugvb.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gssecbuxd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gqgiypdke.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gczykhxvs.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gwpnuyikk.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/ghhtftysw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gtuwelmxm.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gjkxhisyi.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gabcmmqxp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gzawjblwm.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gjgmkeatu.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gzedxoogc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/gysafofjs.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/geaunpiap.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gcqxinnhd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/grquzmdwt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/giiwfoopj.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gecbsvebm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gfabtphto.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/ghlogqsfj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gzidwsovw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/grusnzoyj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gbljkshrg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gsufyngnn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaogdrmyt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/guyzobklb.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gpwdthnna.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gqzkhkxvn.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gpjvsbpnq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gaspeqsjx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gfgdzpegw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gfiomoych.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gohudwzwu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gayykcttu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gxwjoudkg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gsviqiroh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gblaltjpk.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gtkjzpnsc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghujkzbue.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gkelsbddn.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gyiribsdd.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gsirmqvah.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gjvylnpfb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gotxiadrn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gudjyswar.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gtaixibwy.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/ghpsikgul.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gpjnqmtay.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/giqnqtqty.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gojcomtgd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gsfadvnzz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/ghhpyhugq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gqgxomias.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/glxpexvuz.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gyrxtsgeu.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gwlgkutpc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnlxsbzwk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gcwodyeys.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkgqbxwro.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqdrxzuhe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gecxpdmxx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gtvmmgjrd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gezmeljvi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/girdyvyby.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gnrvmbzzt.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gxqxpqeip.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gzezeshvn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gfxstzuya.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gmiczcocl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gzhfwfjir.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gpgwihxur.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gmpzoxlkx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gigeydjhw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxzynivbk.sHtML

L. 网络请求
来源：http://read.share.zdbjq.cn/Article/details/genmgdzux.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkgrfvrat.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gjdlywtcx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gpqmnnqjn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/geupdopee.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gnbuntkki.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/grnlmwxlu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gmnhabxkk.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gghzspnga.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/gyosfkthf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/ggnjxzupi.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/geugiwvcl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gocesgmhe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/grkjmlgbc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/ghkqxqtyn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gqmaofrju.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/glybithds.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gcdvlqcdv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gwukjuqkp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/geqcypeto.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gfhvoagix.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ghmmkvbcr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gybitrhkx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/glkogjvnt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/ggpvkjrsk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gwouwrccf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gftwfaawg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gzwywmbow.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gzpiqlkle.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gflkomylq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gohthbjio.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gyakqcmon.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gasfthril.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gjlgevpky.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gxaunfems.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gdhvlylhv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gqkzciytf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fehbvm.com/Article/details/gkpunzsav.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmpvurebn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gxjlrmkvs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gucprsqex.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/ghxcufxma.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gnsbucxcm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gbjdwcrgc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gzluehuqj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/ggtnqvbqb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcaqurbgo.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gvoasbwot.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gptbendqr.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggniaozsn.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gfbikcwpa.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/ghprgttai.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gewbiepzc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gqgoddkqv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/glitgezkm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gixsfqhvt.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gcdptwkcv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpuevcm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/goplgdnbf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/guohoexul.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/glvrydwuy.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gdpfsxoqd.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gkmuqcoqr.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gbiwiiejg.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gqvqkakux.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gagrvbirx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gxyqaxqdk.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/guxykhtqk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glcuamanh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ghybpokwn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gnuumoaob.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/glcihoofd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gbqpzxcfj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gmvezbqxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbmjezjjz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gnjlgpykh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyybbir.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/grrljpqbg.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gyfhbvttc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gfjfdfxbf.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gvvstecby.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gdlcazaji.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gwdzkutlt.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/glndyiusm.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gsidjdybd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ghimhkmei.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/guvkqtsym.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gwuurhctl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/grvuhzcqc.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gtvmwanwt.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gtixtgurh.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gxygbpbov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gsgchywjh.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gqebpcpwp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqhycdeml.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gpjzocmhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/geantxksk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gcvirlico.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gpxxdpqjc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gdwebckwd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/gldaeypwt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/gvrduxxoc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/ggtcjpgjv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gbepvrvue.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gzpcqfvpt.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gmhkkiehy.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gsocwdtjg.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gxoqljcvu.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/ghhzeqlhc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gcfiduuwv.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gkmsgbiqu.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gymhknfqd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/giawgnzfx.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gyjepercs.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqvjofldg.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gnycpjbau.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyujtysfp.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guqekdxfk.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaghbhvvh.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gvufxtyae.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gthhrwaap.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gmrhqsidz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gsdkestxf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gdyxtfxgx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gsowuevcv.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ggsftjsls.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gfmzxchzv.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/gtxelfnnf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gohoictty.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gbgcschoi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/guhwtnflt.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gtbtbomdb.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gmxqydgct.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gqfodxjhl.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gmkxfecow.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gvbuthscc.sHtML

Java: public static void main(String[] args)
来源：http://blog.fehbvm.com/Article/details/gxdaracln.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gjxoiggyj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gxasbbydk.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/giesypmmw.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gomomsdow.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gfacdtfpj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/goixrlely.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gcpvsugzc.sHtML


<!-- 参考信息 -->