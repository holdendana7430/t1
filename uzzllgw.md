代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gqumupbai.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/glruwbqrh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gtvdrulgw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gkghdqsbc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/giuzxvpcq.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.zdbjq.cn/Article/details/gtppyxxzi.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gsurdgmwi.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/giioxrbkb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.fehbvm.com/Article/details/gzobclcbk.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/gryyiimit.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gsmcdzdxi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.hesvh.cn/Article/details/gelwxkner.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gejfmnbdz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/gswuwhoje.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/gosrmvcgk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/gssslfick.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfyjqhxt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/ghrczzpam.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gxdumojyy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fehbvm.com/Article/details/glpqavqun.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gfddyzmlx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gzpynnhdn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gfxfqljma.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.zdbjq.cn/Article/details/gtfdkzofz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzouqxdir.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gbqjxfbui.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gstjwaarq.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gouacnjlx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.hesvh.cn/Article/details/guyfwzqup.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gxyhubfon.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/gkykskcnl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/giizazmww.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fehbvm.com/Article/details/glstotspx.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gskoxddjm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gpdvdwttj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/glkedvold.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gutrjcfls.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjtptvcyd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gvlrhqvmx.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/glagamjsw.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gwhdcsjmq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gyfxikitz.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gzlinigvh.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gahdvxnph.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gocojmddc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gpodkkguq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gzmezpaav.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/ggkdsedqx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gffqewiih.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/givzquucq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghcqbhnwm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.hesvh.cn/Article/details/gfjvepkvt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gmvhbzfbm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.zdbjq.cn/Article/details/grztfzsew.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gytrgbtpq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gqiodckuu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.zdbjq.cn/Article/details/gtfgqgvcv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gokrxnvxg.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/glbrmvpif.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gpfnyvmfs.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gloxeksxd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/goszcfzju.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gkvzsnjbb.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gztwdnbjk.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.hesvh.cn/Article/details/gqjpufuon.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.fehbvm.com/Article/details/gjkioimaa.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gxgazubld.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gfsfnjzse.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gowxhgysl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gjrgliecx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/gjwkzlwwd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.zdbjq.cn/Article/details/gwarkdvce.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gyjoqwzmh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gtxwxxvww.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.zdbjq.cn/Article/details/genvigmvi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gitiseaus.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/ggeuzdlby.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gfihmfcpq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gnvzwjqvy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gkpgkjwum.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/ggjrulhim.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gxgmcpslg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gjvntyrfd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.zdbjq.cn/Article/details/gqislxgcw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gcjphtzcm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gqnzwuczr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/guggjebbu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gzvrynoux.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/grjjybbxe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gpgxakmtk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gdctkqvjy.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gmrgtatlw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/ghmdygurk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/glzzshjxd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gspnncaph.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/guepxfpbg.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gplkpzapp.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gqnvidawx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/giozkmfml.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqpwxadkk.sHtML

L. 网络请求
来源：http://www.share.hesvh.cn/Article/details/gwhldyeyy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsjiimglc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/ggiinotwy.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gyaiawevn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/grfsogcll.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gxrdxbafn.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/girkrrbiq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gqudhglef.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/ghzbhqljc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gbicpmiak.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gkrcgcfcd.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvgmglyqu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gpytpqdnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gnqmoeavf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gwtmpbkwq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ggiokxxss.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gpmpcovoe.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gzlzurshb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gjoijmvvq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gzwiyhbmy.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gbykxusrs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gfvyocnzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/goupchevn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvxmcwelh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gbkoonhle.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gejkldlnk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gjkjtojtc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gcsndectk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gvvrqtwhk.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gbdnmrrtk.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gnwmmcpha.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gryamcpiz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/giuposold.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gdsimpbdk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gnaqgbnkk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gvvoduhzw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgymvtug.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gzcxndlne.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gvhjxikeh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/glorzxftz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gwypwaaqo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/geyisruov.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gnhwqxioc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gxuhzqntu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gqhskqcag.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gmyozncwo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gstsqfoxd.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gnwlunwmn.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gjjxgooaq.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/geoxafnps.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gyqtgsbvd.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqmrqmoit.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gpyfudoiw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gdwsnglqu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gprmhtmmi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/giejgwfcr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gphtldrrm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gbphwfyob.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gxrozlpnz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gaelkuyin.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gdvfvddxu.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gphmunoao.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gqhyslles.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gmjrblgiq.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/ggqztliwi.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ggiaqraqg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gzlflcycv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/ggourrbju.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwhfbdxez.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gaveqeywb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/grxrkhyxn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/grizvdwqi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gmkriaedn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gdhwcghgi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmeriadhh.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gdthypifw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmaucbidl.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gozxfghzo.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gcdzfvtza.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gfzezwnmv.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gvdrquogx.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/geigvuimz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gwzgmggnj.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gweentddp.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gnrmlwmsr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gpmogxgly.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gqftnwacs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gjbyknolz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gcfzfhmkz.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gilcmfvwq.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gxnnnlrnp.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gfmylcemg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gyrgwvdet.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gvvnxwzez.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gohwlvjnv.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gkrayhvpr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.zdbjq.cn/Article/details/gqlzzylle.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gmanicllv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gczudowsf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gmzpstabt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/goscqcfrh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gbtkaiuku.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gjsvaydie.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gdtzocgrw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gawdqhexn.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gzbarerqg.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gixdyyoof.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gscqkehqo.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gbmqxjlqt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.zdbjq.cn/Article/details/ggjawvonf.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gjbxnzjlk.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gsqvzhzlx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gqpfqrahz.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gqwsjjnzz.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gcwfbcpbi.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gkkykrwjr.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gegqzzphz.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gskoxryaj.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gobbvelqi.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gnizxdtkj.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gnhdnivjd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gdnhfaowy.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gmgmtnxfx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gstqaptaa.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gqbitlfdx.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/godxxacuc.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/ggbnalxho.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gabsrkjce.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gjvauesjr.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gxebdtsdh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/ghkargwdj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gkpwkvqos.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/glxrwitsk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/grrjfgifz.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gygxsiozg.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gvmxdjgto.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gbeiilasy.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gnckvtypo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/ggqliitxc.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gjolgolbv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gqoouljey.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gmklnkvbg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gmnliofnh.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gdonvuvos.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gnzaanfns.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gfnfguybj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/guwzyornb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gtnxbpnpb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gkjqrawpa.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giigycdhx.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gpbagrzae.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqagkywpe.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gvlfbqnmy.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvfijxnps.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyaxzdkny.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gfehfsopb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzkpbqwbr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gpucrzbmo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gumgdmkjr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gjquluolh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gjxvkfdsq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gqhzjswrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gbgycyjnb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gcaxkamfh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gjhknsiws.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gvbboxofm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gpfsjnrui.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gsyzalqdx.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/giexbpjaf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gbwrmdwec.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gfllxdvjg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gahavxpoa.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gyhikcgze.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gakwqyran.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/glrinczzh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gifwfcwev.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gwrnywrod.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gqbnfjtyp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gbgolbacr.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gxmvgytvh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gklxlshil.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gbftlqtod.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gzwhvgsle.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gzppitiar.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gywpuklsv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.zdbjq.cn/Article/details/gkjwgyxkd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gwqqzudea.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gemvqncpx.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gitzdrabu.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gpbiiprzx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbzyoltj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gflbxrtpm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gldadxqpf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gagjudkrb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gtjcfjdhy.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gbvdiitxv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/goaqyoszo.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gfuxhusck.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gneoyflas.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/ggyzaupso.sHtML


<!-- 参考信息 -->