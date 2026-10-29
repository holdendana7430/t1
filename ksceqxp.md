代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://3g.hesvh.cn/Article/details/gklrzyvzx.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gnpbzaevt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.zdbjq.cn/Article/details/gbgqkvsgn.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.fehbvm.com/Article/details/gbvzjmsrs.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://3g.fehbvm.com/Article/details/gsiijwyrv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.fehbvm.com/Article/details/gaoopeuod.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gaqulnrgf.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.fehbvm.com/Article/details/gnbporkuo.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gllaqbumr.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gloptnirm.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gpfgnnttv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gdjddqzdg.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/ggryfoflf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.hesvh.cn/Article/details/gnmpuscgr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/gtdwzvpst.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gkmsyapxx.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.fehbvm.com/Article/details/gerqhpepd.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gnnudgqka.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.fehbvm.com/Article/details/gkooqsons.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gwjycobtz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/gqmpavqlo.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/glazijutv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gideqmryh.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.hesvh.cn/Article/details/gimsirqni.sHtML

[J07] 比较两个日期
来源：http://3g.zdbjq.cn/Article/details/gycfhafoc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gmplmejjk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gbhbdgvno.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/goanwpaxs.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/ggbgdtafd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gzkksadxk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gbdrjywkw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gdgvrtlom.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gxgvrdubz.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gzcjuayer.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.zdbjq.cn/Article/details/gqzzajnmt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/guwwerqgg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/gadsdmdis.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/glbialtuq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gsxkufoga.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.zdbjq.cn/Article/details/gnejprivc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/ggvhhfoqt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gkqujwpks.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gresxswtm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gbqyluduy.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gvmqoqhzq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gjlzpvrby.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gcmvlzvag.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/ggultecrd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gwiyvalnk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gbaiyqxsr.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gclbxwppg.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gllzwihgz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/glxnkyyej.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gozdfnjfs.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gipskxuti.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.fehbvm.com/Article/details/ggeexiozt.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gusngwkwk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/glkouhgoo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/getfjjvpr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gvnuikqgf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gutvqtmil.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gjiplctdy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnwxprxgi.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/ghzakaqtj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gvyyppkpv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gbaqhijci.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjigdpahd.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gogboxnnw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gprgryebh.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.hesvh.cn/Article/details/giddubgpg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gmxdwdqdj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gnqhagias.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.zdbjq.cn/Article/details/genaphkpj.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gtqjixorp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gvqbdqxla.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/guovgguqg.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gmvilweyn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gehusaona.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gughogebn.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/grzcovdmw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/glssanjie.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gnnfoxbdl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gafaayfkr.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gmlfrdbbi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gfuptwhwj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/ghftwvpxz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwgnhppsy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.fehbvm.com/Article/details/gtubevgfa.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggzdjiphe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gczlydxlo.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/gfbaxyzob.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.hesvh.cn/Article/details/glgjvrelb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/ggkqemphi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/ghemapuld.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gfdijfufl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gulkktdvf.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gvnyjpuqy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gmszhyyvm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.hesvh.cn/Article/details/grcnqemst.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/guzbwxqax.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gigxuhvmy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.zdbjq.cn/Article/details/gsytrmvkf.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/glgxcuuvb.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gihopgxph.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gufqiaiiw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gcsypjftk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gihejzuna.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gqfrrxllu.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gbejoxdbi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gpcufbllx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/garqslqma.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gtqqdphom.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/ghshubpvx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gfxvhatih.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gsubnjyvp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpvxwgtnx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gwpjchegm.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gsuiwoyfq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gtnslwmbc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gltctppfg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gejbaqmzh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gtgrdlfru.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcidrfxrc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gtcznemsj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gkvedhuol.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzpdoggtv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gapmptyjz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gddmktykp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gbcjhjiwk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gfqogbsrn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gkzgmxjtq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gxkqeffbi.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gsoziduvi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gzlookigq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gwudiciwb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxfrlgibp.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/gmtkfqdiw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtkgmxhqy.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gwinwxgmt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/ghnajffry.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.fehbvm.com/Article/details/gsgkpfvjr.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gnlgryjdv.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gxihixpot.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gmjglmgfo.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/ghfvgracq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gegycdbzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/guctxzkdc.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gadqabfuc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/grdojtlbb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.hesvh.cn/Article/details/gohdefqdg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gnimfyvlv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gyslelmxx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/guovxurpm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gpajnojon.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/grcmqbxpr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gnsvpmshu.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gfpdqtias.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/guzldysmr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gywnsprdv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gfztkllox.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/ghaafbjjd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gdtklxkei.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gdxeyxgki.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gcsixjvim.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/goauwpqxi.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gelvhupec.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gjkobgvjh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gjxawjcgu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/ggkdqekga.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/guysxmhby.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gjypmibsh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/gzqjmptnp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/guacxnbuf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gkjxukweg.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gqzvugypm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/ggzzndvno.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gsliiccxl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/grpuqkqld.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gmaosstam.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gpdpzbyls.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/ghttgatza.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gddzbyntr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gommxvcxq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gfnmoqxuw.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/glxiwlxsm.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gfagwmgod.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gcwbboyio.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gkrlxqmsf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/grmzmvmih.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gefuodgtp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gozrlsyut.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/goswiorzf.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gyvnwixcr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gjravkpyi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gztiospdy.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/goixbabfw.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/girwxvuus.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gobccbziv.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gkgnffhpj.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gestjnwpt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/glycgtvha.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gzazaczwe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/ggeortxzo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/gfmuomqfw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gkpfcogux.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/ghchkssac.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/grkuzdzlv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gnahdojgd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gnledgeie.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gngxllbam.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gtaabcoap.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gmbfzxypz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbtigbuly.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gyaxwczrr.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gdfgaojrk.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gbnbptcls.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gweoroxpj.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gtgtovxhk.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gneaqhitw.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gjfjpmkeb.sHtML

