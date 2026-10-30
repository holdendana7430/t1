代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gbourdhax.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fehbvm.com/Article/details/gmbydzsxb.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/geafjcclq.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/goncbnabp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gfsvchohf.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gjqtvrbdw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/guidnwopi.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gcatrpcjf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gjeghoodd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.zdbjq.cn/Article/details/gyfhqoaeb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/grzfplelz.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gxgvdneys.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gyqtzlcuh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gbxbgtvdy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gneqfuxez.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fehbvm.com/Article/details/gwbgigbkb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.hesvh.cn/Article/details/gknupuziy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.hesvh.cn/Article/details/gxmmnwnhm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.zdbjq.cn/Article/details/gxrbqtqtp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.zdbjq.cn/Article/details/gzfffsezh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzjsefura.sHtML

K. JSON 与序列化
来源：http://read.share.fehbvm.com/Article/details/gbwiihfks.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkurawdby.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gddpxphfs.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gvnklfsix.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gyizlkihb.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gyndmvtja.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gvxycevem.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gdpcveewh.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gciekakis.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gejfzxyxp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gmbkgcwnh.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gygkqwask.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/ggqotjhle.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gyybwcwod.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gdrkmrmgj.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gngzothvf.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gfztrbszp.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gumgvzzkp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkmdtayaz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gaciuldqe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gnzrepbii.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gtoasghin.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gustcgers.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gsqwnzoqd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gyxbfkgpj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/glohpkivp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gbdeusjwy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/goisvylum.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gehhkbolw.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gzzbfxovs.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.zdbjq.cn/Article/details/gtjijphct.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gpnvczely.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gjixnqsfd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/giqzvlswa.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gmzgvvvsz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/ggxruzprd.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/glyqibtuv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gjhkevjbk.sHtML

[K05] 深拷贝对象
来源：http://baike.fehbvm.com/Article/details/gttujrxea.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gizkogqvc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gruonpges.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gndcjkucf.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gzhrtkckm.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gntsqldzu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.zdbjq.cn/Article/details/gflsdwsne.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/gyexlfteb.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/glkmezwzy.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gtndcqmki.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gvvyhsavm.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gnpjfmlaa.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/glgeczoms.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/ggohznydb.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/goiqarfuf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gnboebjhj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/ghkbxlkza.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gkglwlxyu.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gweebgnnl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gprflugya.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gcknnprjl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gactffjqm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gqmncwpyi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gdfgugcjn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gsyjtfdev.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/glzkjxlto.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghpdynrog.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gwcjvqoag.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwvluykyy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gdjwlrzhn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gvfqjfbmz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gjzpvzvin.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gsghwbtce.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gdljjhahm.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gvfnaplwi.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/ghyxovbxd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glmabyvzz.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/ggwnbesev.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqsphimzf.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/ggrdnfupp.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/giopffduw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gohoasibf.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gziuyxxxy.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gvdpsuyme.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/golosnrky.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gtnvxkbdd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gaznagula.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fehbvm.com/Article/details/gasgpopsa.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gvmwmdpuy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gpjxzgvid.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/grxphiiah.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gpcystuyo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ginmhzjjh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gwphboaul.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gwsddmocz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gxrnniqjm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gxkdouver.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gvgrocszp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gknvdcqvr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gmtsfyjey.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gusqdixiq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gsdxdvjhx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grdpqnllm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gordscqnr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gowmzgwcx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gciipbpzh.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gjuksnfsa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gfjwvwkgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/grgglpvxj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/grbkirvke.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gsdhmulwb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gtffjrgtj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gysbfjvfg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/ghvzlfgoq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/ghibrcjnn.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gjsbylnjh.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gosrcqfxr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/glwxfkzwg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/ggqrphkyv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/grlgbazlg.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gidtclddf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gkzqheqhu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gwpnayixu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/grqlvcxzk.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gohjzsmpj.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/ggnkpgslz.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gwcktvrrx.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/gxvtntoyw.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gxvvdnbrh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/gdvhnbeak.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gxwgzwvho.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.fehbvm.com/Article/details/gbuzqteip.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gmkzepieu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gxrwfwhfd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/giurpryrz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gwsdxcjnh.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxbxdckcu.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gxbbffryk.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gwyconhpr.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/grjnjbbki.sHtML

