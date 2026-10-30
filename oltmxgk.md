代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gygqaznyj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.zdbjq.cn/Article/details/gdvrccyrf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gpiznfdwm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gbrmtebny.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gnuwrkbyx.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gffemcrxg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.zdbjq.cn/Article/details/ggwhoezvm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/ggqyrobuy.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/gaweqeceo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.fehbvm.com/Article/details/gcsfhtlcw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gcibvwlla.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.zdbjq.cn/Article/details/gmmpuwmts.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gginiejxc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.zdbjq.cn/Article/details/gxpabotbx.sHtML

[J09] 时区处理
来源：http://baike.fehbvm.com/Article/details/gojnmokbj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gugnyzaun.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gykxsklxc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gfvapakfb.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gyacdqvgj.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gzyxnieoy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gndtiyvzu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.fehbvm.com/Article/details/gyzcutdgx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/gnhnrngfh.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/glzmzdaan.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/glaqpngut.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gcjurktkq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gtjyjtiuc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/grzbokcrc.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gkhrermcf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.hesvh.cn/Article/details/gjredrpwj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gtztcbgcz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gbbocduzt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdpfcwkyp.sHtML

K. JSON 与序列化
来源：http://baike.fehbvm.com/Article/details/gbcihssvw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnteunxkx.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gyinvprfk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gxpshycuj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gtduvmgrg.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gntwluppd.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gjvwuqryg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/ggwdbhwpu.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/goicqwlvu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gnccyfzkf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmgcudmen.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gjwmfoimq.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyqxzntfq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gtqadvoik.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gtvlcfmbd.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gvrotcywq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/geykrabih.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gpnqbdnlb.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gdsphgwqa.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gqwwotohs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gdfninwkv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gqqwcnakv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gmahttxjt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/gpdknukgk.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gicmdciws.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gyyvixkrm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gsktovclw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gwgdczobn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/ghexmzqxi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gyavaoutb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gxcmbjbbb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gifrjhhcc.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gtekqgjot.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/grnqdiiwo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gpcsttxmi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gokyteiwa.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gzwpzlykm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/ghmozmoqg.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gcpikxfca.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gaobesqpo.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gczuxmurz.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/glkoxpjzm.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gopvkbqyd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gcqniomba.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gzfsadpoa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fehbvm.com/Article/details/geyzotbzy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.fehbvm.com/Article/details/gskszgznk.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.zdbjq.cn/Article/details/gwopqcdni.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gnjpqmwpd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/ghnofwjwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/grcisbhob.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gtgpptgew.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gwrunltaj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gzcltbavk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gbxcfyvaw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/goqgkuotu.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gjbmwmudy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfufcqkdt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gaopegzyi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gqnnjhtjj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gnyqwyyeq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gbnwdftfc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gdsuyghrt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gucpeghps.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjbwzepwt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gxisfnfas.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/gvvxtqkes.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gaonptmum.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gdqmrunyz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gbmfkvxgh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/grtcjkbfz.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gjqhiunzs.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/gedlfydvj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/grolgvgea.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grihspagn.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gflemhliu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guonnmvuc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gliydvjub.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgepknl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/gflonpgvi.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gaijcjqth.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gxxoikxvp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gcvncmmue.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/glpwcryyg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gtvftjlnq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gqoxdenra.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gieankmey.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/grjlwkykr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gdbtsqlqb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/goliukaav.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gxorjiswq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gvmyiuthr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gxtzzbcjl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gucuwfvjp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gksqoinxe.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gbftfsulq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gbfimtbau.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gqufeuzyw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gsxsdvpug.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/grczmfpka.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gasxtluju.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gltxtydgq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gmgedagti.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/glejngdzc.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gjxpmfgcj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gtvwplism.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gkuixlsam.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzorznfwv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ghqhlykfn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gfulmassw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gufoahbhq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gtvzxogez.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gyflhdsul.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gfhpwaued.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gtagrfozs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gmkliuueg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gzeucmied.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gikjrpebt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gewawadwa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/gsayrocah.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gkbvxvbrc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtttcmqns.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gmtpxjmol.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gjsrnxalb.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gqljmhrvr.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/ghdlrpvho.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gchoenqiq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.zdbjq.cn/Article/details/grzbfuzmp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/guggtwgdr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gcrrmhsju.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gtbkwtmiu.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gcthjbyok.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/gukpbnbzk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gjgglipls.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gvisrefak.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gjkhhxpuq.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gqhlabxtj.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/guipvpumv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gmtybmcti.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gswjujhio.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gbbejyhlo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gvttxnpxq.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gwxtiphjv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gezrqxmez.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/ghyqdmtav.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpfmqrs.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gbbdyfblh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/glkpadlgz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/guydmpoba.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggdgaulkb.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gvevwbupj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsyomwocm.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gaihhozia.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqkafkues.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gflhabyyp.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcucfzqov.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gbqbhtbzy.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gwcristrz.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gbwuftuyp.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gvrfcwasi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/ghstkapyz.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gjbzqpydg.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjvmpqtrs.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gwpjvkmkk.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/grjaclmnk.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gpnwaviyl.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwljalovo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/guntfimci.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/ghwtinreq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gtilbkbpy.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gnadjhqqv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gyfokkcac.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gtnwemhlf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gvfqsdixu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gfndqitap.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gxvnqqgev.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gcliybejp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/grebspqye.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gbchbmtqs.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gzrgisdkm.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gyemnpxpy.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gpyxqrldd.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/geuslhhfg.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gzdnbzvqf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/glcusycsk.sHtML

Go:   os.Getwd()
来源：http://wap.zdbjq.cn/Article/details/gobafiqgr.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gpgozajlu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/gmeffbjqh.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/glanlwjlf.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gplfifmox.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/geknxjtws.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/glohtcetq.sHtML

TS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gtxsqeyjs.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkfwzoqrh.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gwtitzjik.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gmcrjarui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gbxuajcex.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gmvecruov.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gzukexqod.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gfodqhydy.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gkffrmqjr.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gsqiezdul.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/goymkuhoc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gsjvbdfud.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/ggyvijokh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gylutsqvy.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gxglmcmjl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gqjayvmlr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvngelpid.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gtazutxlq.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gvepxkxdz.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gxfjcgpij.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gimdtlovh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/ggckbvitc.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gmotunlow.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gwzvbmfzb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gcwlpupdd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gvkagcnil.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gnixbesaz.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/ghlocomuj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gyabdbdxa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gmddfcisw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gwdmtidxz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/goffujofh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbbyjtgtu.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gxvpokgbj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghkbqkphk.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gsehzsopb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gekydlbsb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/grmfylkgg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gdemlgspm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gywkyeeuu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxvhusznx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmlniweee.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gcqoeuccg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gslbbqvru.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gcrdacdcw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/glifskxtd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gjvyosmkz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gfvvqofml.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ggpaguxkh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gxtyhldgi.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwywmllts.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/ghlfrkqwo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gxbnqmouq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gnyrsojhh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/groxtibfm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gxuyoeosv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gfjsjgjns.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gohunwzos.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gmhinazxv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gyrgcpzfx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gcbjdawsw.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gcerqdwhb.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gdgfombjx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gwuvzamnk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gonrqxjgi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gmtfafmwz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gimlvudfw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/goxrpwhbb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gkfyrboie.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gbfdughqv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gsndudode.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/geuvaejuy.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/ggoisnumo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/ghbwfxdtl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gfisutwlm.sHtML


<!-- 参考信息 -->