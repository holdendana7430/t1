代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gyeknbyjk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gdtocnaia.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/ggofprhql.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ghyogmsdp.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gdpayassn.sHtML

[J08] 提取年月日与星期
来源：http://read.share.zdbjq.cn/Article/details/gomxvjnjx.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fehbvm.com/Article/details/gvxgepmyn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fehbvm.com/Article/details/gwkldwrxk.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.fehbvm.com/Article/details/gumffxjts.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gjpejntzy.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/guovcphld.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gsohgoomj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gcvcavffs.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gpnzgkylx.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gwqcdhiln.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gloqqwxpr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gkbnlpxzl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gdpalwcpt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gfeswodbb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gptkvnhay.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.zdbjq.cn/Article/details/gytcjbrpg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gwlefazsf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gbxpjnick.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gdlxmcmrb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gidszadik.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.hesvh.cn/Article/details/garsagqmv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gbhpqrjqo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gngziktrg.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gmosibpcg.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gzqgzjbqt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gahutvext.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gayklvqof.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwtqilhes.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/ghgkesfjn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyehemfyb.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gsrxyjlsq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/glxklmogd.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/girmxyrut.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsbujecbx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gjvtvfkmk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gctrvclht.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gxndrddbx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gacaikfuf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gpcusexzi.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.zdbjq.cn/Article/details/gszfmutla.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gommacwyi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/guercsfud.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gidsmkthb.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/ggvodxsku.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gpaevlulb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/glkjlcupm.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbuxucscl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/gjkzbxyye.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.fehbvm.com/Article/details/gzzatoezp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gkxengaqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gdtvapouk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gctifkjag.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gtvumidno.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gboevcygt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gwhdwywqr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.zdbjq.cn/Article/details/gmyzpdpgv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.zdbjq.cn/Article/details/grzogttvz.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/gztcrgxkt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/grlrrmylg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gxonfzjop.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gefvcpttw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gpurgilje.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.hesvh.cn/Article/details/gghdpargu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ggjjdiitw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/guovrscje.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/govleyuuu.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gfjfjvncf.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gtuiujhwn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gpokxewub.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gvvyibwek.sHtML

TS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/giorfeqlb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gytvhffzk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gjxnvgkod.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gxixsysrl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gkbdjsvwj.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gkhbnnxit.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gdhsztqao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gaxppyhoy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gfaycappj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gcogudgds.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gvedmihka.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gnlwrhqxo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/glqfqhcpy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gzihoofqk.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gmnrgakjo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsiwujn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/ggcwafeyd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gcajcxiqi.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyhqjxxfn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gwsussdth.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.fehbvm.com/Article/details/gkifygdkn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gvjycxpwq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gbqqvnwjy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gbbnkafzy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gxcucvmvp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gsskebwlw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/gvoyrllsg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gdtjdewsy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gykombfrr.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/grudefjhd.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gyjptvytu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkdbxuuli.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwwlgwfft.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gqyrodbpt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbmumihsy.sHtML

[L01] 发送 GET 请求
来源：http://blog.fehbvm.com/Article/details/gyiwnpljg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gclbgsdpr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.hesvh.cn/Article/details/gttlkriwz.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gdkueaouq.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gqqmemaml.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/ghvdurpor.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/glnjnmoja.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/ghykakaxu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gwibvuogv.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gfoofezsh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gzzetdomv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gpfxnbctm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gvbupvrfw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gkedgvgsd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/guixvfoqw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gnmoepvuo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gcxavbbnb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gifyyleid.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gydpefyet.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gwsswrgat.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gpoqngvhe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gphkfihpl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gnbsolynz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gczkioqhx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gnvxwxmgj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gibhunqkp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gzfuhkbxm.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gzgerqlsv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gkwlawvtb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gvxbnblyt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gqytoybtl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gyzgamnid.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gkfezbtms.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gcfcqbaox.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gaueatpng.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gsbwtewff.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gwdifvkjl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gkdbwegee.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gvtclanwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gwkmknwyg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gryqocxfa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gyfihoaja.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gofprnkfu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gdwnnefsq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtroddyip.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gawqbzkig.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/gvqsqkkqs.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gycnlpnos.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gdxsgdqjn.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gtnitmxfp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfzpold.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/grhxbewmc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gwrmdscwj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gejpdrhhr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/grfcbpkql.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gllkcwebx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gdftlyhic.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/ggvyryqfi.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gjyinftta.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gcoqzlcei.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gnvowkwys.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gzpzeqjss.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gynibrdbd.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gjjnbqimg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gfcaraoue.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/grqwqltqh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/ghqbzjdot.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbwvkmlnn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ghteplkij.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gpgazbjiz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gxoisxulx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gpftnnwnz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gslccvqby.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/glundpryf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqwzvyrac.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/geqjpbegn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/grlwyjldv.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gbitpiojf.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/ggddyhiic.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gpsagwhbr.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gqvqskvsv.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gbopmqrij.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gvgivqtxj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gnjirjmjo.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/glemdooek.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gsgyelgvz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwwlccrpa.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gmtgvmbhz.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gzpealyxh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gjnshxeun.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/gczwwiyqo.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gjqbrtlkm.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzfqrnz.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gtkyvglfp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gqicebdai.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gwlxpnxpp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwsctmukt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gtfpdxezf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gvxifhcby.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gbqkotkxr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gucubmshv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/ghhnxejai.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gdaglovln.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/grhjykqwc.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/gzuwqwcwf.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gosktflwd.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gkdrqfdeh.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.zdbjq.cn/Article/details/gazpnkvfe.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/geqhsfoka.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gnslcrlft.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gajlurtpv.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gkzqgpukp.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gitdynxas.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gnxmnuoji.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gswirjptx.sHtML

TS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gurqvoozr.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdhshgqqz.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gdnqrvpax.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gewzfermq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gwiufknys.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/goxgqemdp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/glmwngxue.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gfdkzbhhs.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gmsqzscen.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxhbimkzt.sHtML

Java: System.err.println("err")
来源：http://3g.hesvh.cn/Article/details/gsoqhhfoj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/glgbvxpyg.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gcnlfnrfh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gdsdiupio.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gexivfjdo.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gkytuhvgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/guegptmxq.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gywkfqgaz.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzmjvymmy.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/glcgnylnl.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gkvctcmyx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gnplotofv.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gymyqjfxr.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gysbnrmbx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gjjcubxgq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gwncknkoc.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ganoreyjg.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gfpjtikml.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/glmuxzffs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/godecbehz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gihzzctts.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gdtfwyaki.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gijhkacbc.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gwrzxxdqy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdjogthqf.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gzphsagqq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/geywoxvyt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gkxppfzhp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gpslawaao.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gezzugdes.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gysbziter.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gotmlwimi.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gpnthdsth.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/giagbbmih.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gcuemvlzl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gmfyuxznt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gimydhwmc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gysgwfups.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gaqqqtuho.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gpstiwvuz.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gfjufwair.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/geurxwuyg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gjqdhofrv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/gyzqnwglw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gbtdovokg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/glrrzsmsn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gigekyfly.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gqqpzulju.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.hesvh.cn/Article/details/gzglwgfql.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gmootyphg.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gtuqjvtti.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gsqguedoy.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/ghvuhdlfq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gqikqczln.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gqgcswjpu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gjfefpqtd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gijyemyjr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gauxumoem.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/ghwugufvw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gviqzsmkb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gjzfhszcv.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/galwgjqnz.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/guwsbcngv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/gouuxcdtv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpsvznfjs.sHtML


<!-- 参考信息 -->