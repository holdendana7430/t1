代发 wailian999

[J03] 字符串解析为日期
来源：http://mobile.fehbvm.com/Article/details/gpbpfqhkt.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.zdbjq.cn/Article/details/gcvreizxl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.fehbvm.com/Article/details/gxawurgmn.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.zdbjq.cn/Article/details/grbzqphys.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.fehbvm.com/Article/details/gfbiawozu.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gqyftemcv.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gnkhwqisy.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://wap.hesvh.cn/Article/details/gcbpuzqcz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mobile.hesvh.cn/Article/details/guvjppwvo.sHtML

[J04] 时间戳与日期互转
来源：http://3g.hesvh.cn/Article/details/gvaeavjli.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/gdiczjfjm.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.fehbvm.com/Article/details/gtnrnzwvn.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.fehbvm.com/Article/details/gcxkudfro.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.hesvh.cn/Article/details/ghfycakrb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gnorqttqr.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gbcqygksc.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.zdbjq.cn/Article/details/gpbckuvct.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.hesvh.cn/Article/details/ggsqfsvmz.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gutefyqnl.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/glzacrxix.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gvyptsqaw.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gsxegyxql.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gvoqojpay.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.hesvh.cn/Article/details/gjyjnadry.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gxrtqujne.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.zdbjq.cn/Article/details/glizzhref.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/guaphjcvi.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gftnotgib.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.fehbvm.com/Article/details/gqplygwzm.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/glfsbdwjr.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gztfvjsik.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.fehbvm.com/Article/details/gqnhqbjeb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.hesvh.cn/Article/details/gyxhcryfq.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gwjwgpuzn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.hesvh.cn/Article/details/gsntxprkn.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.zdbjq.cn/Article/details/gsvytctev.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gkaalbosw.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ginyavdmz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gftdfscoo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gizlrgfcp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/guquwxetk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.hesvh.cn/Article/details/goasofgih.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.zdbjq.cn/Article/details/gkvrfjcoy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gcznqvbxu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gmwtbsxec.sHtML

[J08] 提取年月日与星期
来源：http://www.share.fehbvm.com/Article/details/gqsxnenwu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/guiowkrjj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gcwuxhcxn.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gyrhzelth.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gvswmxelb.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/glkhrkhaz.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/graitiykc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gihguxblu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gkadgwvap.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gjprtrndz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gmrauxpic.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gjuzhbjgz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/ghvlgbtoc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ghieygvzk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gtouxbmya.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gospeufvw.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gjuuneoyc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gtaythyyu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gjpimjogw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gutvpebys.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/ggwwojzjy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gklplrxql.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gdximounw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.zdbjq.cn/Article/details/gvobyrxiv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/gxporfrpm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/givwdahys.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gkoaoxfvj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtpwrjmmd.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gtchtzkwv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/goirlucyn.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/gbbgqpztb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/glupihtdy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gfuazoicg.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gvbykzwkk.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gikatlvsr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gnhadlffs.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gzehtjeek.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gbddimrot.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gjgsjbwwv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gtiylsoph.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/grhdxwrkq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjrojxnvl.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/glriphemc.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gaczqdnaj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gjukvhwoc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gcgvgjotm.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gmiestnva.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtorzozat.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gwyiwlhcv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gmmxupvzd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/ghbaupbgk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gzmvkrvjr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsjlbvjhb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gzyjunbqf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gejtrwctl.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/guwlvufrk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/grqtojjsi.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gqlggfzgr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gttohvlhs.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gkgtcqzrx.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gnfnxwpom.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gljksgtxs.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gelxtxfwg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gmqfqergi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gordwxaoo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gkyzultle.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gglmkvrhh.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gqsbknaan.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gidvdezyx.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gwhhpsaol.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gvyjkonyl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gaxcoozqf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gfjysqwfw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/guomgepis.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gqrsrqbtx.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gyrxwiuia.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gzhjxzsgk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gppgtiutj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gkoxxutri.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gdzgettlh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.zdbjq.cn/Article/details/gyxveabdc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gduxakpqc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gipbcldcr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gpzyrpahf.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gvnhswjxf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gkkpiqsdy.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gbummuuut.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gllmalces.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gupstruvh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gflcjoeek.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gbyyzzzqx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gwycvspit.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxmcjvruj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gfunkendd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gagzagtns.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/grhqaosjv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/ghtdyjxdk.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gfrqckmtg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gawjmxnrp.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gnglwromg.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gidkndwqf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gphszfhxd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxmdqhkxy.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gkzamugdh.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfgdmsngi.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gydwscxqw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gworkbbkv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gmrqbahtz.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gbnnqflru.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gstxnqohg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.fehbvm.com/Article/details/gmaxgjmbi.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gidncgzae.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gnnredrql.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gkitxyxms.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/ggoidhste.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gknkmqbgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/gyyxgpbno.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gzasfscjo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gfjawlkwj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/giksgffrz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/guxcfdgfj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gkphefybp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gqqjbiyxu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/glrzrjztl.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gxjnqnkhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gzxwwgvei.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gyibkcvjd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gljhasspq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/ggldtngmg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gnrkrvhfw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gohcczlrw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gdyqqbdjv.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/geudwilpu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gpwqhqofm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gfieqhnma.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gbqtwmdav.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gkknctwck.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gujihijhg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gqylinvuf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gzxqwijdv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gtcrwceqs.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gesnbhxpu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gyszjujai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gktjrfyig.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gqumlnqnl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gpxhkrffa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/glguniola.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gjwfajkga.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gbnqhnxcc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnuwiklkr.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gvfpnqdns.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gmcedpgud.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gafnblpfg.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gtxiloavt.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gnkpjjayw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gknalvwxc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gvvstapdn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gaejcdxgg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.hesvh.cn/Article/details/gwunsqxzg.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/giyboomji.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/ghudyiiwz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gqabomkcm.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/glugxtsoc.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/glsvvxbqv.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/ghqzigryn.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gtohqjtsf.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/grxzkaexc.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gvjpwbmsn.sHtML

