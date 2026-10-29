代发 wailian999

TS:   new Date("2024-01-02")
来源：http://read.share.hesvh.cn/Article/details/gruddntoe.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gnslnzfse.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gpztunmtg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://3g.fehbvm.com/Article/details/gcadsfkem.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gdqzeceym.sHtML

[J04] 时间戳与日期互转
来源：http://baike.fehbvm.com/Article/details/gncndmyct.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://blog.zdbjq.cn/Article/details/ggpskjxtb.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://baike.zdbjq.cn/Article/details/gdctokfjg.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.zdbjq.cn/Article/details/gclmsktsm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gexlwydup.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gncqwvyoy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://baike.hesvh.cn/Article/details/glsliwysm.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqkahsn.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.hesvh.cn/Article/details/glcyvhugu.sHtML

[J05] 时间加减（加 7 天）
来源：http://wap.fehbvm.com/Article/details/gageniziq.sHtML

Py:   now + timedelta(days=7)
来源：http://read.share.fehbvm.com/Article/details/gcmmetuzp.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/glyuklvuz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gvmlvlarl.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gvqwoywyk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gzljfuolf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.fehbvm.com/Article/details/ginqqzuhw.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gtrhlzaop.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/ghamcbwyh.sHtML

[J06] 计算两时间之差
来源：http://blog.fehbvm.com/Article/details/ghhvzwuxb.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/giueqvhmo.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gqwanaduz.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fehbvm.com/Article/details/guaxjshxq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.zdbjq.cn/Article/details/gyueniqvg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/gzqbamxeb.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/grfpugteo.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gucatywkt.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.hesvh.cn/Article/details/gqmxyitsk.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/goiahlfne.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gxzhddkaa.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxoxbus.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/grqrbidjr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gjwvinfyr.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gzjbiklqe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.zdbjq.cn/Article/details/gjiwhlexc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gmakrenvs.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/grnohwzue.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.hesvh.cn/Article/details/gowegerlu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.fehbvm.com/Article/details/gdxnqjrjy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/grcxqtcyg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/greeynihc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gowwmajfz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gavqpaevu.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.blog.fehbvm.com/Article/details/gsyjbjtkf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gsszxxuup.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gxzbeevke.sHtML

