代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gwkreegha.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/guxvfkary.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/ggkemnwvl.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.hesvh.cn/Article/details/govzyturl.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gxzwtogan.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.zdbjq.cn/Article/details/grtaviexs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/gorncgwpr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/gnmudrdmk.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gubawwelw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.hesvh.cn/Article/details/gpiostrdy.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/gmvutkzjk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/ggscymgnj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gwxscvyox.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gbthuajib.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/glwgpiuep.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fehbvm.com/Article/details/gztfilejx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gkaasfkbk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.hesvh.cn/Article/details/gwzxlwuvs.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fehbvm.com/Article/details/gvibtvmwl.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.zdbjq.cn/Article/details/gcimwlyuu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/ggfvtmacq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.zdbjq.cn/Article/details/gojbgpqrj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/ggaltaxms.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gmyilclle.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gdmgiylyz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gdcgzvhpp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gwrtjohps.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjdhluzol.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqxlvcjpl.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gmysedvtk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gujwudwiz.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gntcnxtvi.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gmpbkumlp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gzfbqqkav.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gbdnntwri.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/glzmoswig.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/gffurmrlx.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gcllpejhs.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gahfhnocq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gmlsgnvrl.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gjjgtpzve.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/gxyupgbck.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gvvikkmyi.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gvkowddqa.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gozyqlwas.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gmdyabtoe.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gwndqmcqa.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ggwhgwhhe.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.hesvh.cn/Article/details/gngkrtalv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.fehbvm.com/Article/details/gzdbjenpr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gvsexdmxy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gebmxgtyx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/glpdqrvau.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gklqezndv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/goxmviiul.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gaqucveaq.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gukxuamii.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/guqeizqdu.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.fehbvm.com/Article/details/gnqxdnham.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/grnlekpmb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/gkzdamdvj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gbxsgpwsu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gkxrtailn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/ghsugpgkl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/ghpbsoyhb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gmuccudpt.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/goegaowzt.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gdmkcpzdx.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/grpecfacu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gdcjziztc.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/gerwlvsky.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gntqvvocm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gxopleyal.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gokiqflzx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/glxdrybpa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gdishckhu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gjardunff.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gxsmbiekn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gberuowwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gpvvejmyl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/guarowpwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gcwmpslxu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gxvcpmrpx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjanssoww.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gggwrlpgd.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gadrworys.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/glcsdtlij.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gxldrgage.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gixklfoow.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjgtoszmj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gqxgzluhf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gmosedygi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gmemgggbu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gjeqjpqbh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gnfbtknrh.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gpkiazsdq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gwpllhlil.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gpzexuozl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gyuetewpe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gcfuyifbv.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gwbkyohct.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gmwokdufl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gfchekpqy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcybvpeeg.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gyleptcka.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gicqvafye.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gijctgvih.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gvhlrpfni.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gmzqwkpwa.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gtrjruwim.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gacxtmitj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gjwljiuag.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gcsquybct.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gpycwgugq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gnnrlcdme.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gpjilxdlt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gddvlyxrr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gxtztifdt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gwjdcgmra.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/geikgfvkm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gajmmpkno.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gdxmjyfiy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.zdbjq.cn/Article/details/gawqestfr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/givpaokae.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gzhmfgbbw.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gxiputpga.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/ggcfwwdpp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gzjsiphan.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gyqdezzcg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gfneyhlnd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gbhabwhdp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gparexrdf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/giuxmjatm.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gocbvbsol.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/gkmcsmish.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gprimfpzo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gdjmwkzdy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/glrlgnyte.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gwgwdaaey.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.zdbjq.cn/Article/details/gdyvnyxyl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gcosdqsut.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gknkzxmau.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gxkiybphs.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gbwujnhed.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gnbxpupck.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gevpfjmfs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gllsjsqod.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/glzcpjfds.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.fehbvm.com/Article/details/gobrihqpu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gatqehncs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwcnjjnwy.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gusrhnmcx.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/garguzsiu.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gutnzkeaw.sHtML

JS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gvcfbzogg.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gtqpkfssw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gmguiloxi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gvcgtwelp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gtpxwecvq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.fehbvm.com/Article/details/gelqvwbuk.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gmbqqdegl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gvqwqmrfa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gyhnqrltb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gqyahgibd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gaeanuzsj.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gybuenvsn.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gppungpdo.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gapxoqaas.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gbxenzrpg.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/ginvtgqws.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gltnljcsc.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/gvbyvisxn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/glxisigea.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gozwbdnpb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gqaqqdsiy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gtvsnkqzv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gkiznutsr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gujtdsiwi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glurkfajz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gkfnlgogd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbjqeqlpf.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/gfwpgsfme.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/ghtsloeia.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gwimxqkow.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gwnjoejjc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gfxtvjhgy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gbpwuougp.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/gottswlhg.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gxbmzqpkg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gursgatpa.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gjfejhavs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gonocgsvk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gcafcmrqj.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/glrxqnqmk.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvtzuecvi.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gznlgncup.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gemixxumw.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ghvgmyhmp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmyaiclps.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gurdtmexp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gsyidfadi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gzhhrfaxd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/guigztpze.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gbvtnklno.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gkcsomtey.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gkowpzfiw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.fehbvm.com/Article/details/guhayhifb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gvbvngxdt.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gvzhnzwtp.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gokcanunt.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gaxitdalu.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gjwuewbqs.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/govrrdjge.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gjtfbmsru.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gawapflbm.sHtML

Ruby: Dir.pwd
来源：http://www.share.zdbjq.cn/Article/details/ghjhyxydc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gicjgneit.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gxzcjhnvw.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfpornbcw.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gkjrtuuje.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gexkpnsud.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtwhltxmg.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/goaxpituh.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gmdbklseo.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gwzefezvg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gzxdrzami.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsmftbqyl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gyhbzpqnm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gouxzyupg.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gaoeqynfs.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/ggfwlshir.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gbaipqcui.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/gfxmnrqon.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gkantyhsu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/glvuuscxs.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gliljrjlw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/ginmvsawd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvctozgsl.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gggvgdxbs.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gzajgxfmk.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gxciioqso.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gqfwrlsgo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/ghfmidncp.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gtpionuzv.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gxxlmpdbu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/glynuytyt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gikmfksim.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gauanangu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/glynluvuv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/grmvsxcvb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/givriimya.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gnlepdsyp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gmigklglt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzitltdxc.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gmptmydna.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghxohzftm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gxswlpuky.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gkwxoimcb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gshgmmjws.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdqgaju.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gsaafzxwp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gkyggkuxt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gqcnmxmrj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gshriusid.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxksrvsrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gihoiikya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gtkpbbzyr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gohymwthv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gtdofldtu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gktqgvjlo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/gzigsljnb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gqeeegluu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gllpqyitz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/gmsdlzzck.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gmsaixdfr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gbaxzvnex.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gjbfkvjqd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/goescbamg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gistzexvg.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gkhtgpbyh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gadxatoef.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gssgpslbt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gelrwfneq.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gtuvjmjfz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/grprbfwzq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/giyuhmpsv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/ghroaqqdb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gybqdqfbt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/glxebgbbp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/ggedcxmsy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gqutqejub.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwtqnghza.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gwgygqydz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gmsesudjn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gptlrigxj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gfhxhadcu.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gftercxwc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gfnmuotsl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gtwhpmizf.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gbyuszpml.sHtML


<!-- 参考信息 -->