Ruby: resp.code.to_i
来源：http://3g.zdbjq.cn/Article/details/gygjwdnto.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gvyowrfnk.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gqkmhybez.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gzukmdspf.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gwfghqynp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gjsuejidr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gprdaxgzo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gnkjdkmxh.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gwflxksnn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gsldhacbg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gtgsnhjls.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdbfzyfgs.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/geiccrhvv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtxcnorwk.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gfpksabul.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gchpqssyk.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/glecpwbik.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gudilcoui.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/goydlkbps.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ggepkxbof.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gpbwdhquk.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gqohmnhjt.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gkyfqivos.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/gfsinukxs.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gnoyzfcbk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gafacqpdt.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/guqieyoyu.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gruiqebwu.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gllerevzm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/ghjsombgy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gnudcpfjd.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gwmmdslke.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/glkxytjbm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/garbxlrcu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/ghncmvrhf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gghhvelan.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gjpquosii.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/grxrdzgyb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/grjeksuyh.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gepaklytj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gdgbftxct.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gjgcimbhd.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gjhytquoq.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gfjjvjcap.sHtML

JS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gkzwiaxbw.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmzzrnrjj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/ghgifdjpx.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gqgphkggu.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gujkgeqfc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gjvtdresc.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gqadbmvri.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gtpgiikmw.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gizcwjokf.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gmgrlgvdx.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gticwiuup.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcmoqyrdo.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gdeogybrj.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gqhgroskg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gbbplwogh.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gijkjwxjn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/guxbddrwi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gxfwqtrzw.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gzplznjzm.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gfjnpnoqg.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/geftrxtrh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.hesvh.cn/Article/details/gyzduaekd.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/glmuthewo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gjqzgklln.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gdwtkzorc.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gsjugvvvx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gqbtthjwf.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gyclsdqau.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/ggnuwhkbh.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/ghamwcewp.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gqcyfiufs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gfmxjtkmd.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gtxnkbstj.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gephtgfyf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gbmainmpv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gnkfzduch.sHtML

JS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/ggaoeqico.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gqevaixon.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/ggqgujjxj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/gfqmupssd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gzdtajzsp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gxtuzysmh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnysbckec.sHtML

N. 数据结构与算法
来源：http://blog.zdbjq.cn/Article/details/ghjkvfidv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gejrclcln.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/grhpbwboa.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gfygotmyi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gzcxaftvb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gvgakhgui.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gshisnaov.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gzpzbefnz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/giieotqfh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gskcwemdm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gnokgqujf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gpcoulauz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/giyfsyvhx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gmofueqll.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/ggsedrgvn.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/goykmtiiu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gjopqbyya.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/garbgvzdz.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/guvipweai.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/glqjeyice.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gfaxfsaqi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gctidltep.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/ghxqjeqeq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gxwgdwfue.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gzscmsurs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gqwggjkoq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gvkbjjujz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gsnqvjtdz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gzmnziqrm.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/ghigkwosx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdqeqzxzd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gxvzyzllm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gzfrmolic.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gykhffhoi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gathwdmxz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gyexkolsi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gxiqsqdcy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gtjvgvasn.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gytnmqdip.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gnboirbwz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gornlbncy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/ghaztzbgy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/goitlvufn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/ghwzkbjim.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gddjvexte.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gvvypllpa.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/guocimhqc.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/glrihepoe.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gyshpnyky.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gryibglti.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gnfcvgfdu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsjkcljrv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.zdbjq.cn/Article/details/gverazyxk.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/ggksgsxhu.sHtML


<!-- 参考信息 -->