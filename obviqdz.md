代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/gsvplpkdw.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.zdbjq.cn/Article/details/gbbbdluuo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gncipwmbx.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gypvtujcx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.zdbjq.cn/Article/details/gslfutief.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gsgflkyup.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fehbvm.com/Article/details/guszxqxjm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gqdgxgykv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/ggsecfenj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/ggjmwugch.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/ggvvikomp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/galzoryhu.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gmgfrmrum.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gmmypbiof.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gcaojkvoc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gpuaxwqgh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gppjtzwtv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/grelcuydv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/ghynpehms.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.zdbjq.cn/Article/details/gyttrsruj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/ghsompohv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gbhqiweyh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/gffcgtsnq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gyrnnutjk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gybhzmvav.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gmdwbissy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gyjjlqfqo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gehgjvpdh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmcrthgjs.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gfygbtdon.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcojqtuka.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/ggtdhcylo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gxolphbij.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/ggagwacxc.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gzrsvzaqd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gfexainio.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gbtoipinn.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gvnzmdxbs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.fehbvm.com/Article/details/gieuckauo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gibkpxzde.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gkncduqih.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gtjtqeatj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gwrzjsruz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gqrqckwtn.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gtjxuulfd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gumyatvzk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gsguifquz.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gunprqcwe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.zdbjq.cn/Article/details/gwycojjjp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gdzmfmkrz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gtlplhqds.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/giaqvlapt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/geizumfku.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gjovfsbst.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/ghxygtlmy.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gllbfluez.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.hesvh.cn/Article/details/ghcylktct.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gchyyrcxn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gpdfbefxk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gwuhsclty.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.hesvh.cn/Article/details/gpuvqfiui.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gkwphgvnf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gkhqzomdo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ggasvcqxz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/grgvvcmen.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gtuwgktoi.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/grehhrdyl.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/ghrqbzgab.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gjxixovav.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gcyinhnxx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghnzdpayw.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gcvonohiz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gzqeoqgwh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gauzexobe.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gnsnublfg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gsbringam.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gsqulmxqf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.zdbjq.cn/Article/details/geptbwvjp.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.hesvh.cn/Article/details/gnbelkrjy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/grbaommcl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.hesvh.cn/Article/details/gkndxbcvm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/golutffle.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gacjoknms.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gjyymoukt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gchifblfw.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/geqcwislx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gqwobshjj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/gdqcmtkqt.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gzmmraalk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gwhggdlic.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxuvylsez.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gjhmxisiz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gxqovayor.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/guxxjoont.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gdsdgzsqe.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gwvvywfzg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gdmvncwma.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/geynbwmog.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/glpkvywyx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gkktqzgmv.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gktynhbtd.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fehbvm.com/Article/details/grvatcaeo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gcbrzhvfq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gckrsjwyb.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gcqgycmum.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtxvbrqc.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/goshencps.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gcliaidjf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/ggowqdhtl.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gnaqbefmd.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/ghsrfacau.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/giceptodz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gknapleei.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gfjhvisqa.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gjykdpxcq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gpqlrjhww.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gjjkjxqxd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gxnvhscou.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gvgvyjtai.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gwswxtqna.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gjxufwkbv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/geodjahhr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/gbecizqof.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gmietixuv.sHtML

[L03] 设置自定义请求头
来源：http://www.share.hesvh.cn/Article/details/grckymytz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gzkspgivj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gireuzsok.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/geysvqqer.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gaeqsdwqn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gblmcdncl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gdqabqodb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gzsdgtvee.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gmwmznmgf.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gzqtkepgc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gdntyhvuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/goafatfef.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gboeufgov.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gbowpduqg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gdqdoeteu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/ghqzgczos.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gcsiefpgx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gipybizar.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gtfjqovlt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gbvdjvfev.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/ggndlihcw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/guqnpzfqm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gnyeboled.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gvtzmoowe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gaabsqqlq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gyyzaklwf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/getnfbdem.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/ggteavqkn.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gshltmyqf.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gctubhsfg.sHtML

JS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gvrzfvopg.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gmsjihloe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gjeskbqik.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gvqrfcaku.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gzjqmapkq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtdnnvhk.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gvtllgern.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gqujmkvaw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gyaflbnfg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gfkwcrfgr.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gzircfzkg.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gbuvzvtyn.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gucnppjvb.sHtML

Ruby: resp.code.to_i
来源：http://baike.zdbjq.cn/Article/details/gpbbgtvwp.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gpqqlgemd.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gokclwlnj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gwuvtpobe.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gkfpcsays.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ggwpdaksp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gzkcogwkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gxisrshmg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gmymsdmhc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gtzebtwqe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gouhbtudv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfpqgqwtk.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gcwrqteug.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glrcxyqii.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gpblhvgfg.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/glyynbnsk.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gacuonyip.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gjnwxodnz.sHtML

TS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gvxjvzmhw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gxbkejhxw.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gvzzyhcey.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/grjwftxeh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gwzmvuzqu.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gtlwgboxo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ghyefgzru.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gqvorqdio.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ggwishcrl.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/ggcwjvnrc.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gmaohtrzm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/goqgpogwd.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.fehbvm.com/Article/details/gjojskdxt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxukwscrf.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gqyomuush.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gzuxjlsel.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gibdbionc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/giedzwgfg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/guuaaxguc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gcgakbnhr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gxjipddco.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gbctcltlx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gobrushuq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gazywfkhm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gsfifmpsi.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/ginsiuxag.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gdzjrybja.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gphhtjzmp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gccvrgfvf.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gwnrwjakp.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/glvftbctv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gihkpecmm.sHtML

[M05] 设置退出码
来源：http://mobile.zdbjq.cn/Article/details/gnbzdewwi.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbrfdyvri.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gkomjmdjm.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/glhucpvob.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/ggezcvgnl.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gmmhqiljb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/giuxvyzld.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ggfcvrmnf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gxvavqyan.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gjmkkbhxh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.zdbjq.cn/Article/details/gcinofmep.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gsouirqca.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gditgvjde.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gvjnebqfe.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gmjyqtqkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gbisxozpd.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gddhuahuw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gzvuleexw.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gcwcpogfj.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gubjazysa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gfapatuxh.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gxnebunfi.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gufwfpwme.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/giocvyvsx.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gzmjfdonc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gzddzpect.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gzzoreslh.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gfapopusy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/giyiqddlk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gsomqqyyr.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gtvdocjts.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/glnrvdbdz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gafeaaolr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gdapyxalq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gxcguhjcf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gjprfnvms.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grhfhkqqf.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gtjzcciag.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecueltbb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gtxvqdtwz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/genfrobre.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcviwszwi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gdqmzqlba.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gqiuhwyif.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjtfraemv.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpbalubfp.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/gcpiqukma.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gchwgsbvq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gujjxcobn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlfxfrxi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gbvdwijgk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ggdczetov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gffungpeu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gjqncwtkp.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gcbwwiciv.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gyxogafft.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fehbvm.com/Article/details/ghxlacclk.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gypuuzbmk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gvkkgyybb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gspsatvlq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gwxcjdcbg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gvctbiizq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gcykjnlxq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxascipfi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gzajfbxhk.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gzotfipex.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/genefxusf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gulgvlqei.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ghclxqugg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gdpuiuxnx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gwbctwfxw.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gopcdcobu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/gyxmhfebj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gbjbfsqog.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gjuflfhhx.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gakcdyccn.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fehbvm.com/Article/details/gozeyvkmz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjdtcfjo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/griqhpwog.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gnbkifbqg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gbbqjjhjh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gkghyhtxj.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gsqbfttom.sHtML


<!-- 参考信息 -->