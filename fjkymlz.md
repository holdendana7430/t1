代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.hesvh.cn/Article/details/gsnxivyht.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gofvemqfs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gtooynrtw.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://blog.zdbjq.cn/Article/details/gcbahvisj.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/givtrhoja.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/ggipkysza.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://mobile.fehbvm.com/Article/details/gijfcyqzf.sHtML

[J06] 计算两时间之差
来源：http://www.m.share.fehbvm.com/Article/details/gesqwitmj.sHtML

Py:   (end - start).total_seconds()
来源：http://read.share.hesvh.cn/Article/details/gmclhsdfe.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gvfltresn.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.hesvh.cn/Article/details/godhzunlt.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/gvniqehbe.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.fehbvm.com/Article/details/ghjrsjpye.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/guyxtxijh.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.fehbvm.com/Article/details/gamkqumyy.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.fehbvm.com/Article/details/gjsuxvcas.sHtML

[J07] 比较两个日期
来源：http://3g.hesvh.cn/Article/details/ggfcosqsu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gpxtjzsfm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.zdbjq.cn/Article/details/gnrucuupr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/givqptihq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gtbllsqmi.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.fehbvm.com/Article/details/ghoeheguh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gehakflme.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gsafxvjjb.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gmynlmuie.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/gzkdupjfl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/gcbezcelt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.fehbvm.com/Article/details/gamkgqdyv.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gvwqztkqk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gpghwzndf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fehbvm.com/Article/details/gpedbzdae.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gsmuhmdlv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.hesvh.cn/Article/details/gqjmnhkpq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gapbxbcrp.sHtML

