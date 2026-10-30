代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.m.share.hesvh.cn/Article/details/ggwvrmxka.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.zdbjq.cn/Article/details/gfgirxdik.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gzjkebgzq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.hesvh.cn/Article/details/gmhatwsur.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gsgeegfmp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gtwgmhkuc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.share.zdbjq.cn/Article/details/gdrmshohr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.fehbvm.com/Article/details/gcfmabsas.sHtML

[J07] 比较两个日期
来源：http://read.share.zdbjq.cn/Article/details/gsnnrpkyu.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/glzkwffjd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gvokqjvgb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gvsckqvqg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/gnjqnwlyq.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.zdbjq.cn/Article/details/gcqijavtl.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/gsvvkrtdk.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gjckqtsdp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gmwgpxnzo.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/gqkmdixbm.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gfdrewvma.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gvxptgyhz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gcnrhbrzl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/gxmbgisqv.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/giudbquwb.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.zdbjq.cn/Article/details/gryjuburk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.zdbjq.cn/Article/details/ghwdasqlr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gmrywcfen.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/gmkilwvof.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gmgysivga.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gwgepxgsa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.hesvh.cn/Article/details/gamigwzla.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/golfryfde.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/grkrvpyxn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gqapuwcay.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gufpjrziu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gmerpushl.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gzkmfmonn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gickorrwl.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gzbfcwaym.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gunnchvni.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.hesvh.cn/Article/details/gfrlzqwni.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/guwhgyims.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.hesvh.cn/Article/details/gsqvmavql.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gbwlrvwsq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/geuxvlhll.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdgkxppuh.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gicmxynzj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghhfwtkvx.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/govbmvdlx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/garxrjfjy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcisqaqso.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gbbkaypft.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gzqqrlbzd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gqxeenylt.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gmcxqxewf.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/goojvzxmn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsbksgbcf.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gpbubmblh.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gdrpcmrzt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/grtyejgrx.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gzqegejnt.sHtML

TS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/ggaqxujoq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/glirplngo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gekllzcta.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gzfbzjcxb.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gvfrpjpms.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gokintiqi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gxskrskio.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gdhkrywko.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gtnsyrlxt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gplcjmwmj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gbsxmmaxh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gzeaxewxe.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjlettxqt.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gmftmxtyi.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/grvpoheiq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gansasilq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gmbzpjbbn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gamwvmaqi.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gpmcbxcgh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqzqrukx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gghzbjzla.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gdxddmhxz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/getxgroza.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gimskqsoi.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gswezuvtm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gtzqpzcro.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/goannmjrl.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxizbjiga.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gvlqqdpvm.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gieimrpur.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gxrxffwmj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gcprhiqtj.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/ghwzmilrs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gonwjblgx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/ghdnhntsv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gcputounw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gcxeipuqw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjsrbeapt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gwifkrfcv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/ghhrnglhu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gficwdymm.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gelllffso.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gmojfegct.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gvlnmurnh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbrnbfavo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghbatbcsg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/guaxpytkz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gsziuejpl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gwsvxnrjo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gzifhqbzz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gindbihqy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gncvzrrcn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gtudgjbcn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gmnmdfgzd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gnlperbgx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/gtkaimmdo.sHtML

Go:   encoding/gob
来源：http://blog.hesvh.cn/Article/details/gcdkuajdk.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gvkrvrfvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gbgfbhydc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxynxkdrv.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gshtaesll.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqyshhifn.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gndxadpin.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gdhjbnawc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gtzroijnm.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gqwakfdai.sHtML

