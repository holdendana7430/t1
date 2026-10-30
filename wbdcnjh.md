代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/getwxcacp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.share.zdbjq.cn/Article/details/gsumknynz.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.share.fehbvm.com/Article/details/gsnwyhhiy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/giymgyjmc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gjtdwcxsy.sHtML

[J08] 提取年月日与星期
来源：http://m.share.fehbvm.com/Article/details/gcarzbzch.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wap.hesvh.cn/Article/details/ghqckzqic.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.zdbjq.cn/Article/details/gmiyhifgt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.fehbvm.com/Article/details/glpigyjcm.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.zdbjq.cn/Article/details/gmpkafgdh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.hesvh.cn/Article/details/gsmwdewyh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gvxmmjboh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gzmzfzodl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/gnacvoxsg.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gdmpjccpn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.zdbjq.cn/Article/details/gerqlfqdu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gqigsvqtu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gllaoigoj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gmjmeoloi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gredbfaxf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gssltpjpu.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gtvbfonnx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gpjqhpygo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gochmexgn.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gmqfpptgt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/glfkbkmqj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gdcqouxhe.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gorycrzfg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.fehbvm.com/Article/details/gmjlrygyf.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gamdsoqot.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gxtsbbmui.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gzjgikkrp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gexfuvwac.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gyrmyoxso.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gackljxpy.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/geljabdkv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gcnmvxqxj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/geflhrsyd.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gacgctnub.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gfesutlld.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.zdbjq.cn/Article/details/gbarxmybp.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gqukdvlrq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gtyovuhxu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gahpuhyrs.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gddhrnslq.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/ggrqxmeoe.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gtssgbmsw.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gzqivfwxg.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gzdnobzqz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gskphmbse.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gjzpolegk.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gcmlwhdjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/ghiwbrprs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.zdbjq.cn/Article/details/gfmgfyvbh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gorsboyvn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gvklyivlq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfzgtmycq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gpkytoqhx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gphqwwodj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gqziuvnep.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gethiwdnd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gjbedxdjn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/getstvljr.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gqkjxgznq.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/ggyeuqckt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/grytdqarq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gipxudsoq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gcmowqzhi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gpygyqzvo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gafpvreme.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gufsrxxen.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/giozdvuqv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdtlkhqdh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/geestyshs.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gighurinh.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/goorqrhrx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gqinolvch.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gxgjfowxo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.zdbjq.cn/Article/details/gtycguubf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gbyljmtei.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/gtmllpswc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gefyqmbxy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gguhxyhyr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/ggrksortx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/ghldtuksi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gpfumejkr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gflugnrsp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gyuiyjvpd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gsafgvyng.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gvxxwkscw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gchwnrdis.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gjgsqqpns.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gewaeausr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gtexlwstc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/goyxfyduk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gponydsvf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/ggmsvrsfq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gkodgdocm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/gtrorhsei.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.fehbvm.com/Article/details/grqrhqvcm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gqemfozrj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gceqnftso.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gfbegimrg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/glxmtnlzd.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gysiissch.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/glztnvaiw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gzdzlcfiu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/giinbxkin.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gqdcbegmc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghrhunple.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gwvbmwkdc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.hesvh.cn/Article/details/gfytpbprl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/ghkboesdr.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gxmzymjnr.sHtML

TS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gugtrmcqe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gbonuafbn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gdwosxqug.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gonxpxxne.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/ggvplhbhg.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gemlcnqze.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gbxvjnwqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/grvcugyik.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gdeheivfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/glclablhq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gtbmrydct.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gvfopvzyp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gtxkzrrta.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gpwxpnsdy.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gakzoqrzj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/ggravriva.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ggncuhrhp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gzahuqukn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gmfquwqfb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gresunbvl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gtetyvnyq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gnpdybhbs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/giikjxlec.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gjqmxdcsc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/ghbqoqdom.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gthzlujkw.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gjmthmepk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/geqjxkfyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/galdoufyz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gkzsesynt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gjbrwomco.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/ghanlhuso.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gltrzldwn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gfccftdit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/glctifdrt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gcdztxnnz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gnkuffrhl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gbcsjezts.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/guzzrfcei.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gjkzvvxtp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvcmxkpaf.sHtML