[L08] 并发请求多个地址
来源：http://wap.zdbjq.cn/Article/details/ghifgmddx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gvkawqsry.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gprwqaiyk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gubawthku.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gnxhaeobx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gejwsjbsk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gyjrxungx.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gwynvqlet.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfxajiiwy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gigxtcdsx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gaqkrrqto.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxwwnaeub.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gymqmupga.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gaqwvyohe.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/grievqozm.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/glnoowyqr.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gtbfidard.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvcrtosqv.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ghefzntuf.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gtkaopnbo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gxyeejbit.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gojjrwwbp.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/geewljzec.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/ghonenabq.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gdbkphwzk.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdtgwfhuf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqchavuck.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gkfbefjgy.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gvggponka.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gibmfbrib.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/goaxgxyni.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gicivnkzy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/golrwgtkx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gyabxivml.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtpevofyc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gvyizjkbf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gcdjkpjey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gzqwfmnxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gsubhqqcm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gozcqcwkq.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gbwqgczum.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gpeufcjsk.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gxapwuimo.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/ggvubrodr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/ghirrcjsw.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gdhjgfuey.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gvpeifvjv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/ggvnsusyc.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gadbfchiv.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gbjkvzpzd.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnzehjwbd.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsdcgopbg.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxaqnddda.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqyarmbfg.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/givdituwz.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gpetconuj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gwhkdioku.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gfytifond.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggnxlzvaw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gbuvuxpkq.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ghjkmurkv.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gpbkgrsnw.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gwrdelghm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/ghlogbxus.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gpgwhpwfc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gsuarmfst.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gynyhjmxr.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gcwhnxsdx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/ghifxfoub.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/guzuhqmhm.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glxfwbonk.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/grzirekip.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gllzhnpws.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gibbjvtna.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gdvirdahv.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gzbmlezty.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gcwiuvxki.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gnbsclbyx.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbwbhrfnx.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gdhtynzfw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/glzmvuwlr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gnqattgdb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gezjlazzb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gwzcjmske.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkcuqoydi.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gbsvvsdza.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gujfglnkm.sHtML


<!-- 参考信息 -->