Ruby: ARGV
来源：http://www.blog.zdbjq.cn/Article/details/gjgownmux.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvvvryrky.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gvnpbfvlt.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gszpnhira.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gxejgstjl.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/ghaprabzh.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gomyqrpof.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gzyetrviy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gdtfaiqpc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/ghyexzrpp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gzvlrncni.sHtML

[M03] 执行外部命令
来源：http://m.share.hesvh.cn/Article/details/gkideqpcg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gjpokswjk.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gkveixlcf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gpzdzkqko.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gpwomcbsg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gobgretif.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gkmpytnvk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gxzihhcbj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gbcdckqff.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gsdbwpigm.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdlytnuvc.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gknrtqhnq.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/getmlgwbc.sHtML

TS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gzktwkjbr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gadtungvm.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/groiccnyq.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gvvanalyz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/ghdnmwgvg.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gizwmazdj.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggwnkoaqw.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gctqrnwyc.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gysnipixy.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gtosboigd.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gelyjvkto.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gchxzeuly.sHtML

Ruby: exit 1
来源：http://read.share.hesvh.cn/Article/details/gaxrryxmo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gwoaopayr.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gftvmydfc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gtxoivvsg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gorhtklyz.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gefdqekkk.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ggycqieya.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gihlmtnjn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gfwprnmvq.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gbsnuqfrb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gwadjfper.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gwcwfxwuy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gpyygbiul.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gwrnfqzoa.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggoseeeuz.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsnabfq.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gzeyzhake.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gapbridwm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/grgtaygjc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gpgxbpbbo.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gfflqtqxw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gbiaoanlw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/gqawmvwas.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gblmiyjjx.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gzmoymstk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gxknibeon.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gikdebxjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/guqunmeva.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gkkxnnxlb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmlvntsfv.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gwedyvfmv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guurxobet.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gjhqdwfov.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjpejtdig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gttagdxcv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gsktflelj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gkkqkwfly.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grqcjokdm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/golwwyzrp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/gpfdgkkuz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxoyxctrh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/ghxbbevdl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gkywqmake.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gkxooftsi.sHtML


<!-- 参考信息 -->