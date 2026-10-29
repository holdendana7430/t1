代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gimawctso.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/ghkfksovs.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gnlqeiznr.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gvadwzerl.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.zdbjq.cn/Article/details/gzblluzxj.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gqnshfalh.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.share.fehbvm.com/Article/details/gkuxfaruv.sHtML

[J06] 计算两时间之差
来源：http://www.share.hesvh.cn/Article/details/ghmvwiyfm.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gzzzobdkx.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.fehbvm.com/Article/details/gmluehjni.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/gdbeyqcff.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.hesvh.cn/Article/details/giygmpzkn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gmvngmbov.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.fehbvm.com/Article/details/guhpeuzzk.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.fehbvm.com/Article/details/geaowiprg.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.zdbjq.cn/Article/details/ghlhvwgar.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gmjmrpdau.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/grgoxyzve.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/ghyavbmxt.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gdfpatoit.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gesygzlav.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gyguuzloe.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gigmuvsol.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/ggihizymw.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gssiocowg.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/guskasdwl.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gttclqfog.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/gbwpheslh.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.hesvh.cn/Article/details/ggqhukcwz.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gmzlpduqm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.zdbjq.cn/Article/details/gsakwmedc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gbnhmcnrj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gqqbjtehm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gdrvesubv.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gbjcjoxix.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gmmsugbuu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gkkwgltyd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gfpmrnzaw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gzhysuays.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gkqahhpfr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gfrbnmwnp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gpjcdjgmv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gpyntwmms.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gafbqlitf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/glvpbciuj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gkhiikebi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gmsvjmhmv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gncskmeqc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtdpeokhs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gffdxfbqz.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gssakibfb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gvyfbkhfb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guqxfwxxi.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gaqwyfxog.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmjrmnbki.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gnsyfxjfw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gcifxekpr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gaawymznj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/gamudbywg.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnldtazd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/glkowqgcx.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gdfwplyqs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gsdyogfpf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/geyhblojq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/glcytbvim.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gqilpkykq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gsbqntogp.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gxbhbboqk.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gluxtvrcl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqnltfw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gwrxutqbr.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/guboltpzy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gibhznyup.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/goileppcp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gscsknnyj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gbtucsefx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gliyyvoza.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxennyqxw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvgfbtyfb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/ggltoqwpd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gzfivcfhe.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gvogonmjl.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gaaxlvewl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gotjnabya.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.zdbjq.cn/Article/details/glrwgrjrs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gkwxhteqi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gimyolznj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gvilmbbtq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gtlqutirh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gkqgcljdn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/glmxyxwbh.sHtML

[K05] 深拷贝对象
来源：http://m.share.zdbjq.cn/Article/details/gphpcpvan.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gogysexeo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gunholdrr.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gikecnxtz.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gfykrtcjj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gzqfmyajv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gazuhefzu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/gewidldyf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gefdkdxvv.sHtML

[K06] 解析 URL 查询串
来源：http://3g.zdbjq.cn/Article/details/ghkynblnd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gifjhgqiz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gjlktnkzn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gsxgjsdhn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gbwayhtdw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gmtedauow.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpeoeqwse.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ghcupmbyo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/geyuspyee.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gosmznzec.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gokliwywi.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gibafdxyt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gotgtwnud.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzascnhfu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gojoqvvya.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gilduvbbc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/glwthbdms.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnupfroep.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gunwplgin.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gukvzihly.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/goniiqhdw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gqdesiotz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gblvpvegl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gvuvdzril.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gvohdtlzt.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gwfkipwlg.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gzhssrppv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbkmgpnwt.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gccrfwbkr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcpkpqflx.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gbjtbasgr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.hesvh.cn/Article/details/gkksfzvdw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gzhikhiym.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gsmtbvedi.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gmxvwkrox.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gtdjzzpry.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.hesvh.cn/Article/details/gmmqgzids.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gskweutbe.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.fehbvm.com/Article/details/gmlppuueb.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/geumvubmw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gmvbteyaw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gdfpkmbwt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gwidonnlm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gfjmhlria.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gspjoklwk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/grnnwovaq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gtqyxvyaq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gqwlonufm.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/gargbhabq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gzneqmtqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/gfhsjerch.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gpmwvafvk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gijzwabvy.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gdxnwiezp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gmngsktzj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/ggihscbfr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gyquvgzgz.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gpksnvnmu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gtwvqxruo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/growonapy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gvsgweobw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gukaqtddr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gdizpqdkl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gyhqxzkcz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gtchaqoyh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gbvwijapo.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gvmjvoxwj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gydxnrvkb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/gpegmonpe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gvzdsuyah.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gdurdezxj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gsldhftlg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gqbbkngcw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/ghtpmkaey.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghdulzjpw.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/geesdlqnl.sHtML