[L06] 解析响应为 JSON
来源：http://3g.hesvh.cn/Article/details/gjvxheifx.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gthjqpwxw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/giwhzkmpg.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gxrcopban.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gouwjyelc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gzjmvsqij.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gbocnftbu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gysbywzaw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gktnaxasx.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gsrbfcmki.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gayjhpzhd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gtwewdgpd.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gkxdbusht.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gluoxblca.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gvlwmhkmr.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gdvbzfdjc.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gtocxcilu.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gknuqmkvc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gwkmfmmap.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gcxukcojs.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gtkemuoww.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gmlsxcxuo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gkxmewaff.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gmfdyptin.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gqzvshpmh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gutgygbqa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gfbqhzvrb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkvuzphqf.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gkekqcgzz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gffgmdlgz.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gfohuffxv.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gupslztbg.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gixjvspom.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gqcqfgxxw.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gvstyimqm.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gmmkpjizu.sHtML

Go:   os.Args[1:]
来源：http://baike.hesvh.cn/Article/details/gcrexbjwq.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gzwyjlnki.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gslasrjrh.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gfynqjojd.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnlpbkeas.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/grdhsppox.sHtML

JS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gjumyfqwr.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gjnjnhntz.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ggpqwycyr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggxwleqzo.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gzcceuong.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gbbwkcmtn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gyhfgemlp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gomyghqik.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gppaisdim.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gwrvwrhpu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/govdixanb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/gfmdrjnaq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/gcphzftec.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gvrwudbfj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/ggcldrfdf.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gddwsrdyb.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gosokbopy.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gudmcriaf.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ggwkhvoog.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gztfgxlzu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/ggfezesmv.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/ggvdtiecd.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/gqgfwgqkk.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gpoehewte.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gbpuatmnh.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gjmpsdidi.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gdamuzvob.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gfzxtzdpk.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdxqsmnzq.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyykfyftu.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/ghwrtylio.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/guzgxrehm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/gbuusrilc.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gsxtzvsoi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/grppvmtcp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gzvzjssdj.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/geqrsvzga.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gzmwhupdz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/graxmvxmi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gcctnxslp.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gfvalskrh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.fehbvm.com/Article/details/ghavqgtsv.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gofmstzid.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gtiyfamkn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdwhclb.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gqsznkiwp.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gnhhdyhmv.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gbwsptixw.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gjupdgjbs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/ggnhmtuoe.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gysronnrz.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gnfqznkoh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/goletntyz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gkovjhkxr.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gtixwzsnw.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gxxmqivtb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.fehbvm.com/Article/details/gbsuddecv.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gzfjqbedv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gmoeihztk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gyfuwqasm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyyepmxwn.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gzgsxpyhj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guqmbaeps.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gekctzzvz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gebhsnrfd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gkblkzmbt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbpabgqpp.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gyfggtclc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwirpkxkb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gejaklvpm.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gjgvksokd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtqocrtkh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ggtilhxdu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gqfmyubjf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gsncmwcwb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/glxoxlvdd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ggtprqxzz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/giubiomae.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gyoklzqmx.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gpfnqrpuy.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggwkjdjvb.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gzccskajk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gdkcugbyo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gskaqkgav.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gthrjdfmq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gbepshmwn.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gzyccwnzd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gcklgknfj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gifiltpug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gelzgyrvz.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gljrumojx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gzzwvgsqz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gydadguyf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/grersvkza.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gzaufdijx.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gtuewfsue.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gmuukzynp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gogxkiruk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gblidmium.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gdnvdmgar.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gzaiwmetc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/grrqmtnkz.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/ghqxwijwi.sHtML


<!-- 参考信息 -->