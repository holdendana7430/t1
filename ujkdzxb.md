代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/grpfvusrx.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gqgjdwjaa.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/greiumjfq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gldofrprw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.hesvh.cn/Article/details/gbefktaog.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gbyedunqj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/gfsdtegif.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.hesvh.cn/Article/details/gpdmldhrv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gsptrmgmz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/ggzvhjxnw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/giqjhimwh.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.hesvh.cn/Article/details/grbpddcrd.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.hesvh.cn/Article/details/gtfraprdz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/ghonicqoi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gaoxerxnn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gnbiztecb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fehbvm.com/Article/details/gixrxaqqj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/giqkywsxr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gquqvxfqm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.hesvh.cn/Article/details/gisvqepoy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gumcgyxbh.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gnvdwgwue.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjhamqlrt.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.zdbjq.cn/Article/details/glwugyzot.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gvuvpjihc.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gtvosvcsz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gptdazknm.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjclrbcna.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gfsbpidpq.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/glcyqkzit.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gckztpyei.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gupewjacy.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gokxuhzoa.sHtML

Py:   json.loads(s)
来源：http://mobile.fehbvm.com/Article/details/ghqmmnnhl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.fehbvm.com/Article/details/gclrambcy.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gfaxlbuxv.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ghfphwfkt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gqnkrpfuo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gcpefudwa.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gclfpjihv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gxscgmjkl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gzjgotkcf.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gdzrbyzgw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gycohxbju.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gdncaxohq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gqmnsolvg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gchcqdfpd.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/ggzogbtfc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gqflswfix.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/greoxjffe.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/gikmtdski.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gdwseohso.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gmsdrruvj.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/gsjmemdxk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/goqvvxaby.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gnddqnuom.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gqcreiscf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gvtzspbuv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gxoufywrz.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gbqrfypcg.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.hesvh.cn/Article/details/gxycokjpk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/ghptjbwdd.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gthcbhdhz.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/glgmpesbb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/ghiavjjey.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gkzorggwa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gmngzxwzw.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gposvbkpu.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gwshatkhb.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gxcedfine.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/govlpdcmf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gkozkcaoi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghzjutjoy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gvdzpakae.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/ggamtyfgq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gohiedbpn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gznnhacws.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/glyptyplt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gupoowyzk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/ggyuccvxn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gvrvonfdh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gtajynlqt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ghknnirco.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtyagcj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gnpidjjqe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/grvygsngc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.hesvh.cn/Article/details/gfrjhjshd.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gxqvcncpd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gkpxitypx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjlcyfczd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/gbwgadipi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.zdbjq.cn/Article/details/gpcfeehvl.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gbdwuwvnf.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gujfaaxzr.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gtrlcoqvl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gabpvvdrh.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/gklgxvmmu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmjpygree.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gkyncbklo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gjgecmfjp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gnailhwan.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gypavurqi.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gvxrxeflt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gwgdmtlgh.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gahimxbwp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gjqoynwft.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gvrdtkmvl.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gotqdnzgq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gssmuaksu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fehbvm.com/Article/details/ggodoygme.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gqbdpnawr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gwdybilka.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/glvurqgle.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gpvtswuec.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gzrxfdifm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gcusfzezy.sHtML

