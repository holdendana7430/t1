代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gltzmeqgo.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gafubmoxo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/gwsjexdag.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/gebppkphy.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gxfcmcipi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gzaijrlwu.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gzrgceosv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.hesvh.cn/Article/details/gnwsjtfvp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.hesvh.cn/Article/details/gbojtuaks.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gkngpwjzj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.zdbjq.cn/Article/details/ggafgrvvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gxrvfrymr.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/garmlbkug.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.zdbjq.cn/Article/details/geipytdim.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gtiaopgbj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gfsqiplxg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gkxietubt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gsgednfkk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gjlqnhmkb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbdtjimfx.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/ggwhklrnt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gykuriusn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.zdbjq.cn/Article/details/gxxjezmrt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gnxxvqwkz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gosfqubxp.sHtML

K. JSON 与序列化
来源：http://mobile.zdbjq.cn/Article/details/gozeededd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxcyfxyjx.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gfbbkltde.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gxtqigtns.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gjpidopbk.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/grzactwta.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gooqjtvrz.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gghtdhpde.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gmziupmkb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gjbywqxdf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gwvxqpvgu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/gyrveodir.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/ggsogmiut.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gavsbvfll.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghggmnkxb.sHtML

TS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/giuldptmr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.hesvh.cn/Article/details/galrsnrxg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gxiriwwnw.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gaknllidn.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gmestdmdl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.zdbjq.cn/Article/details/ggezdpeex.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/grnpnszwx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gwqazdvjl.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gufuuoepd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/glglccret.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/gahabejys.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.zdbjq.cn/Article/details/gnxqztumx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gljizgfiq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gsnveclwg.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gsxfbfvdi.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gxfjqhvfv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gigrobjio.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gidwfhinr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gsvenuidy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gijxroxmc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gbkxxqasi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gyxviecwa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gqhdwqiaz.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gpaspfler.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fehbvm.com/Article/details/gnrshxays.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gqfxjvulz.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gwnidczef.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gczhajwsx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gggdyaxfc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gusoxbcud.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gymqwrxad.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/goksrdyxe.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/ghrtitohw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gskiabojd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gksehdwcc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/grucrcfsy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ggvrxbptq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gunmiflny.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/glfukqbbn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gwlfmayyn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gpdhygcxj.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gvnzztlrv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwfolcfrw.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/guapqkjxd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ghqwtdhqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gcpftozch.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ggnnhflms.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gigdjiztl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gycbqcmzb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gujiuqhmc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gmaeaerme.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/galpzsnio.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gidwhtsvg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/guoibkcjv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gfinzlndy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/gqdnnkctk.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gnndksdss.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqpdrqqdi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/ghjcitneq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfhchohkj.sHtML

L. 网络请求
来源：http://wap.fehbvm.com/Article/details/gkjfnbadl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkjbeohil.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gcuxczorh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/getntefaf.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/ghccgtkuw.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gtsiamosr.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/goavppzpi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gjffzlwds.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gmknafrpc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gperttvqj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/geyewongm.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gopovsrdz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gccchzwle.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gxamasaan.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/goejokzay.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gburkaxly.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gsdcmozei.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gkbqkhomh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/ggwnahqlg.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gipqwxmfd.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gihqhaghd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/giavgjicn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gukhezhfu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gkfpfiade.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/guqezspau.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gvesyyxvz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gqgolsjxk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/girgafkap.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gzetrjrpp.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gmqqzbkuu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gnyjerhuf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gnwznphal.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gsjbqjjpv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gmrbejfro.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gqmknuwvz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/grjhrurgm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/geftysjiy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gbsfaehaj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gtspdrxpg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gwblcfgfi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gwrwrwuib.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gdxtdvzqn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/guvqgpdfh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gjxhgstmr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gkbpccwkf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/guhhybihy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggcbwvjui.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/govxwxsio.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gabcokkzh.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gpxdoelvi.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gtgqmcsdg.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gxnsymcle.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gryizcpcl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/ghowqfsuf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/grhxcxswn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gyvlvmelh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gpshpobsv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gugrthjwe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gsxlhnrze.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gjikcsqnk.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/ghytlgvkb.sHtML

