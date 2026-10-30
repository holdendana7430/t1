代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcdynoyh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/gpkoxlodo.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcsmaduk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fanxiaobao.xyz/Article/details/gfcoltzsv.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fanxiaobao.xyz/Article/details/gspwctywa.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fanxiaobao.xyz/Article/details/guiybfktz.sHtML

[J09] 时区处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwrepsbtp.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fanxiaobao.xyz/Article/details/gdmtupmlg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvidyda.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcijvrjwr.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gpeujbtuc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpmnabfz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fanxiaobao.xyz/Article/details/goexfjryp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fanxiaobao.xyz/Article/details/gjazcfdvq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfnmfmif.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoyploui.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fanxiaobao.xyz/Article/details/gxlfngqxa.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fanxiaobao.xyz/Article/details/glidbicfv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpipxngeo.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzelkwkdq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gnuweebff.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fanxiaobao.xyz/Article/details/gdzbavtyk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fanxiaobao.xyz/Article/details/gguljhxhv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guetzykjz.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvxkumye.sHtML

K. JSON 与序列化
来源：http://m.share.fanxiaobao.xyz/Article/details/glpmqxrnr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaabgklem.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gytwfthsw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gvallbsmm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkzmxqtn.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlndojbw.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcacidvdn.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.fanxiaobao.xyz/Article/details/geggencdx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucxumvgx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fanxiaobao.xyz/Article/details/gdbncauyl.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gvbzuiero.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fanxiaobao.xyz/Article/details/grbstpqof.sHtML