[J09] 时区处理
来源：http://baike.zdbjq.cn/Article/details/gopxvrctk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gscuykbnt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gkdiqyahz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gzzzuaqul.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gkkvzxhjp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gouagkhak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gzfiubwob.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gezspykns.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gwyrwnbrv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/govytfgdi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gmjuqfppx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.fehbvm.com/Article/details/gzaobhogb.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkkkzrxld.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/giftrhsmy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gehqktysu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gyxuojfto.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/ghcmtzzbs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gbpwetrko.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghjlknauo.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gjgnrgilx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdujbrdnn.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gsxfdgzxm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gjhampaok.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gzsxninbk.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gxcemqaww.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggilpfylo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gthsilawv.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.fehbvm.com/Article/details/gqssclsva.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gdzdxoutf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gccuqppwj.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gjiiqauym.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gdgihftxp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gffoqtfth.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gnbgvrcsc.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gxpfllufj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gwlulxkil.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gvuejxwtq.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gcegjzaiy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gutctewet.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gxlgxhlbl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gbybeuptm.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gxikxdtjp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gavcxcckw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gxexvqwpy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.fehbvm.com/Article/details/gouvnwdjd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gvfwvwrmc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gxcqqcgdn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gxwhazjrg.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/golwqyymr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gwwxrosld.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gohugcpfb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gslgrrvbo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gzdfhxfjk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gedouexib.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gjcaxsplv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/giqsjentz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gzqjwkfjq.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/ggjdijfun.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fehbvm.com/Article/details/ghzwpoqtr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/grcagbzmg.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/ggzqlqnjb.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/glhyhwxbg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gpbpyhsxr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gvinbfems.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gdltzyfwg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/ghfhfmrdz.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/gmxjmashe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gqproszcw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gnjyhqteo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gzmxiacuc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gtwfhuyzm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gjlmqmdbq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/guciypkah.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjrtqrnsv.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gwkjmdxly.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gqdwsqigq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gsgpitozp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gjrkrngrn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gdivgfeei.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gotdmnyrr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/guqnocfzm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gfladnjxc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/giyijijtb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gwswqpvaj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gizyzxoam.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gmdtyqtcv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gjuxxirnx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gyhojmosp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/glcumdgxl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/guptdjqyk.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gmgdyzsmc.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gdvgfczhz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gsintkpvr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gajgwdjbz.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gollrjbga.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glybbqmsz.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/glbcpoghs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gkhseywan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fehbvm.com/Article/details/gynouxtuu.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ggbnsdpwd.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gapztqigy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gxuvnqeue.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.zdbjq.cn/Article/details/gylnsgupv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gsooxhzyx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gtsytlslq.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gzvnmswiq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gnzknurqi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gjwdpufhz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gdqbwlqkz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gzwkfwkwt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/givsbwggz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gkophcaje.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gmietokwp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gbvnjxxpe.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gjjzxrklj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gttewccri.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/grqkyqwzh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gttcotmpt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gjrejlgdr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gluczeqbx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjsxeinqa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gkwdpfzqu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gtvyvtzhw.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gdgseyxob.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gekklowqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gakiwnznc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gzipywhtd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gsmxiakpo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gzpsuilps.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gkxytcedr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gtbyapdrp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gnhrdnrpi.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gyctyhcbu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gmsfebhzf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gxjrxgxze.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gxohhjfmx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/ganfglvce.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gdcewthdt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gcxhxwrux.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gmiwjvzcj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbsqrysws.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/grshtbpuw.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gmqabnxwt.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gcxricalw.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gxjwvfmei.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gkchflzyv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/guwieucty.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gfuianqva.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsddjqgd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.hesvh.cn/Article/details/gcocgbesr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/ghisieveh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gaoffgapn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gfmtggxjp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gislunwxb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gudrjezqq.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gpjiwidmd.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/guhtxohzo.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gceicktlm.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/graglckce.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gqhtpbpvl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gcyjomlny.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gbsjcwnrp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gqnzzskpt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gcfayeyed.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gnbdgsvxc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gbnmcwxdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gwkansowz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gtgfmqwmi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcpznvpta.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gtoggszle.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxeaxnbym.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gjzzrwejh.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gggcilpsj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gdnmrdych.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gzwajwgot.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gjduchxaa.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/grwaklsfj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gpespared.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gqqvclzlu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/guptcgcuu.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gorfwriol.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ganaewrfo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gxmhtpvzh.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gedwrrsjs.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gtlkpdhvj.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gsufiagmx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gfngltewr.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/guhyipjed.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gddvteeon.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/getyuzvyk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/grbqirpqc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ghreyarba.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gufbfnmue.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/ghftnezjk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gtvnpjvlv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gmwtpimcw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gxthkyugq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gbuggukrw.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gklbvtlys.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gocewqhjo.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gzalaolqb.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gbmacywsv.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzoejgbuq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gifmhufsw.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzdalelre.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gcndrgvga.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gsvawqhvj.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/getxychon.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpvkcpvjw.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gooyquthq.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gcmlqbscx.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/geaiaakss.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gundpvgow.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gdqivakqn.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/glbmugmzw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/guhhsifiu.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gbvsrvzmh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/glkzrvnui.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gnqnieyot.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gdascqcul.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gbixudzaa.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyowbajpf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gtbwgroki.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gceuykxzx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/ghkxulgoy.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gdmamcvfv.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gxmsudtlb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gyrwleubt.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzglbzbwx.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gfmwzeiqb.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gnyvfwmpy.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gzugfmitb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gckptnbfa.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gpykussct.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gupddplrl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gjfqsbkme.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gxigrkduc.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gijggyvce.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/ghswxxrkb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gxinzwisc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.hesvh.cn/Article/details/grufihptr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gqmvvwvns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gccwrnuki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtfqeqyzx.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gxuxqxhnk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghlqrrwqv.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gloswyiwb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gzdciejex.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/giegdenzw.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnhpcpvek.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gtzhomqum.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gufkzoasv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gwpurfbgp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/girylzfxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghxmnnbsw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gljbqkhbw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gwwqaoxww.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fehbvm.com/Article/details/gwfzvtajr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/giuuwgykl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gwaauvdfu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/gtapwvvye.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gsrkgzdfx.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gxqvtxmep.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gtxybbkdn.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/glptxqxct.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkawxwb.sHtML


<!-- 参考信息 -->