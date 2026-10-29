代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gxngagghl.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gafasyzcy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gmbicwjnw.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gseazfhmc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.zdbjq.cn/Article/details/gzvrpinnb.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/giiufkqzw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gabtgbuia.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.hesvh.cn/Article/details/ghwfizxjs.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gzmkkbzym.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gqcywkrdr.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gtsnkocrd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.hesvh.cn/Article/details/gssbnrrqk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.hesvh.cn/Article/details/glbvvtiec.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gwsmeqbmu.sHtML

[J09] 时区处理
来源：http://www.m.share.fehbvm.com/Article/details/gnmvhjlyo.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/ghficudvf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gnozfmdgw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gjeqlzilt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gcvwlcbyt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gqqpklhtg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/glsbpzosf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gnmtbiyqi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gzlgmmevw.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fehbvm.com/Article/details/grkhlzzox.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gigfsqwdo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gexwkzdhw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/gcfgprzbe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gqskhkfnd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gngpalxhr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gpiqfcuyf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gtihgldwk.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gzrlpsija.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gplynfcop.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gltioxnkr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gouwgktev.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gtntlkwcm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gcsuhtkue.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gxqgfubxm.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gkouvrgpo.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/goggsienj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/guojosmqh.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gqwidaxrr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/ggnzvzqgn.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.hesvh.cn/Article/details/gpdcabezx.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gvgeiqxrf.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/grdofjwnp.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gggewlrpn.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gumffnwjg.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gsycwzktt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/giclzwmkw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/guxvllggv.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/grwqaujqt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/gpzswacjy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gietcoavb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/ggrpamjmh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gkeffgfdd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gveyzqbko.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/glznilhhc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/goxvoabmj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gupjkpzlm.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/ghhtuowns.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/glfubicyh.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gbrokumzc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gjqxetzan.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gagwskblj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/guikmjtgg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/grixzhfql.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gcmscfurn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvykhme.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gufnrpsjz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/ggtjinzmm.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gjtdzrqre.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gplippdpl.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gutixpffx.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gxahfwgpc.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/geywqrzbv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/gtvffkisu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.zdbjq.cn/Article/details/gmhvmdtgc.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gsxoloyiv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gdizrceho.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/gntguiled.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gfpdtdkgv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gecswxhih.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/ghtebytmo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gzejafxbb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gcunybwqh.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gzhviwxrt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gijbqfyto.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gbvrlhmoy.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvpbygrkp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gpeuxmeew.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gggsixjkr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gibyxjjdw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gwzdfsmmn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/geafgynto.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.zdbjq.cn/Article/details/gksyxzpvh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gzblufcld.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gmeaktzrg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gdvzkewam.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/grhrwsotu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkvnilcqc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gyyhmbftt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gayafpfzp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gmugkbkzf.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/ghqgpcyuc.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gqbqqshwn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gqcmurmpu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gabacgbkv.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gwukztsaw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gejnnjkzp.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gtahubtyd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gaimiyjia.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gwgeqpsqv.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gvhbklvyd.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gsiyjzige.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gbknasxhs.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gwwalgoqq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gwrqldsmi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gvffpudaz.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gbgctlhov.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gdhbedeyj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/grzirqnkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gyvhvlkam.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/goaqrmtaa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gjkmdfhth.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gvcecnejq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gvsfjjqnv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gbaexrjab.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/ggzvudovo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gharutdoq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gnczrpamm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gqtllydxb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gumczvtzm.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gfcwqowva.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gqpgozntr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gsjzybqnt.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gldyyvvsk.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gefnlgqyh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gcalvsrss.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gidvagrzu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gdokfvekw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gvivarzbr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gmwyqwaql.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/guqcerxup.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/grhsniqot.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gehpztlku.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gduairqcj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/gjdshdpbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gugwhcstl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/ghojoxeyk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gkqcqfszx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gduzgaruj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gccrdldpa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.hesvh.cn/Article/details/gxzgrclmu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbgnrrzyc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/guhkzkcod.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gjumbddqg.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gvleslyfk.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/grdsyolai.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/goplbnhdw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gthnckojk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gqryzfpwd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/grrasuith.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gywfeojmc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gfktkgcfb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gihknecsj.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gkqfqbhaf.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gmnpqckjs.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gvrhzxupq.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gunpjnjdv.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gqvhssfyn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gswedeeed.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gaqwslave.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/ggqzuizgv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gwhssslcl.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/glcflsjyr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gnslbrkdm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gdvzwjnpc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/grryuweqf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/glqdofklz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gxlbvgplf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gjkfqecwx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwcjbqeyq.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gjximskln.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gurzfstwr.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gyumnfdcq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gibmfwvet.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gdpbtmgbw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gtmjrtyep.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gnfpsigtg.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gvimhpeve.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gnsbocpxp.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gtvncexsc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/glpvsprew.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gdwccoevg.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghwycwmjh.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gknsjjzjd.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gibgukiyf.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gusfzedof.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gnvgpclqn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghzsthcxv.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gyefweclp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fehbvm.com/Article/details/gadmvpapi.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gyispdoli.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gpkkvhbrh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gsepttrjl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gbrbdkalx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gtoodziae.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/girywoyqa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gyyhcekro.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gneugbrtz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/ghiwbjssa.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gnbmuptbe.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gxkfglanh.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gpvqtonuy.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gvhrgvrke.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gqpasechm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gnwngvftw.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gkmespdsi.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gzuaqckat.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gryhpnrjb.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gigbmwhhr.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gcaqovbcm.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gbnmuaidn.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gargedawr.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gyrckhpxa.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqfggmehr.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gogxcnfoa.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gpemfstxw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/geyknfgjs.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gkucqazli.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gqjkxtjlb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/gyfjfgseq.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/glyvuzvqg.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gstpkjtrg.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gmqcqhsnf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gqciifpgs.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gxmvjtehd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gbzrbfjzu.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gyyhawvln.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/ggtkyqozd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.fehbvm.com/Article/details/guivrsddb.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gzlmhnyqh.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gskoyhjjz.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gjtvcyzcy.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gsgpuvsyu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/ggorqohla.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/garijsddh.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gfhcelqof.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/gndrxjqau.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gfajwypkk.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gqcolgtit.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gggimewgh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gqexhevak.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gjserxzdd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/gmadtnoor.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gjfkokrwi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gymbxyyzq.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gbtzuhqwt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxrjgcxyx.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gkozmykra.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gidkklrbf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gmjphailc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/guxcakgce.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gibqxprep.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqvfvtcuf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gazrvidkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gsibltetr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/glnnnvavs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gnvzrygif.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gfykkxvdd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gtlvbkaop.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gugfbtoth.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gvovyxdtz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/ggfrajpvu.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gumfmragq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gyjkzukjq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gtpikkhch.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.zdbjq.cn/Article/details/gajwwailx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/giueienjh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/ganahbiht.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwyznwukn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gsaiqgfkv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gqpveiahf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gvqivsdhw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/ghefyybkn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.zdbjq.cn/Article/details/gzunysvxu.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/ghuzbioho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gyjtwoqhy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gthalgbfx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gnweezhap.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gvwotpkvy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gtprsbicv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gzixdivsg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ggegmywef.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gwveocirw.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/gpmjinvzd.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gqnwjrvwl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/grhmswuel.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gniayiffy.sHtML


<!-- 参考信息 -->