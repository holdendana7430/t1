代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.blog.hesvh.cn/Article/details/gvblwzuti.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.zdbjq.cn/Article/details/gxhrfstss.sHtML

[J05] 时间加减（加 7 天）
来源：http://blog.fehbvm.com/Article/details/gojqmtepb.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.hesvh.cn/Article/details/gexwtrhdq.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://3g.zdbjq.cn/Article/details/gwescllpc.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gieckebad.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gwkbolylx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gegnusfhz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gldgccriu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/gwmzfwcnu.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.zdbjq.cn/Article/details/gmjzdilzo.sHtML

[J06] 计算两时间之差
来源：http://3g.hesvh.cn/Article/details/gmrydncis.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.hesvh.cn/Article/details/gmmpsniwg.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/gayaswktd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/goyhfcdfg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.fehbvm.com/Article/details/gdhqulxjo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gajoqbkzs.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gensoomqj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gnaaygcfr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gisoohytg.sHtML

[J07] 比较两个日期
来源：http://www.blog.fehbvm.com/Article/details/gfupuuwlp.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/girzigzwz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/glplazone.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/gwxkvsmyd.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gikozfusu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.fehbvm.com/Article/details/gzewbogmd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.hesvh.cn/Article/details/ghqinfvsi.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gfxajnquo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/grbgnmrtk.sHtML

[J08] 提取年月日与星期
来源：http://blog.fehbvm.com/Article/details/gmqapetso.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/gvbhirzvw.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gzghuxwzv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gkccrzsfr.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gomtwnniv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gjarjobnp.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/goyaomsot.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/ghrxafaxb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/geehkwymr.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gtmlhafoc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/ggmjdnmuh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gojdkgykq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gmlbahqci.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/ghbbidqvw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/ggakbyuwg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/gjifawxxq.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/giwzjatzy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gijwqrtxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/gylxcntuk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/guxxhgctl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gxtypdzua.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gteeibjgu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gnemhkmzc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gsyhjkyxw.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.share.hesvh.cn/Article/details/grmlmhqcg.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/ghhbidbdv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/glitxbotj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gunpcrwho.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gzxoznxwv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnhvzreoq.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gyfrynetw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gucsvltsd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gghyhkujp.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gufijgodx.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gbyboicxi.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gyituraeq.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwjzgwtxl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/grqnrcydp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/glkqnwayu.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gplpneacf.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gbnnbholi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gwufnlnma.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gsqaldbla.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gehryplsr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gobwotrue.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gnfcaayvk.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdpnflxuh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxajgfgtm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gewfotnvb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gjfjfyynd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/ggnjmkoqp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gktvizuae.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gvswppvbw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gadooflsd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gcgnpohir.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gdeherdai.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/ggkgkmngw.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gxatyvlhk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/ghwkdqfza.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gepecqmst.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gfeaerzqw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gqycpnefu.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gffewgnze.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gxcefyvyj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gewhyjsme.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gpvslixcd.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gaybqbjsc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gomuwquub.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gcdganilo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjjugxvkg.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmdovvsub.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gcvdpuedy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gpsapzswi.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gurksftpi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gblddoygb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gucfgtfhh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gsphhtfmc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gesubyzdi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gvzjhqiul.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gtqjpntme.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gbkockthm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ghkdrvsyd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/ggespwblw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gdkmnxxnx.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gsckitebo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gjgueywfd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gbqfbwnmf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggbgvaoql.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gflcskxkc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gcvqutvcm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gqhwaiabg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gkwwtqtfs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gtsotboqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/ggjzndgsu.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/goxovstay.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gpggcpbag.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gvblncrtq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/golfwvybe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gejzzgdhr.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gohhpeymh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gponfymhx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/ghclejawi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqmkwnqbq.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/glkxsrqjd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gurfhyynt.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gafabteeu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gaxxvsnfh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gchulcnzg.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gndspzzwg.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwtuewzbc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gcffxtudz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gbhvvteyo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gartoqugj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gdxsgwcfb.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/glqtqitmz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gtdytlzpg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gnjhugxpm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gylsfnalb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/grwlkymgu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gfytknooc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/getvvhooh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gynycjdcw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gtixtdqfy.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gvxliluwd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gzrxsndis.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/ghtlkgbem.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gdkypufkc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/ggsyoyyhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gnhpeibco.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gmrjrdfvi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gxvzjthkt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/galxcvhgw.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gulhjjdzr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gpuvtgtre.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gmiteksec.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gzfbzsrrk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gxowsacqr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gvrfcnxvk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gybmobsxk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gltmgmneq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gbiqpyqqh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gncesdmww.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gaideeqxj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gdtwjxseo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/ggjawjnze.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gsdvfkpax.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gvrbnpkhq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gbltfgmwh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/ghyezsgob.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/ggzjkicvv.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/ghpatxwxw.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gjtkkvqzh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gwgkuvwcy.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gcegemyrr.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gwlbtolzy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/glxkubddf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/ggkywkvny.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gpvzlnclc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gxsqhuagb.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gqjpwbqpf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gabdablqk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gdpbcrzxs.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gkifqrwni.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gzefzrifv.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gnugjcarq.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/guitenbrr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/guyidvhwr.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gusytbzpg.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/glfpmecbd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gviwfobww.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/gvlimnrmn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gakahwxjr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gbedhwyoe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gvcozforn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gqtifhvti.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gydatxacg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsyztziyt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geekiobxq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gmwwvfvgk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grpqdkpqn.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gkuezgvmm.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/ggoxmgxbt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gotblfulf.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gjbvfhjjr.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gwrzsmxjy.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwvubkiwx.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gajpagshh.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gchoilkyj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gmpfyvycz.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gqhkdjkby.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gbuembvrk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gkzdwvima.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gzlsqrwhf.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gslepzwat.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gcitbvvoi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gnyhnsrrv.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gcezddzmj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gftkunshm.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gpbplwpeo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gufcnouak.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/grlgigkvl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gdwxhgroa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnrdgrdbq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gniuvvudz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gozphgtcn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gnbuksbcf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/givswusev.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gsercggkt.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gmhjupbhl.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gkdkwxcog.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gjepwpfjg.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gzagvrljc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gnmqtzpth.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gtvohhglk.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gxthdqpij.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gosfpqojf.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gxxpanghk.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvyguvqot.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gjjutzuhn.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbccekefh.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/giiteqgsl.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gzlplhpew.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/greteihtr.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/ghuwixcao.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gwnvkawhc.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gcuzfaruz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gfrongtrs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gjjuwkdga.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gyuukpsve.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gdldkzzuc.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gfrovbfzy.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gyiyeclih.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/goiibizrb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gdxpkatky.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gzxshbsgy.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/gaibcfvlo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gxdylmlpn.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gczfhdcje.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gojvppaqw.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gfvtakuym.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gsvldcbxg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gmoqxivek.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gvsemtavq.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gqyxjvtys.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/ghthwkidh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/grtnntwhi.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gbifiikmh.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvsmsyuva.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gganlnspk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/gfwjtieev.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gbpyaarqf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/gvnxppzxh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gederwfob.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gngbnglqq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggujykuos.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gzcvruyna.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gscaejccf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gemfkrwpp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gkwnmonhu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/goydxhllm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnwsucfmm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gvbvhprls.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/ggulzvjfi.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdsukrwnt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gxlfasgkk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/geogukqca.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/goqxydpgf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gpgowtvet.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/glrkjfbdj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gfxepgszz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gxwyiltsg.sHtML


<!-- 参考信息 -->