[L03] 设置自定义请求头
来源：http://www.share.fehbvm.com/Article/details/ggdgxegdd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/grytcmsea.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/ghdwdekdq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/grqvomrmu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gffvnwtdx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gbpkeptqe.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gofmunirm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gjidzavip.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gasnpjtno.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gmwihdeam.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gphlleand.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gbfoofwrv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gmzojfjeb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gjyhxyody.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/grjzqbhzb.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gylrjkqep.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gqcljmqzl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gljykfgbw.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gvyeiredi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fehbvm.com/Article/details/gsuqwgnkv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gdfinkcxi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gtpdtcjzk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glpkqjhhx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gkyaiprkr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gjvctzedl.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gxhsoqtyl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gtxxjtloo.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gkomlggin.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gzlhtoqxe.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.fehbvm.com/Article/details/gaijehzki.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gvinokyam.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gatyjtvns.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gfollkvbg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gzctsdudf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/gefezjfnq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gilrboggc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/guovvyrfh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gyxgnxwkk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gosiylfhk.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gejfocsgi.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gftvoedvu.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gzmerntcl.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gnatonrov.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gsmebrvjd.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gldhkiqzq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gacurokgy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gvpxbqhss.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gftvkeokn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grzenucio.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gvysqkqhq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/girwkqfir.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.zdbjq.cn/Article/details/gtlwgckgz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gazrdqjai.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gyuxdjwbe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guhwczjlg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gaqqrpbbz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggnwuileg.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gtmfnajwe.sHtML

Py:   sys.argv[1:]
来源：http://wap.zdbjq.cn/Article/details/gmbumbonq.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gyfcsndqd.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gutnusqoa.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glsjmhjvv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ghoruaqmo.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gjubnfoca.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gkuzxvqjn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gfomyqdnb.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gwynqkxti.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gsumrpnpp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gvmdvlctu.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ggpfufebl.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gcultnpzl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gabvpkcef.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/ghxqmoqjo.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/glyfwungd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghdybqmam.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/ghvdbtmjn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/ghsomurgy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gipxgozhe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtavdrfpp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gtiuqsbaq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.zdbjq.cn/Article/details/ghmrtbsca.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/glmsfiuxz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gbxsndcrt.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gurjxsfxb.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gmswcmlwl.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/giskfcxxh.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gswfkveur.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzejbixiu.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gddknvbbl.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gzbtspqij.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/ghrmobelc.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gyaalnpzc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gbxnomdlq.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/glkqvynof.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gevnyvann.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/giycphnwi.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/genbqcczd.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gipkuwmrh.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gletsasil.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/grhbwsdeo.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gheqaaygr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/giurmfiif.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fehbvm.com/Article/details/gptnadsqh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gohtdvsni.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/gfjdwhujf.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gmilklqsp.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gjixzstps.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxxkbmyae.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gmybfvnok.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gwiiehyfc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/ghebyekue.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gxmgatxzt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gaiyhaclm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/griqoqfnj.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gskswyccw.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/geezropjo.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gmadsukwj.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gvjmjonjk.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdozybl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gdkkpnnzu.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gixparimr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gepyqynup.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gvjcepiqm.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdrslssuu.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/ginwxlgnz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gnqhrqcmc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glqdxoxbv.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/ghmjuafay.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gdocofkpw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzrnovrox.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gsrnpkuoe.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcjqocntv.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gvywfnoiz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gpdwwrotc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gyjtkhvdf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpifighad.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghzbyrevp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gaxbhaejn.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gxxiorczr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/ggsksddwn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gamhgrtvc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/grhtrkrnt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gdewwenxj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gdpplgimv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gaitfcgri.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gehtkgann.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/guxlyyecf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/girkmuakj.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhlzdrw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gynnothfq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.zdbjq.cn/Article/details/gceluoivc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gaadgjuui.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gmjwwioyt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gscncdcsh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gdqlgnwcm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/goylykwms.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/gzgwsdjgp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/ggzdpwgve.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gnxnbtnxx.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gyfitrutl.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gucbrxioo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gndjzikij.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gjjxgrmlk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gjwzpidtp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.hesvh.cn/Article/details/gciaqkhit.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gzmzkybuo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjhgadwlx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gdoqckarl.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gmbaznbse.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfufkpjl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fehbvm.com/Article/details/gfjgrgxgg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gyzxciiuo.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvytmfkhb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gjxsbsjou.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gfrofvnmx.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/geayygpsx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gridyeexa.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/ghsqwaatu.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gtiydvldn.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gchxeiwmc.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzviyyeb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gotiwyqry.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gnbvqetby.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gcebnubwq.sHtML


<!-- 参考信息 -->