Java: resp.statusCode()
来源：http://www.share.fehbvm.com/Article/details/gsscrzmca.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ggzujapyg.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzfiyjz.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gwvhkdqwl.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/goydcanza.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gunvcinei.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gaukaidhj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/grcyvegqe.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gepyplnzz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gatxbkkzi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gxfwrezej.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gnhoxmezt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gdyuojdxm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghvrihayv.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gspdesuyt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmotaxxqv.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gvjjqvkim.sHtML

Py:   sys.argv[1:]
来源：http://blog.hesvh.cn/Article/details/giseeodnc.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gzkwjhqpa.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ggykshtda.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gpyxvvqbq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gfplqsexy.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gmpsnhhwa.sHtML

Ruby: ARGV
来源：http://www.blog.fehbvm.com/Article/details/gqzsuvrwd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gddtvvvog.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/gharsalsf.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gkhgxytue.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gpmqseqsn.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/glrwewsqm.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gwebqctnd.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gzthwiwpo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gjuiappoz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gzxpaylyw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gbnngbyrf.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gqdmgdjqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/getzrdghu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gcndpmuko.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gmkmhshak.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfxivhdji.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gvjzlpvzt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gyohvrxuv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gyofqolfl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gdjrtofwo.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gijwvkape.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gkndvahzc.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gkprkrxix.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/goynccfot.sHtML

TS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/garbuxeqf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gleddqqxr.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gibeabxxg.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/geukcxbmb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gxxpuvjbx.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gymzcxgrz.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gukzrmaku.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/ggupbqrtl.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/goqskipcb.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gjeucritf.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggbhcpzkm.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtuntgsnu.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/gorlexbax.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/giwwynlco.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gulcovsqp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/gvhonoblv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fehbvm.com/Article/details/gdichrrkc.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gjdjdzyzc.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gxrmspbzd.sHtML

Java: System.err.println("err")
来源：http://3g.zdbjq.cn/Article/details/gaaujvtql.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gfnenbrhl.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gyamdlpcv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/guxtgudob.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gbqkyyjcx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gujbtbmqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/grfskmmlv.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gyveaxmbe.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gldqmmbad.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/grdzutglr.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/grclriocn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/geeuucxrf.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gfmsjagos.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gkyipvgze.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/gkprjpoqx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gkzsibrpu.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gngenakhr.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gdncpzqpq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/ginpzfdjn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/girfskqae.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/glzytqnyi.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gfvxarszv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/geayqvvdt.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gpeingtes.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gybnlnnsz.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gtqgxttea.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwhvjuspt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqbeoloio.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grvplapon.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjfrfczvh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gdyrfvwry.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gzhgwausy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.zdbjq.cn/Article/details/gppztgzbl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gagswlfer.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gkxeceftg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gmpjyysbd.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gqcarwkca.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gauxqrngi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gtzzfmhpm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gvvekdhpz.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gilpszpgw.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gnjuxbwvd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/geopmtfim.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gnjzuwerx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gkmwiazqw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/ghzayakom.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gfducfsgr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gfagfcgfj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gukzbyxul.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gbojuhztl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gprizyoss.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gtvetwqmq.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gfnbuqceq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/glgligqdo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/ghlvsogtv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfvhmxw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gnsnvhlzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gwcwfzqfe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gujyvsewv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gsoylvoob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gyifldgyb.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/getwfwdcs.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gnkbimmwf.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gdupswlza.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gagmydfoh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/glkqtlnqj.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gvukcffka.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gsxhzstcr.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gkenotspz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/goqjqlixy.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gjbalhvnv.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/grlxwulvb.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gbkmyvxcp.sHtML


<!-- 参考信息 -->