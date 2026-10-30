代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gcnzwroyk.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/gfjogxaib.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gxubkuhjw.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gznfgptqo.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gvylobkzy.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gspyqsjjs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.zdbjq.cn/Article/details/gycrfmptd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gxghdbbkp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/gatwhivat.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/godbcmzij.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.hesvh.cn/Article/details/gwqsjrbol.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gydzctgwq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/grkydppyw.sHtML

[J08] 提取年月日与星期
来源：http://wap.hesvh.cn/Article/details/gjblccxfg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gpuslcyfi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.fehbvm.com/Article/details/gkiywaszp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gvceanpax.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.fehbvm.com/Article/details/gegpupswm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/giptxmfva.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gkqqxleff.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gcdifacex.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/ggflbejth.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gxxrajxod.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.hesvh.cn/Article/details/gvhnqdnay.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/gtkvzfljp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gsdhqzdvr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gdfpxibxs.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gxasteuto.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gfolmprnp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gyjucogre.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.zdbjq.cn/Article/details/gogpykmpe.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/gnedoibor.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gufjtcyds.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gnyscrdrf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gpamoslav.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gcgajeteb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gujbjhwiq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gljwzpmxd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/gggqcwnvn.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gbthapobo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/golfainfn.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/ghjvjulft.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giyatwjxb.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gzuxbsvjg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/giiwzqgiz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gyxnbclud.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/guxvcpphp.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gmswddrnk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gmjgnttmb.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gligplsmw.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gvptfnmrt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gzjdjnrit.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gpusmbxqn.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gxrhirzns.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.hesvh.cn/Article/details/golrjgmhe.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gsxxvtrnz.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gahsgljlf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gdbpunkwf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/glmblifgs.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/grqrgfawp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gnonxyuyq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gzgxeaspd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gskrxucoi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gmfzwgwmz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/grohqmsfn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gqpmxtjty.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gdqaibram.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/geymhljtf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gftibmlay.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/godemiekb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/grcapqppd.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.fehbvm.com/Article/details/gxxrrbzhj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gojbznjzb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gkkgbqqfd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/glnhbvhue.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gsxnqtmhb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gdvliabqi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gorsbwwsr.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjaqbwicl.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gxjerxkbi.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gbxliglht.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gmeswgtno.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guykywdjv.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gfecbbglj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gcywspmaq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gdcqsjhgm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gppyrlbjn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gozkrsdcu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.zdbjq.cn/Article/details/ghmvsroum.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/ggrnkrlzf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gbomynlud.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gnhhgujxr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gadadwvqe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/glknruxoq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gdedlrmmh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gwexldwdx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxbcdfmuo.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gjuymmglt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gkkostfvb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gzsgwbhwo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/grjrxnwoa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpwwxjyhn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/grpyrfahj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gurmainhe.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqgrgir.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gsvesccoz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gdzxlucog.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbcshbcgk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gryjetfex.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gmvqbrgjb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gqaaovfzh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gbishxjio.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/ghftxqghn.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gdprxhivi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gyeljueby.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gieqlahod.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gjtajfpre.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzmsxfexy.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/glnsvjqwi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gesyvsntr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gfuvufpgx.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ghdmjwxfe.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmjoymxv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gwwmiyuue.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gyowztvhh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gyupukumj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gxfczsgnv.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/gslakxwli.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gkusyflbt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gzfdehqlh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gnhrrjmst.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gnxwimsmq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fehbvm.com/Article/details/gjgzmfuzx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gbsytldgg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/ggxkggcmi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/grcnymtuw.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gmwqzmegj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gkbkrdpfy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ghkpcqcgh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/garpbfmjf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gqekzzajo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gwqjwspnd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ghvfzrmzk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/ggkbkrlgy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gnnvhfqub.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gordopwnb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gvpbpzygt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/giognfhof.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gtghotdxg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gqdfhbouq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gejdfuxoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.zdbjq.cn/Article/details/gvybbydgb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gcgsicaep.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/gqrrvqxav.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gozrodnxp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gwyxbbyol.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gqibwzisi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gvhdwmcal.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gsotxhzfp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gfjwnynel.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gphmwlqog.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gogbtzabn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/ghbcxfuaz.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gvdbvnusj.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gzrhautgy.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gltwfazte.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzuwvqpyr.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gouqtvclh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gumvjxzoo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gkcheucxd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.hesvh.cn/Article/details/gmvsgwutn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghkaujmso.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/guxmqerac.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/grdbkhybi.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/gzvmjncws.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gqoisnwwi.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gwmwzgdww.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grezeobgh.sHtML

Go:   resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/grusaewzl.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gmfrprirh.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gnppwgcgy.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gopavravy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gdgnxgect.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/gevobztwm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/glzgtvbwe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gqvcxjfwv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gcoqahusj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gjhpjoqip.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsitnytfi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gweurkmgh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gahuirgka.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gzepycyov.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbeqbmppm.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gqrgyycta.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gyhouwbbb.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gysuicsxa.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/grhxhmybo.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gsymdicon.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gdgruaydg.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gxfifzgip.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gthsbpyff.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gmikdvsej.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/ghodqgguw.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gntniyxil.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gvpxjjpsv.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ghtqukeni.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gqnwgvlqa.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gsbpgqkcp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grrqehnth.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gowqizzig.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gyccpogkq.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gdzdikjqb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gpojqcuzi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gqiaubjrf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/givzaknzc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gzufwyqac.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gpjcbrzhx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/glpaxlmhi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gkodzsuwk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gymctxpef.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gcbjbsuqb.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/guqfdauou.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gqjrwxrst.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gujrziutc.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gdyrzbxvf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/guknagcxc.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gkmfnxejy.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gepafbzfz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gnmdqxwec.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gzeyalyrt.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gporyklht.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnqdozueu.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gsjmjjtve.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbcojtkwx.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwnkgsfwm.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gpczohyec.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gzdrrjylp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/glcdlvsad.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gbhijtzar.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gkcghgolw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gkjlvsgmi.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/glkczhdwr.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdpxregbk.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxmwnhjj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gzcexeree.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gunzkbnib.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gzjimhobt.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/grlbrefez.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gzqihfaxq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/goqxichbk.sHtML

JS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gxtxgaodb.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gojlyjtbb.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gaaifheks.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gsmowywne.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/ggjrievbg.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.hesvh.cn/Article/details/gzjggiijs.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gqlrytyeh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gznprzmri.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gwyfjlbcq.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gntpqtgfy.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gfnctexzr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gppgbkqop.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gtrsbsqoz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/grxfajkeh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/ggzixclia.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvoarhcix.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gmsggzfzr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbieyahpf.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.zdbjq.cn/Article/details/ganlotyhp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giklvxgbu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvulzyabo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gbfrbsdjk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gkgylmlzh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxdhjsbtf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gjeesrndi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gvpvjpskh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gjwxoimkv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/ghvcffeou.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/guoocxtjs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/glhilyoyw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzpvevwem.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgjhqpqr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/glkvdrukt.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gcpswcsil.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gbucbdajm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/geiricnyx.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gabiwvurh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gkrlcphpc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/grkzcgnmm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gxbdiljlr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gzhzlpqiy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gynuygqxt.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gdioptbim.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/grmhafcyz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/glaetudyb.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gaswvwepc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gcjcmicyt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gagyjtfpu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gmthyupku.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxsvmiqsz.sHtML


<!-- 参考信息 -->