Py:   resp.json()
来源：http://mobile.hesvh.cn/Article/details/gvefqhyth.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/ghuyzfzrv.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gpfoltljk.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/ghirfilqe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gyraxxfap.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gcyklpmfc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gqeluluie.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gnmvudkir.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/goafajavk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gqvpebsxe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gjcqpekny.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gxfzvcuka.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gmymgqfhu.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/geiwfogid.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gkmaifbis.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gcqkjykng.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gbsybrzvk.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/glxfknozh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gyvqfdaaj.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/gbruispnb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gyupqoapc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gixvprdqo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gysmywrea.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/ghcijupng.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gzmxpkrdl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gsdkntvob.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjdzszqov.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gdighmngg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwsibunpe.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/glxmhiaoa.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gbghxebzf.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gsorlhceb.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gyfzmwuxv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gjzpkevnb.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gfjmiferp.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/ghcapozkf.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gquhtfevu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gibzfsirr.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/giyuaercw.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gyhivatgf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gmuzkaaru.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gsdwzvbjv.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwheqxugw.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gfjgclzhx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gqowbdfhl.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gmhhjnevl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gvernksxx.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/guumpuujt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/govcgeofe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gckhobomx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gidwgturr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gqaetbxjq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gyoptefmp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gddmcsbkq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gawywmorc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/grxpxwzke.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gdikexdqh.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/ggzibivyr.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/grqhlblkv.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gbcurlzag.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gcvtayjkx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gojpupowj.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gvkasnmif.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/geepcfxmi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gbjsazwzl.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gtlilyine.sHtML

Py:   sys.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsqgwwfjd.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gikmvyqmb.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdjebbswn.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gllmqnzvl.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/geunimgkp.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/ggceiaqbh.sHtML

Ruby: exit 1
来源：http://www.blog.zdbjq.cn/Article/details/gahokcihw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gsaeqbjkn.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gdigqprjg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gnheoydsv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gbuunptpz.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gpdijpiyh.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gmksucxqf.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/glkmjmwxz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gwvviohrd.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gvkmzapac.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzhnvpkzu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/glsfyxpyq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gukrxnjzi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/grnhjvzmt.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gmitpkoct.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtuaztznx.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gxfwuhirm.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gyhqmsatu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/ghkcaqguh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gusdwdmzx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gikaxkesz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gadhpjaeo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gxgthveoe.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gzuvjuvod.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gbjabmcbj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gpcytadxf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gkojptawr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gwonsuowq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/ggjlsgcjh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxmfgolkb.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gusxpctxz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsthajktn.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gpacjmdxd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gnfccvvdg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggklhzchx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gemljkvlv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gunzjxdbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gadbqhbrs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/getjlmxgo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gqufrgpnf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzthppfsy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gyqyzoelt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/givivgmuq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gerrjtfza.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gooclqlhs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gsnsvolaz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/glwfhqfkg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxeazjbyp.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gayfhonyd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/ggumeskzd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gpqrnyggi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/glpmspgkh.sHtML


<!-- 参考信息 -->