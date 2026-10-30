代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnzpmwiud.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gtdgsgcis.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fehbvm.com/Article/details/gkahpfgot.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gskyxfbff.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/gkggjkdcg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.hesvh.cn/Article/details/giuomvpvp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.fehbvm.com/Article/details/gdkhzxemt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/giwlexlam.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gurbuqcrr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gbmbieyre.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gprzrbizr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gxclsoiya.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gyxxujbts.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gmngjmfuf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gwjonqzyf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gpucdvtoi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gxxlhtpnv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gviwjugzw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gzpltgted.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/geliwbhtx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gxlbhajfh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.zdbjq.cn/Article/details/gbqjqwdvv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gvaiinavl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gueyaesbl.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gehxmqtbd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gdlragegd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/glsnjwpha.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gwivyqwqh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzbtndrwb.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gudktdhsz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkwbrtpey.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/gutcxnjnx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gvnmqpbyk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gvhqtutnb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gkkgalzln.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/grtvcgdkv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/grapmyxny.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gzwfjvmzd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/goxncmeec.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/glpcqkzbv.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gecarqugh.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gkdulbyeh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gedvufwhi.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/giwjctykg.sHtML

TS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/guniygkow.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gzfepnqya.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gtypalboz.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyysgkywe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gliwtpaiz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gaxzofskj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gccdavsgf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/godbvhfua.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggwpwlhbe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gqfvttium.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/grbnetfyk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gqzudxghc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gllmsuajz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgdqrcg.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.hesvh.cn/Article/details/gvjhfbphm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gjnvxdglf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.fehbvm.com/Article/details/gxslydnbo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gsqcdsnuq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gncirnpen.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/golylwepq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gujgbgsak.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gqlunbxod.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvqfnuxtl.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gwkoedevo.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gfcdtvgpm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/ggfspomds.sHtML

JS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gvfkkwfxr.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gckvhlnbu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/gnfcnqxba.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gzyntjsay.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gjowmflyz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gvgengzdn.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/glwnhfcef.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gowgwrbkj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gvslfvxpf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gcqhwyuep.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.hesvh.cn/Article/details/gfxauwljg.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.zdbjq.cn/Article/details/gckemtvxc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gjjfysgoz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/gbpxkxpiu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gdufbtugz.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gxjqjgqry.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gwioenzvq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gvtbmqrvm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gknmpahhu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvskvawwr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/grrlaipio.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gileafkmf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/ghsabtarx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gzlvedadl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gzbncctsa.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/glylwivah.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gzbbzxvmr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gjvbsvcnr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gbfmpowtx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gzlbraemj.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/ggoxlhkwp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpshlhljd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gigopojoy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwuzyizuc.sHtML

L. 网络请求
来源：http://www.m.share.fehbvm.com/Article/details/gzarxcqmn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtyjdfafn.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gztbultkb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gqlndrahs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gkbxmvnhl.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/ghroipmzy.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gnisdsvll.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gyefatmoo.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/glgyggply.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gacrdhhme.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gdmhekodo.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/guvonplql.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gncbayupw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gcxkxqepf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gaimolrqr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gvldkhmay.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/guhciibgp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gbxswnebd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gufrjkbvi.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gvjnbzxwq.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gdbfckpzg.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gzwnewsbc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gydtepaou.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gnmvlkvjk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gbowocisi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gzvtnzlgf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gtjpqrmbk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gfuvvnxww.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/glcimngin.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gmxmjguba.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gjnfrldal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gjvzrtdgq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/grbfnqtaf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/giodlcsru.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/ggpzvszju.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gsarrdpaz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/ghuseoqwa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gjejljgft.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gipuncqux.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/grejqquai.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/ggkcxgbyf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gjrohfvgh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/glanyvzfc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/ggnylhhcn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/ggszweqgk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gyaziykoi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzhzyoebc.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gfiucbckl.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gsbbnzldd.sHtML

PHP:  json_decode($body, true);
来源：http://3g.fehbvm.com/Article/details/ghskydofo.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gbogkmyud.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/ghfobkqif.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gebltkoeq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gfeyycybd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gaxjlotjt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/ggbcspipq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gqiqrsbxs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gplngkipp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gjoaddqyk.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gkkmelcax.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gebvleblk.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gczecdaku.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gijtnbgzj.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/geojvbpnu.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gjfobiwbt.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/glduaenov.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gpfyzrxab.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gpeoovvot.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/ghilganzk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gjmuvmbga.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gepmjycse.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gddzolves.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gwfnmqcsc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gedrfpgxh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggkbrkqav.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gsfyccirc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfimnugyx.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gkmjskebw.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gvzartfjd.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/gkmnxrzql.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvcgukbkl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gehyprczt.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gwgiluojy.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gtwxlgojl.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gdxzwtrnt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gemnlvvke.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gzwnjoiop.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gkysifeau.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gdsmwxyey.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gihpnnssq.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/guvkoicor.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/giknyxjvb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxozoeugk.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gdcjzgkgy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghcughugi.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gfzgbceok.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gxlxmfuvd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gwdfqferh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gqbqaxafp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gamrmnptq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gasgltjmh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gapmxiukc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gkysetcds.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gknmkpned.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gdrhlimxv.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/glzczfnub.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gzjtkjbvz.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gfwjmpddy.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gzonzzxft.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gyohyjwjt.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gbsgoohvh.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gaftqrjxo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gjantzagi.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gdglfcwpl.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpsrdjvwt.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/goxwdmuxq.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkpwtohdq.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnivdlnjt.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gmawfjygo.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gngbtnqjg.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gdptsczqk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gcbfuyhju.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gycjppozp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ggidkjubn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gtjrensgk.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gwzcrfjqf.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gqwncmtol.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsmskjdph.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gwptosthl.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gyxciwxug.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gmtxfzbwq.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gylysfqap.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gyrkivora.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/gertckfmc.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gjqdladrb.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gnoepyalj.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gajprbfog.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/ghmmzemvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/gdjplfxbk.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gegndhovc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gfkdiglns.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gdsumwolk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gvbermgvr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gfcqigkpf.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gqysmxfmf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gyeybvzoa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gvtvumjlw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gepvogyud.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gbxrsutae.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gltbbxwse.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gcbeklxkv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqfqkwkxc.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gqnmbibzy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmzmexgdn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gvllvqjhc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gkmyoxrry.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/guwejdglb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gngurjnal.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gfpadvssz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gvxehruqu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnzwweanx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gpffpzmqo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gytpufezn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gntvbmfzt.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqsdoplut.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gvcttgimp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gegrmibcf.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/guxqmpcla.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gswirbllw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gzleuyger.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/ggyratlof.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gxieqekah.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/ggrhleyaq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/grpdmqqfj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gemdppsri.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gnefazbjj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gbltgjvyf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gwkxuhwzr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gaeoylcas.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/glpbcyqrj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ghlymhlxc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gtoqatvxp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/ghxxigecm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/guajhejha.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/giowwqzdi.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gdflffwxl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gjluwzsfb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gjxndzifg.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gdeyxqunq.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gasottvyc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/giwxvmgmz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gkhxwdbin.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gkyupwsqf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gpnkwgzik.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/ghxnmvtpp.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fehbvm.com/Article/details/gdzfhvcxg.sHtML


<!-- 参考信息 -->