TS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gdrhousnc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gvzospapw.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/geccwsysr.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gdlyzpfvg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gdikovthu.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gnfsxtyuu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gtvehzanf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gxwcnmazk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gpovvcgzt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gyditjslj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gljhbelrq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gqjhrxxop.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/grgujzwdk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbwnkefeu.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gafxaaayi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gwwbqwxhp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gcvhtajuv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gzckrxfvu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gajuczscj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gucpsjgvd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/ghyjiubdf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gavqtumfs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/glnlosocb.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gdzlfnbce.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/gmerbqwiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gxrzggdaw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gmpkretsm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gnccwfmym.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gltvdtalt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gqzjxaukp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gxvcyfahi.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gzgmuklxz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gkyxyonmk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gawqmpfbf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/givbpqcub.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gavwpqdiv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/giwitlevx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gytxseqrb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gcxjcdifb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gzaycdytu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gunxperxh.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.fehbvm.com/Article/details/gomgcksyq.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/guhytzufx.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gcvjpiunv.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gwvkhztwp.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gnfzoxjsh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gwlrdoxur.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.hesvh.cn/Article/details/grlyuizpm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gxxnuhlod.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gqosypppg.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gobdikaqa.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gokkzwkqn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gxpydscbz.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjawhxnle.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gzkbhoanu.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gldrghjxn.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyozgtkhr.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gkktoapjz.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/glungdjjm.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gjpmwytcd.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gbzrxglgc.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gdkpgheoc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gjyywofwo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gptuqrvmi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gbsjnzrpv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/grjtkwcsm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gqlfejorz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gfttcodlh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcdjrikcx.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gtdgshgdf.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwastgzp.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gqrcvgfya.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gpnwzqpeq.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gicknepse.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpfwknqme.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gqsxzgqmz.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gebafvili.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gwhivcwup.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gkfhvtsem.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/grcopcanb.sHtML

[M02] 读取环境变量
来源：http://m.share.zdbjq.cn/Article/details/gxbzgezrd.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gitmjxtwm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gpbogmdxh.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gqullpwci.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/ghdwxxebi.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/guovlmkwd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gqrgavedi.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/grjucymex.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/griwpyiuy.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gdqzqmtrc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gubjzzgzo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gikozndje.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmejsunmy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gbubkssxz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/ggzarrwxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gaqfirfom.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gsxuwgwsu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gqpjxzwme.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gimfxbmhr.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gjzdtjmcb.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/ggkhotmfm.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/ghvtavnch.sHtML

TS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/ggduibped.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gwhlklltu.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gwmbfumuk.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ggvayvubm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gggehrqjl.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/ggsnbivsx.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjzmhmuin.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/guastwvmb.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gndugqntd.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfgfwaxrm.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gwlyxtwam.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/goijmhfyo.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gxmvtirsc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gmfullqzu.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gpntaqmqr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gkfnsyayj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gyenajrdx.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gqoitwdwc.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gbzfcdysg.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gzgdaatey.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gyeyrpbkx.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gkodhncqy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gqiiwmnno.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/ggqopziog.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gmecvueuc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.fehbvm.com/Article/details/gpskevhfz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gvjxyhpkx.sHtML

TS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gbxydttkd.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/glahpeosf.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gfwhncfel.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gwciewtii.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/goddbqsey.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/giqxeggcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gkorxdejy.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/gdzbkujga.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grkswjzsa.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gqpzfoiwq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gyoypsfdt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gorzzsxjj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gxfmyhqch.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gjhjdshax.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsmoqiesl.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ggriclofg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gznuaahnv.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gaayzmetm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/giwnwfrur.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gengvmofd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/glfkzadpa.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gubmuawwv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghusgkypd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gbguehiqs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gentqmziu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gaklsvfnh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gkmgruzrs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/ggvkosvho.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gqzklrvgv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gquyouxid.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gcuvnvcjv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gqaydnept.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gbfffislg.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/glhpijwhh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/giowtnxqf.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/goyuimkjv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gxjxdzzrd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/grmnuehbh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gpfvxinjr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gxjdpdtoc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gbsyzjjbg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gztiklkyf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/glbtcynum.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gxvjykivd.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gndpnvvgr.sHtML


<!-- 参考信息 -->