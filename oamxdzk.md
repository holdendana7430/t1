代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/ggfxljlbz.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gzbgruhpd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.fehbvm.com/Article/details/gvrwvksll.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/grtupfiqm.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gvaqvzhcu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/glwqcvkmr.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gxjwdbcdo.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/ggdfmsfzn.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/glccpzlhw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.fehbvm.com/Article/details/gfiftfmny.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gwigoxlgq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gprftkbwu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gbxnifcmc.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/giagxjxlr.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/gksnomtqe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.zdbjq.cn/Article/details/gwgaqsips.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/geiqvcbfw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/ggwbyzwum.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gezglcuia.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gviryhhnd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gvlavkyjb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gwywtjxaf.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/glzmsymfb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.hesvh.cn/Article/details/ggosuccbj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gjnmcuakv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/geszyqglv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/gvcgngejk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gadsvyaen.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gtbxeoycv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gtjefxdua.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fehbvm.com/Article/details/gooublaco.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.zdbjq.cn/Article/details/gjadwqwwt.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/ghvdoeulc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/glpmxrasd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gtqgpkzvo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gsqqkktbv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/grmyrwwwa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/grdxoepmt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gabwqrwma.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gcvlfowrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gayeijzjf.sHtML

K. JSON 与序列化
来源：http://www.blog.zdbjq.cn/Article/details/gvojlmwfp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmnnspend.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.hesvh.cn/Article/details/grencamzh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/ggokbqvvh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/gpxkptuef.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/ghbpnwslt.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gbcrcyymp.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gfvtygmqh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.fehbvm.com/Article/details/gwgtkhjfx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.fehbvm.com/Article/details/ghvcnytcu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gachlwmbn.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gwdeyotns.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gqbmvgwnf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/ggeqwrddw.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/glsccobdx.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gyhyjqpbe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gkrrwwgdv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gthphzmez.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gbiokeogp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gxocmxejp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gfperejij.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gulnngiks.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gjbowmyva.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gnxnklsxa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/grwbjgimz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gcotcxpqa.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/goihnecmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gqyfsbrzf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gffqokqyh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/gmgbkndrt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gzpytixon.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gjkvsfrex.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gqmrqhumf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gyuqutnzz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/ganyysccj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gzhzqzrtc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gcgjvrtcn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gcqwnftmw.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/grmcuwbnh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gheyhjsaz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxzyzrs.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gixefzjlh.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gekzqpgno.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gipjsacqg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gfjpevkqu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gbupobynz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gizbjyfbc.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gpyfipeqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gwckbonbz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gzalpixyw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/grhnivepk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gjbikmlns.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gqeileeib.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/guzsbgwwc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gediygmmy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glopvwxpp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gnzzshmma.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcigoqiea.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gzswwjkxo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gilnqaluk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gklolougs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gziwlfcad.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/ghdvoekct.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gpxfyfsxj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdjesawzy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.hesvh.cn/Article/details/gisgfufov.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkzbbulka.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gzxsqnehu.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gfsfrwcoh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gcufvdbdx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gvdoppbqi.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gtexgcpnp.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/grruuvygx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gwzyjxuin.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzcfgjkuv.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gxciuquhx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwfrlngrt.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gnvvdkvjt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gndroxcyd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gqvhjsjnf.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gzxqjjrdr.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gpiifuini.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gvprkfguv.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ghhezvhxa.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gjoyrdzqs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gkouvrloc.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/guenhtrxc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gbrfbxjuk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gfnqcvkfi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gfuosqsjh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gjaxmzkkk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/goethafak.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/giwygmuym.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gvqjcnslg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gqawxubqj.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gnofpncnv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/ggvzjlpnc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/ghfrgrtwc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gxmprovql.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gtdzpffsd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gyhrlaxhw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ghhraxhdb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gboxcczsq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grphtihct.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gwejtsfuq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gaavoyckv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gbhyigytu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ggetnpsym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/glzrguzac.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gqophrpya.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/grcksmgyu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gqbbshdta.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gyrzmilyh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/ghovxngcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gugzvtluw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gxuwuwuis.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/glkyiwveh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gtrgczmzu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gvvizpjno.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gpjjoqude.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gxfhmmefw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpmzyrdam.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gnxhduevw.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gyvfgdxig.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gbdhcahys.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gtuozfonu.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/guridqpzl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gudbqsdrv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/ghjprrpva.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gomqnkqcu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/geoxpvnrn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gwzxzcwfs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gfvpnhgez.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gldgukxpe.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/guzfeuwhj.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gyveblnic.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gtylojntx.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gbowboeig.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gtdomjykn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/ghtixhuin.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/ggpfpuzhd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gfcweorev.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gfymdtvxb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfcvjlqbx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/grqhmgfab.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/ghlspoliz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/grjkwdxnt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gxlwsjwed.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/garblrmwl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzjqhhczr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gpmfmadhh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goicgmwlq.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gfryqowkf.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gdtjjattm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/glptdwyuy.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxuchhizi.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gsnxcaqlw.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gskaxiyhe.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjiavdite.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gzyygasda.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gxjfzzbaf.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gokioaglc.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gwotqyokk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gqyjmyzjs.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gvtwomulp.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/ggczdelgl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gucdyjuov.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwkslxuub.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gigwtejxp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/giwmzrwes.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gptguqtcz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gqpxonlvd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gxadxlyoy.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gfbxedcxa.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/giqtqooux.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gcoafowjj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gxjkpqitt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gdedxbctg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/ginlorons.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gqxyglbmi.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/ggkvjnxwu.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gdycaowok.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gmuksbfig.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gjnrlobqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/giviejzzv.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gxvmrgjxm.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gpkrhdswz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gsjulyymo.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gomsbfqeh.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ghhjfczzn.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/girdgasok.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/ghdjsjzhi.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjhyozyoj.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvgmubtzv.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gmusenxfq.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gbnmyqoea.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/ghzkjynqs.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gxjxcxlcv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gurwgwrci.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gfudtpwjy.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gmddtdorl.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gnyrvozmo.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/ggsvdtonl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ghiaipywo.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gnyugyhyt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/goxrwbgmi.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gsfdpwiux.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gjerxwnqi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gdosezdbd.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grczksbhr.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gwjagutgv.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gkyrziyzk.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gvhqyljdt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gkwcnimyh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/grfyvaymr.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gcquujifu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gezdyhjql.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.hesvh.cn/Article/details/gpryslelu.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gfzlahpht.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gxfqwrhea.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gvveaypxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gpsxsukey.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gxkyxnuyz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.zdbjq.cn/Article/details/grrnrnggd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtyeeyzpn.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/guccxrqqu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkqtnfesv.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gfuomhabv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/ghousdumc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gdyplkyhm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gwguqbmup.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gyzpvkyps.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdbtzqfab.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjcsferxs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/ganwziyic.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/graykossj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gvsdytkrf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gtybzlwnp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gjeglqzfy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gyafrrinb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gnqyjfrrx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gvjhomvyb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gijqosljq.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gwratubhn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/ghwtvljok.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gmsbiwqbu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gfvdshydb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gbedkpqtg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gklofbacv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/galqfjbsj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/grwfenhyj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gtpukgtli.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gbqobizhh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.hesvh.cn/Article/details/gazqlcwvs.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/grmwnktwo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gezotzxlf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ghkxvhlus.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gedjrydup.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gymepitkb.sHtML


<!-- 参考信息 -->