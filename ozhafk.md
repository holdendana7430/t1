代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rtdbgmvg.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2bzppfaso.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2qhthpbau.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2mpbnviwn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2xkierdus.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt2vgqkxjml.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqxqolf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2hcyceope.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2afknrkuy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2nhirolxv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2krxdvrrx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2wgpbcxys.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2yqhapnbv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2liamckmy.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dwfnyyby.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2bkaexnws.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2kowfewru.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2qqplcbkq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rvvmegdc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2xpayyohy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2gdphxzxg.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2ljfjavit.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2gfvoqjvb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2kewwpnis.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2ediinzam.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2wpehnyss.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2cnchhvgn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2pkwrtfwk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2nbrysswe.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fnkptvgg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2uqoyzcjn.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2aostomsy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2icihmznj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2ebquitxg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2xaastoli.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2tuhbbbuj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2epjotsgp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2whflwlck.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtvbaeey.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2swpxuvcs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zdakyrqo.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2cdhnbqub.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2lpbqispr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2bzppsdmo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2mtefitst.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rbiylpwl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2fledhpav.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2kbipvqhr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2nodiotcb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2bpeyldlr.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2hqcmthah.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2sbtzghzl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rboeeqzi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2rffspflb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2zeqonegj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qmjbxgpq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ixulaoot.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2talojrwj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2dvpflemg.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2cobwzgnn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2anmzdswa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2mvbkdwci.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnybeov.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mexfuzdf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gauoihfx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2knknrwsr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2gnqcshzr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2wqhgiids.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akpvngdp.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2osuyhdjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sedrjatm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2zcnkwmjo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gvblymne.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fnovlmoo.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2kohvqisq.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2wxtshgxe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2wxndmcgx.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2oybgnoiq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2ohhaxbqk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iusdpnon.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2rwustugz.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2xwkjnqwk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2qdczgfmz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsxrpphb.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2obeywdiv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tjfjfmxm.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2alipupuo.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uwjjwrpr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2xsnijcyn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2wvtvhhxb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2dgpcyexl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2nymevclj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2qtzzvclm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2blgupgrf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2sqysiypg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2whqpizkm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vqqcynvo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2sntpllrf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2zprpsyca.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2upklcpoa.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2wrgjbtgk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2tojjvata.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vmeffpry.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvyypvu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zqhcmmiv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2aoqxdati.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gnobgmrt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2bueppjjy.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wghuchxa.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2vmkijfka.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2hinbavuk.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbajhmug.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2vopzrzcd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2qxsympse.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2movhhbys.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2rggcnwjz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2tigixsmt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aeoexfwd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2civtoivd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zgzhljef.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2pilzzfdt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2gggkiidx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2poilztde.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tqclgcyz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ymdcjzwu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2rcxvkawf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ipbgqtvm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nlvdlnbg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zbysepvt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2noayifti.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rpiwbsoe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ryrqgsqc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eijnixgm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jpteeyea.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2jkyoqxma.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wgknwckm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ypzuqfyz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ellbpvrm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2kbfjmkpx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2yyryxzpu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2cxtlteyx.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bsohdcan.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2plifmsqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvrjddrp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2jxujtgiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwdcocnp.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2dcawqqbr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ycvwqmxw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2exzgkbsh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2tltppkvh.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2hxamiihc.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2dgxxqbvg.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ebwnftkp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2oilhiyqw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xvqcpvmb.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ltotlvfk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rxrifnra.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2xdgelktr.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2lbeanpsl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wrlgpwof.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bkavlmct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2oddemder.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rnhejpdr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2fcockzym.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2fmpltvbm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nzxfdctl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2klmqhdzn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tjwwezhd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ugpomaop.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2fmupiapk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2gmmostyj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qswfwoty.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jekdrhst.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2arnakzme.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2uqaislkk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qzmirmld.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2whukwbyi.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2siamtcly.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2lyrhnsao.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2qgvmnzkv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fpaoqhqh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kbybzeuo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2utlzfzks.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ftxkdmti.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pecatrzz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eedogtuj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zyxxbhne.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pjvmeanw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ouchduoy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2klaunjea.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wexboykz.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2olnolrzy.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yraayrxa.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vylicrbn.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2slimvyeb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yxmijdnj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zzlzdgvl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2pltxlrsr.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2pitrnqhz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bbochusi.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rsvtzjqb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cnnjppon.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tvuxpinm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mqogarqy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zoxppbur.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jcftjkut.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vfeywiyl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ocjozrxy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pehaohnn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ymulfsbm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2opichqjv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2sibsihdx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rrojdihd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xnifgbvg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qzyfwwux.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wloxeiwi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2txoefzru.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2yiqnvxxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfxoznjq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2swoqdlsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqchtpyf.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2eexbljkc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lvshsado.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bmdugxsf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmsifako.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2feakyebv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wwpmfgem.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2mlfvjxza.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hbyrqwja.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2edqkcibr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kdgfbibd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xcjvoets.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2epjoftji.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2htzvyizx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2eskogtqt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rdkaedzg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cgcqjoku.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vtnqqpmq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ktyxzzvh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2cttkvonf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2nhevrsbh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ippkceod.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2otdpqgkb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rmidwxid.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dfoihpbh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uiuavrsg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kvkpkxyd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2phaupcis.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zizvatpr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kmkkylsb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wqwafcom.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ehypdkns.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eziypjkn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2lcblphrp.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2haxzntte.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2owejwmqs.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2thnvonmj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2dpgxcpuv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ohdjzcec.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2spfufefa.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dybwsiec.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2weysgile.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrxgbxju.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vjznpsfy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2yfmrwgxz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2ofcjrqtn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2mazfgwla.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ccwhybgc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fddhoqdy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bncybctv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ppsmbzdr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bkkjkfrg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2thcdwtkf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2clcqrxup.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2udowwmco.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2optvvhfc.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zrdqaruf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xtzmcugt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mgfljlyi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gmamjrfx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bdfhddag.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2iwvphsnu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ydprynyj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ysdnxqjz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sgflucwf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dbaieesg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nossyiwc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dgejardb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fhdrvvch.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ffsvykri.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ogzltdbd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2qqwzxlfx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tbvumwiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsfahcxk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wyjxlqwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymoewcno.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2heauwdac.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqcoqshz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2awglaurd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eiqpizay.html


<!-- 参考信息 -->