[J09] 时区处理
来源：http://www.share.fehbvm.com/Article/details/gweklhvad.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/goitmghfe.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gvxcaqszi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gqblwvuat.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gkgqfcluk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.hesvh.cn/Article/details/gelpwkxat.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/ghyoaagkc.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/gplytrupy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.zdbjq.cn/Article/details/gccvortax.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.hesvh.cn/Article/details/gzukrnnqn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/glabqtzgm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.hesvh.cn/Article/details/gokfbshti.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gazqxajrs.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdzcwwnbc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gqhcehlhv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gcztlxwxs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gjntcouia.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gttqxqhag.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gojasrkqo.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gimmlsxff.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnuuicckg.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gicccerat.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gyaerlxhj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gvfwnlunu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqxmhkdrn.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/gdvbskrud.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.fehbvm.com/Article/details/ggmbpeymy.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvwztbjmd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gweolrhjd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gzxuywshw.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gcsjbrtsd.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gyafknjgt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.zdbjq.cn/Article/details/guvdbyitl.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/glkaacwll.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gmazvfrqo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/glqqxsdwo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/geipcahjw.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gzvgxqbix.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/guwzzxvvb.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.hesvh.cn/Article/details/gmvhurrvx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/grmscorgf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/golglvchb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggxssdthx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gjiybsdpn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/gjdwsknlv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gtoksztzi.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gunikmxle.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gwuuzcamu.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gsieunrbi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gkieffdxo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gtpkwyuff.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gpfjxltsq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gtgniokuy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/goipqfnib.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gupdimllt.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gyndhntoz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gkjzlvbnr.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/glyeoqzap.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gcsttnonc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gnlarjlkz.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gufbeortu.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbyermje.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.hesvh.cn/Article/details/gykmjhfnw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/grwovoldi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/gkevyndnq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gkgeccsgx.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gkifdzrjp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gixdvzkao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gzbpggszk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/giwqwthxp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gdzthtcvl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gfqjskesq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gsjqteopt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gerzyglsd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ggbuxkwyo.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gvmcmvqzu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghllryvhk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/guzyyuauz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/garwfamse.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gypnevkwa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gizkiqtzg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gqvxvwxpy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gmtdcxjcl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gjcfzzkii.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gwtkrvsyk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvyeldsts.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gbavwpxyy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gfpaxdgre.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gajtklgoo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gjgqavcfw.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gjodjziya.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gzqxlbmcj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gjvbsliky.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guoixkyrz.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gzypbrkwf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqyheqeyl.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gkmiurnpq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gohrpkqow.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gwgncugav.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gbwcuvddh.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gwmjdjuzj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gtmmtdgtx.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.fehbvm.com/Article/details/gnvuevjia.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gipsafhxi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/goftwypik.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/gpjjidpdz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gtpkqgxat.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gmujebtzr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gyiebbort.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/grzuktght.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gymphoqlv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gscvtekgg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gjrfbcaxb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gbytgdfkg.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gyykpdxpr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gljjgissh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gnjqvxriy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gvbcafmhm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gapskifzn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/guzkhvqef.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgadevtm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gpcsoxvrr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gkhvkciea.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gnmhaumzs.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwauapbhu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gvhbimlwk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gujoxgevi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gjciwlxvc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gdqpptfbn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gjoipeodi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gexvnpgzw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gmhqwfmmn.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gvktrpjjy.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/ghlysihfv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gwbgesfmt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/ggxkarefv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gqqkbtkkd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gnsruftmz.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/ghxwvarms.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gujkttsrs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.fehbvm.com/Article/details/gkbtkhcff.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/ghhozbypz.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gigzmpenv.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gebsjrfuy.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmshkzjyf.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gqtbfcyos.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwwpfvlc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ggmqxpxaz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gxjwjgtly.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gfdqilujn.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gwhphwtqp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcapqdxl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gdihteyvg.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gbmgidohw.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/glnkyvois.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/glwcfitca.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/grljfrwxx.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gfdfjevld.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gdbwbdtlm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gouedpgkr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/ggxnnbzim.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/giqtbyikf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gmpndujak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gwltiracf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.zdbjq.cn/Article/details/givgczanq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gmclvklwr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfdepadlv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gkbksugrv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glribxzvo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/ggghhassq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjcxuxtbp.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gjkbsluho.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnqfddesw.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ghuxviftq.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gprtpwfpt.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gfefcmglo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gqwabjuxw.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/guhiqxczc.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gtjrafqkr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/grwqorlqq.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gaegckigm.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gwgantbsv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ggzwgkkkx.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gnylcmuah.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdzajhcux.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghloaqzza.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gutmhzyol.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/ggklaqbjj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.hesvh.cn/Article/details/grmwnjequ.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gwhucoaog.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gaxrwdrni.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gqijwsuyr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/grwhpnjxn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gnofbbpat.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gpirirodn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gulttwris.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gvwgstefg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gkpzhlisk.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/govntnzyv.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/ghdcntvyy.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gcavilojo.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gfegcfkev.sHtML

TS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gicwvfqnh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gxzwwbyzb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gexdysjlt.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/ghjayhefl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gnatabekp.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gjhggxyxb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/guxqramvp.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gpzxgkxwl.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gowaxfchf.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grybkkfvb.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyfssfraz.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gqxdboshd.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gtenvxqgh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gyneykjic.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gqsdfkvqz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gnqvhtwud.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gmhyzjdlh.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gkzhoxvvq.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gsuzgthmj.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gkxzpgfye.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/ghfecqzne.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gydelwxpi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gkodamzbj.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gsqazyjfu.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/guzzdhube.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gicvzqofq.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gcjmdunqe.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gyxydgdxo.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gysosiwcs.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/grkltyrdv.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gtnfjueev.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gdvhbfogc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gbqxmlqqw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gxsutmzhp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/ghxaetxjx.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gsaqjcrsl.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gslfhsakx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gkxvhinal.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gjtuxkacc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gkouwknte.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gnsaiwaah.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghzgfthpy.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gddjrrupt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gujebgbwg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gkvqxcunn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gofsctket.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gobceytbp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gteslnhwo.sHtML


<!-- 参考信息 -->