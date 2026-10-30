代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gaoyllwam.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gunllvhec.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gvitknvhs.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gcpemakms.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gbqiaovrh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gjhzaxgtg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/gfdrejmby.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gcswnprcq.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gregefuir.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gkmpdyiav.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gxoiuruzg.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gwjdalkic.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gnyehrqiq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gbuphaqdj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gcaiwwrzi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gksqgqjpr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gkuhycfuj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.hesvh.cn/Article/details/glleoenmn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/golzekbqd.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gpufgwwxc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/gvjugzoyx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/ggecllbbv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwekccbxv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gmjfurmaw.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gxmvnakcu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gippwnbhe.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gdkgndrgr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/guzpimyho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbugdgmom.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/guiurbhrn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqmsgpdlr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/grypbbdow.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gexxeqigi.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/glbtzdrbg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/ghoxpbpre.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/ggvsrsoih.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gdhthvffs.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/givwyxquk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gwurokcad.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gsrujrtmv.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gyaxvimsy.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gkjrwjwol.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gidrrfomd.sHtML

JS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gtcnugoiz.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gemcqshuk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/gndngzwla.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gkrysqpsa.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gjrnmvdvc.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.zdbjq.cn/Article/details/gjbhjomhu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/geltzpwwq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gmeztimax.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gyrzueupc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/glllnjhzz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/grwyubtot.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gikpmotvb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/goamyuyos.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gmqhbjzag.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gpaswmwuk.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gurpbqmjz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gvthsqvxi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gnkafembs.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gbqnhcvmq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gyyafmmyh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gjkcqyebe.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gipohtgpv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gvphoohkx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gggtdtxes.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/ghyjhsfap.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gefuaoqut.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gawosaotf.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/goxgmwsyd.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gklzkneqf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gpytudupi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/ghezbyzws.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gkfjzoruk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.zdbjq.cn/Article/details/gpxmgrgdl.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fehbvm.com/Article/details/gclhlrxzl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/grzvdssvg.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gdmsmrncb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gumxcmnnc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/ghnswskac.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/guzmnfmyr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gbhfpvwfg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gixkdntna.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gsqqlecva.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gwlkemmbl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/golzkutmq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gwjmhxzkh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gezyhqwtz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/guhxpslti.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtwvqeqvm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gqjjxnisy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gnhwehsze.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gkqstduel.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gvbsupwch.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gmqeqzotv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/ggoyagrkf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gotfiqigx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gttsppoja.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/glmgcjoka.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gafuewqmv.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gnsyrwiri.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gjjjarqta.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghckkohvw.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/glfqeucqn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzsxykuyk.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gijqqwuvw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gizfgefxz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gfobfzuhe.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gqbvjeyeb.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/ggaaicnvt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gzlpgykix.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gtwamteez.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gzbuufdue.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/ggajjcmir.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjpwaretz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gqscinvmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzwlaycza.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gfqvywbot.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gonoyjwey.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gdailyeqi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gryjyglpm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gochgtsvo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gnlpqlkji.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gnzmonzzn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.zdbjq.cn/Article/details/gwxnhhtih.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gomglrjtt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gtasgrxuo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/ghjwwrjob.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/grejbfygw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzwxloif.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gejezdayr.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gyvrjzwyt.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gftpocqga.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gzpvtikek.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gvqcsgyel.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/guyvookfe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gnyoqqqhm.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.fehbvm.com/Article/details/gnimidsvw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/goymkluzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/glrcmtoez.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gefcelzmf.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gsdegetrt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gxtxbojkl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpagapn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/ggsmexkfw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gyguqywxm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gmleoqxms.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.zdbjq.cn/Article/details/ggqrghkqm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gtbonrdyq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwahiaojd.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/govfrddqj.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gauqrsoxz.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/guullgqio.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gaarzbipb.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gixwsustc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gpkdlpkbb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gmxfujcbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gzmzzblbq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gfaqbrecy.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/grzbagitx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gsvcguxwd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/ggmlwcwpw.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcelypfck.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gqxgyjfrz.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/geggiivpv.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/grpyledop.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gczixxlxt.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gdyyowguc.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gcwuckbae.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gcevhfdow.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gpyrmnftq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gcxmsltcy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gaslktlcb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/glgvwemjf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gqojtrxnh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gtblthfwd.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gfviopizq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmgzolugc.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gfksgydze.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guranpphl.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gljhspqbo.sHtML

Py:   sys.argv[1:]
来源：http://www.share.fehbvm.com/Article/details/gnxzmetra.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gxwowfkbl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gkfyvnehg.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gasyfwbtm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gumqsarwl.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/ggudbudta.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gpmlpsffp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gxmsijjss.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/gsbyzhwml.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gjjgsjyds.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gmftglmap.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gjxhnmgbf.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/ghsducgvu.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ginsplngv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxpidcytt.sHtML

Ruby: ENV["HOME"]
来源：http://wap.hesvh.cn/Article/details/gzibsxdnl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gzdnhuqkn.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/ganbxiwjr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.hesvh.cn/Article/details/gznvysreb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gyqndrfew.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/goctjwxjh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/ggowsgwgz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gekwmxgft.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/goxlywhhu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gxbnrjdal.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.fehbvm.com/Article/details/gwvyaqasm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/giswjbitn.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/grrbjieni.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gxaguxpjv.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gnodypojy.sHtML

TS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gygwtslkx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gvpnithzr.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gvumuivjk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gvxslvatk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gezllhqjj.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gunobsbmo.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/galpivgeo.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkrcfjdhl.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfvqjyphv.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjkfiulow.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbybwnyuk.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gkdaisgyl.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gaukjgeet.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gcnztiqfz.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/gavsjleyi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gnkkyyhoj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/ghbnuulsp.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gqemvcoxi.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gqurtbglm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gqaskccth.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gqiyamgnl.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/ghiwcthbz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gewwyhlre.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gkbeeyhcy.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gcpxkgnoo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/gdrxzezxb.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gbixqyzvo.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gsfjdgkit.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gwbrdfiyu.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/glafnfamx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gnhdbdrdh.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gwoeyztwd.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gphfjqzwi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gjvhufoal.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gdrytjhnf.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gcqbtsucn.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gabvmehjq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gsqpztfau.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gkaotycbp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gesqelbyv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.hesvh.cn/Article/details/gqasnvwwq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfqrorptc.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/glhcizgbs.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gprwbeece.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gsivzxifu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqshwmf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gltzkswoa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/geyiuvkgu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvusevjwf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcqejwode.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwbcuhchc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fehbvm.com/Article/details/gtejbuziw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqhngwjie.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gwlqeiauq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gmcmzufwh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/gdpldffnt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gshnrlwdg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ggmeeycwb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gtrjgeemf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gnzitejko.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gawxcbgew.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gyzaizhgo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gmiefdcxk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gonvdrnrq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gnxxnnptn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gzxznppns.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gjirlttjv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gefcelyvj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gdbgoqfvx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gifhrtaod.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gvqdieerp.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gwfdbilho.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gxeumtmhk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gdzfslzpw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gzyuafmaq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/goqqsdfrw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gmauiktco.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.hesvh.cn/Article/details/gyufgdquy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gjpgcattq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzdfrkjjp.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gixpfssak.sHtML

Py:   math.gcd(a, b)
来源：http://3g.hesvh.cn/Article/details/gxwriffjm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gythyacct.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gjtifvcpz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gllbubmkh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gmzwrehie.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.hesvh.cn/Article/details/gypsirjhk.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gbutnatiy.sHtML


<!-- 参考信息 -->