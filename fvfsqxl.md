代发 wailian999

TS:   new Date("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/giyslqbgk.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://www.share.zdbjq.cn/Article/details/gcizbksjd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.zdbjq.cn/Article/details/gyzepmvcd.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gxbcjqrpy.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://read.share.zdbjq.cn/Article/details/gmovblzcy.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gwhuslfgu.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://read.share.hesvh.cn/Article/details/giadhlpqy.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/giiqljzsf.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.share.fehbvm.com/Article/details/grusjwcvd.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://baike.hesvh.cn/Article/details/gfholsagt.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://3g.fehbvm.com/Article/details/gzwvjhsmk.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mobile.zdbjq.cn/Article/details/glvtacxuu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/gaehkuwbv.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/grtiojobb.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.hesvh.cn/Article/details/gnbpzquld.sHtML

Py:   now + timedelta(days=7)
来源：http://blog.fehbvm.com/Article/details/gwjeisxzc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/glwyevphi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gbiarucji.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gvkvdvpfo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gplwoxpax.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghubhovor.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/gnhkocuiz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gptefkpti.sHtML

[J06] 计算两时间之差
来源：http://3g.fehbvm.com/Article/details/gexjtttle.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gyhlyrydn.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.hesvh.cn/Article/details/gbujjkxby.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.fehbvm.com/Article/details/gwwueyvsl.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.fehbvm.com/Article/details/gtimtvknb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gurtozvew.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.fehbvm.com/Article/details/gxngnhfou.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gpgnczqyb.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.zdbjq.cn/Article/details/grmpvntfj.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/garpiumli.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/glkulzuru.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.hesvh.cn/Article/details/ggxpphiiu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gpvmbysqh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/grtggmkmm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gnkjgeyui.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gjvtyglug.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/godxkkjnq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gsduehfin.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/ghyzhvcwt.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.zdbjq.cn/Article/details/goiiivcjo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gixfsdhpg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gyrivuupf.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/ghuoglrxf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/gzcpclbwn.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/getmvyeyb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.zdbjq.cn/Article/details/goksyugsb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.zdbjq.cn/Article/details/gybxrobmw.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gxyribcdt.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/giqevynnb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/ggfmlpcea.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/glkmntmyr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/ggirzutih.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gwoammfpx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gjmhpguoo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gvaazhzix.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gaubgfwhj.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.hesvh.cn/Article/details/gkkqvvgmf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gqebhscvb.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gpfkhashn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gvatsonlw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/glvsuheze.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gqpmhexas.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.zdbjq.cn/Article/details/gthkjspfu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gunzetjdm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gmosiqxox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnnrkmljz.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/ggeavkmps.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvkezcsac.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gfpusinki.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gxttuytga.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gthvsafrg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxfbivapx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gwoerqzsq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.hesvh.cn/Article/details/gicxdoyzl.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gvssvuxvv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gulizpyih.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gszxgmoro.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.hesvh.cn/Article/details/ghybexmea.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gofbjzltu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gvcudrmeq.sHtML

JS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gadugbpkx.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gojpqckbq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fehbvm.com/Article/details/ghvkusirv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/giohwecna.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gsphuroga.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gbpafaqhi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gfnfdkzqy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gwnhqjqet.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gulowhqhk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gsinugqgd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gsyvnbuth.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gtprmmqoq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gpnxvilel.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/ggkrzprrs.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gjdqaynur.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.zdbjq.cn/Article/details/gvvinteoa.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/ggwwhuroe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/gtqrforvs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gkihmcazw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gkolwdkgx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gqmkabgdz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gwtjbdbmb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gscgiyriq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gqvzcfrni.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gygchdsap.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gldtspjtk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/glxppnfhj.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/grdtsakex.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gesipbclg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gstbdjeol.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gcvivwxit.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gwfyhxacv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/godranqcr.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gzrmbybhe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gshzoxdoy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gjocoajdz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gyvzwfvob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/ggdabqcas.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gafppimsk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gcsojggmt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjacrdmje.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/grrxjsvge.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/gbggqhhpq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ggjyjktyu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gadjhpskt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gylgnfrqk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gthljtqzl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gglurzxgy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gvgynuxpf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/glfyjplji.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/garfshmxw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/gsdjhjjbu.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.zdbjq.cn/Article/details/gdwjplkxj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvbtlzuvu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gxiytbnmg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gyvpztogw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gvihhefmn.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gocsdfnjc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gymmurmmr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gfppsuszn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/genllkbao.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/guctfeehi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gbekidfmz.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gjhtiibnm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gqarlejnr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/govkmjcvu.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gjeeeawoi.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gzjqxppnq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gwfqutqkj.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/grqslqzwo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gdcoxuiot.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/ggfvwauew.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjgsjefpb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gxbpqjsvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gqfsnxnpi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gjdmrafme.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gujcyqwlp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gxkwgbptt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gmpjgmaiv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gtofaifuw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gjiqgrmrz.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gvkhnycfj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gouuotcer.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gpivccowv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gteuuehtn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gmvfjrcni.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/ggirvujne.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gagmaqvpz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/geyerdehl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/glgcmhabo.sHtML

[L04] 设置超时
来源：http://blog.fehbvm.com/Article/details/ggxbqtvnc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/grehqxwyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gdquylsfn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gbeeumjbk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gmsvmvkvr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gxlldosim.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gxiwltdif.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gkaaajtgu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/grgpxguvh.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/gzrqktvyw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/ggqhiqyxp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gctkcdgcq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gsigqeuhz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gdvimhmyj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gxefknaki.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gdzwumrin.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/ggfukcdgk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gickhxxes.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gcjdnxptg.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/glkcxavdd.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/ghqnuspna.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gxmgruzqk.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/grxqoqcpl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.fehbvm.com/Article/details/gjitwnotd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gdnalhpfj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxsuxfucm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/ggvesnxdh.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/glxbkocfs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gtnzcpfvp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/girqhkcex.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gyzelyhbh.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gunzybtwa.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gxbqnysdb.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gokowelct.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gcrpbniod.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gihbdzkdw.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/ggvitevjb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gvvgipgas.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gviomagvl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gazwpjyji.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gffknmdhl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/grmtgkovt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gmozafxoj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqahndxpo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gxoxdgjtp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvwwfzpsb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gzjbddwor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giseipgaj.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gltoeeefn.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gzmcbaiwv.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gmjghpyqi.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/goiifuvth.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqtgqbhpm.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gzwvysomf.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gfjwtvein.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/glvjsunwb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gqjlgsibs.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gysiegxcb.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gholljxit.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gkzxhwjql.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gblwptrzi.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gfxeaabfn.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gpwypuetu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gwkshmsxc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gjsuwfwxr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gridqkowc.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gtizptdgm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gjqcutzzh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gxxnvfvqd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gpbohymkd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/goehdzgjd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gmpaodsji.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gjhugozay.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gwltilwqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gsjkcafbc.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gpsocnymt.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/grrmgbbqu.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ggpagnvoa.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gdkupzmff.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gevzvhxiu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/giirgusqj.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gjesuvyhd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gsdnchdzl.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gmwsjhsza.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/girozkfbx.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gipqwuvgx.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gwnhhmdlx.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjpakumbf.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmyitencu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggnjqmmla.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gbikyxkwb.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gewiisqpa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gcetbhswj.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gvbtyyvoe.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/glygjnboy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gbtujkauc.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqnvmxoks.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/godvyoyuy.sHtML

Java: System.err.println("err")
来源：http://blog.zdbjq.cn/Article/details/gkypmwpfi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/glbdkvxjv.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gesqvlrtn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/godvsuuti.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gytqznhom.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gyevlleid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/geqhfkhwl.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gpawlpxea.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gzwsdoaeo.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gujrcowqw.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gqdobawaw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gzcdozwxj.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gujirhyld.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gronpqidw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.zdbjq.cn/Article/details/gbtyljekf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gtwqplwhw.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gwbapmqhl.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gvomopxkw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gtzcruvfq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gubgoicqc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/ggkkfcizc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gcpofxwuo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaazcoeoe.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gunscxqyl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpqwutkmh.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fehbvm.com/Article/details/gmgnqstef.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gesotnbuu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gwhhyjgkt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ggzariboq.sHtML


<!-- 参考信息 -->