Py:   json.loads(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/guyuyfyah.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmnddpan.sHtML

JS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gkwrwtsvv.sHtML

TS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwxremqh.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.fanxiaobao.xyz/Article/details/gdhynucnl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/guqjzszba.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxidnebbl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gcnzurhpf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscfgenhz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcecvcpz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/glryvrybu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/grcbljyvt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgpbgjle.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpeuwbll.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmhmchrp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/granddjwf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fanxiaobao.xyz/Article/details/grdfdimiw.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fanxiaobao.xyz/Article/details/gqnwpvmpc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzskmbklz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fanxiaobao.xyz/Article/details/gplhbchgh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fanxiaobao.xyz/Article/details/gtyzsptvu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fanxiaobao.xyz/Article/details/gedsopzrl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxfosjho.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicpzcvu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmozhsjks.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gccfraype.sHtML

[K05] 深拷贝对象
来源：http://3g.fanxiaobao.xyz/Article/details/gksrpwrxu.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gffkuzklc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/gvjptdoom.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuqtmfxj.sHtML

TS:   structuredClone(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gnqlotfof.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/gxsoepzqe.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fanxiaobao.xyz/Article/details/gdcmfcmcl.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxcubqwy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fanxiaobao.xyz/Article/details/gkkhsvmoa.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gexdryfsy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gvxfcxbbn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdwnxxkk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqrhxaxk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrnklubh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmpdvjdn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgblxufo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghybpioog.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbvbrgga.sHtML

[K07] 进制转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gollqriwr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdbwqnhn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdokacva.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpbirefa.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlcxosrl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gjnvwrqyt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fanxiaobao.xyz/Article/details/gufdqbujw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gptjmxoyc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrvywmnq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/glxxvarso.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/getxeyook.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gscngtasl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gaoxwuufi.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdiawasw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/gfikakbif.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gngqnjykt.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrcxsqd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gsgodevub.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gokeddsfr.sHtML

L. 网络请求
来源：http://wap.fanxiaobao.xyz/Article/details/gblpcnidn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzenbkze.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwwvqrwv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyltikebb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fanxiaobao.xyz/Article/details/gbccjowds.sHtML

JS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikcejgrr.sHtML

TS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gifarlbdk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fanxiaobao.xyz/Article/details/gltcjcggk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprcikigv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fanxiaobao.xyz/Article/details/gatafzugb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbcpaurt.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gvgdzxwnv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gajtyapbs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.fanxiaobao.xyz/Article/details/gtygmslra.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gxkyindgv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gbhjndipy.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcinkdsb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fanxiaobao.xyz/Article/details/glheimlww.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/geboezbvn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxfnlmp.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/grirrwqru.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fanxiaobao.xyz/Article/details/gdkqxhwxw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gnpdinywp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/gvrgaezld.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzymhuvv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gbujtzlya.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fanxiaobao.xyz/Article/details/gppjlfcxk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaiakyzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fanxiaobao.xyz/Article/details/gualhixkd.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxpvhsrj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaabxjoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gknaawful.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzyoytel.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fanxiaobao.xyz/Article/details/gensdxojo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gaqbmkzuf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fanxiaobao.xyz/Article/details/gbumlpxyc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fanxiaobao.xyz/Article/details/gyzowuhnk.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkseiirrk.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fanxiaobao.xyz/Article/details/gwjqbnrcd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fanxiaobao.xyz/Article/details/grfnufaac.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpcrgjey.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpgbwdit.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fanxiaobao.xyz/Article/details/gatpsjymu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhqtoxxw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghlbyehrc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywhuwdge.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuespllp.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gsumibexg.sHtML

Py:   resp.json()
来源：http://blog.fanxiaobao.xyz/Article/details/gwhfgjsvk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ghtvnqicz.sHtML

JS:   await resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqtzkzkv.sHtML

TS:   await resp.json()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlbaqucm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fanxiaobao.xyz/Article/details/gjmgczyka.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fanxiaobao.xyz/Article/details/ggulqdmei.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fanxiaobao.xyz/Article/details/gozhwpezg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gljciayyw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gwaeeszau.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fanxiaobao.xyz/Article/details/gnulnmavd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fanxiaobao.xyz/Article/details/gfvrejhfz.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvrjitbz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywnmaskt.sHtML

Java: resp.statusCode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcrpjxlp.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gdwbzzcyw.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxcxkwk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fanxiaobao.xyz/Article/details/guzaxpsnl.sHtML

[L08] 并发请求多个地址
来源：http://3g.fanxiaobao.xyz/Article/details/gkyaxoflw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkddvkwf.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fanxiaobao.xyz/Article/details/gpbsljlup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gxsnexmbg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/geiwocijw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/gngqewvey.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fanxiaobao.xyz/Article/details/gvfonjlxm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fanxiaobao.xyz/Article/details/gmihozaxx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmexyyvh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcjwmcfa.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fanxiaobao.xyz/Article/details/giywwpqom.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gudsqiygj.sHtML

[M01] 读取命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyzrcaom.sHtML

Py:   sys.argv[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gplzafwwh.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuvoywhc.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbamrdkrx.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyjolslt.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fanxiaobao.xyz/Article/details/genappcnj.sHtML

Go:   os.Args[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gpayknqxa.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gjypmtwlw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gjblcujnb.sHtML

[M02] 读取环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyeabzxz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/ghluzfwxy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuuuxgll.sHtML

JS:   process.env.HOME
来源：http://blog.fanxiaobao.xyz/Article/details/gmgrfumkf.sHtML

TS:   process.env.HOME
来源：http://read.share.fanxiaobao.xyz/Article/details/gajoaedyz.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gclinuumw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjdfnseh.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fanxiaobao.xyz/Article/details/ggxmltfip.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.fanxiaobao.xyz/Article/details/gdlhdnpbk.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gwyxztyaj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnovmjsv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpfbowue.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqpeqowc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsktjvfni.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fanxiaobao.xyz/Article/details/gqkoatued.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fanxiaobao.xyz/Article/details/gjhlhizqp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjjdldfx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsuhfddu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpqhgxeo.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfohavddb.sHtML

PHP:  getcwd();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqhwyouk.sHtML

JS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gxjcsljep.sHtML

TS:   process.cwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghngwhjuc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gzqvxurce.sHtML

Go:   os.Getwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwmtmfqq.sHtML

Ruby: Dir.pwd
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuzhymuw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnuuofxm.sHtML

[M05] 设置退出码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqhyqihq.sHtML

Py:   sys.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gzlbntnuc.sHtML

PHP:  exit(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikzvpxmc.sHtML

JS:   process.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtwaoqst.sHtML

TS:   process.exit(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gsltgdcrl.sHtML

Java: System.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbnvnxae.sHtML

Go:   os.Exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzddfizml.sHtML

Ruby: exit 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gidpablez.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gykehbnvs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrpxuaru.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fanxiaobao.xyz/Article/details/gqtugsxyn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fanxiaobao.xyz/Article/details/gkbkvgeon.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/gccukgypa.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgpfpzci.sHtML

Java: System.err.println("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gspmhuuze.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fanxiaobao.xyz/Article/details/gghkvvtgc.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkaxdgds.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbigrmmpj.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fanxiaobao.xyz/Article/details/getxrxwjt.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gtlwbkhpc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtrmvcvb.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/goydyyuza.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gfftqcety.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gczqiohwt.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/gawdmymko.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaissouh.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fanxiaobao.xyz/Article/details/gbxsgrjll.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkwiiqbf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fanxiaobao.xyz/Article/details/gbmgzpcfm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gljkwboxb.sHtML

JS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/gnzcjhmwu.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbugghrh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsmitquo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeovxooi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/grlzrvjni.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/gqqmrtrcg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gffkyqsve.sHtML

N. 数据结构与算法
来源：http://wap.fanxiaobao.xyz/Article/details/gukboytoh.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gpezmmzzw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gglrthglm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxxtofio.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilawsshx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/grytdmzge.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwpsryc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gekzeubfg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gkfrfszqe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/ggpzftavb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoinqvsp.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgqdtjun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gbvotlhpw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwegacshe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fanxiaobao.xyz/Article/details/gwuxkghrr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsorlcgs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fanxiaobao.xyz/Article/details/gshiuuucp.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gesjicsbt.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/ggmssztqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fanxiaobao.xyz/Article/details/gcxcrzwba.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gvfqwdulm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fanxiaobao.xyz/Article/details/gvehywbdv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkwonusn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fanxiaobao.xyz/Article/details/gmmzppdqi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/gtcbgfawx.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gprvhwxqd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fanxiaobao.xyz/Article/details/gcijlhtit.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fanxiaobao.xyz/Article/details/gmnophaoh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fanxiaobao.xyz/Article/details/gcfnjjgxe.sHtML

[N04] 斐波那契数列
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhvuepj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtiefarwr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvjiwbeq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpksemdpu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fanxiaobao.xyz/Article/details/ghsimvgnr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fanxiaobao.xyz/Article/details/goeczpryu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggalfdqhf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gfuakiluf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/glzykdhly.sHtML

[N05] 最大公约数
来源：http://3g.fanxiaobao.xyz/Article/details/gamoyadrj.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gynruyciw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwmvlpbr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaelflks.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsekftxug.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggpqnzypl.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gczstzrdu.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjuwgjbx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyebzdtje.sHtML

[N06] 判断回文字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/givabeavl.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/glqqubvkg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghipsptfg.sHtML


<!-- 参考信息 -->