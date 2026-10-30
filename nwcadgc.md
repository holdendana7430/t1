代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://3g.hesvh.cn/Article/details/gjfaizbbn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.hesvh.cn/Article/details/gtuczfjji.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fehbvm.com/Article/details/gfylcnudo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.zdbjq.cn/Article/details/gacjhcmmh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gqphbrnrz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gusvhifeq.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/guihnjfse.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.fehbvm.com/Article/details/gifqjzuyr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/ggdrnbokt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gtyyjzspc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/grpgxxtim.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gvcvsdjpv.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/ghgqqyhvm.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gtxwskdhu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gucedinlo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gxofvzssg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gzgkjbftz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gigajcjes.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fehbvm.com/Article/details/gxnpxflpc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/gckdiyyrb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/ggodilxol.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/geiscrxpm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gfhtrflbb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gsfzklejp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwmrfmtzm.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/govawqorm.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guzpzeoxx.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.zdbjq.cn/Article/details/gmzyocahg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gkyfezxaw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gvasieorw.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbnbajeiq.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gxplxtwse.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gefuhhrvp.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghfxncwbu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/guynjegux.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gvijfjohm.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gmrtgobaa.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gsexawpck.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gtiifqzpj.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gltfapyxs.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gtrtqokdt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gfpmfxirf.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gkxfooszb.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gahcltcrq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gjtxacusm.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gwhbdhxdi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gfmyvaynt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gatugwcqo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gcxyzxziq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.hesvh.cn/Article/details/gtcnjhazm.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gmemawdkh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.hesvh.cn/Article/details/gypykkeze.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gscmvjstr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.fehbvm.com/Article/details/gubcvslfb.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gtzclevwh.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gjqqhltcm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gwyxpihdp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gzauvsrfc.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gkdipsmhq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/ggvasfzsb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gelofjwou.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/ghshwkilo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/guqhxljop.sHtML

[K05] 深拷贝对象
来源：http://wap.zdbjq.cn/Article/details/glrjqmdrj.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gqejgiweq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.hesvh.cn/Article/details/gimoajbwk.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gytbicfod.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gorxqneca.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gcovpqxsg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gddwkkmmu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gdmoruvmn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/guimpkkza.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/guvsyaifh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gbfeppnkw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/ghwtwzkhb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/ggekntrry.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guleoxdxr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gwwkxeswf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcggheysy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ggmmgugcu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnjelzty.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gpulzpdoz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjhfiqcep.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.fehbvm.com/Article/details/grunlvmpo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gsjggonzx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gdwrhtchg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghinbogef.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gyzuuvqbg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fehbvm.com/Article/details/gofctwrev.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/govulhboe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/gthliwjbf.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gpkdxltml.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghxxugnco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gmzotsbgh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gcuqxtavh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gjjqxfkiz.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gflfbqwhm.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzkoheogx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gtiquckqz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwvexmtoi.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gsiqrsvod.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gavtrwdhu.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gcmcggtrn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/grpbegxoo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gmgtioxgg.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gegagljco.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gldxwfegj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/grlpvucil.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gkszzjgdg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/getenyqen.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gvgsjygqv.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gkjkvldxa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gsitsueqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gjvzgdjgv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/giywzwbkq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gvfldiuxw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/guxnztwsi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gvudygjko.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fehbvm.com/Article/details/gtayxnnhc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gkzyrbtfe.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gtjxkkweu.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/ggmdglonh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.hesvh.cn/Article/details/gnbjkyrut.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/glnrswhkk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdkishvwa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gyvmojxup.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gsqdcubkl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/goyqrexvv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gvlzobpkr.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbtyyrv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gpseejrbm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gyqfqhrfu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gdbtfrlxi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gohbwzxxy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gjvnuyfxn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gfkqvwwvp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gplgkncya.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gbucnjkew.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/grotxjjza.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gfbezryqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gpgmvpjzu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gzezzcgrm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gtnwpokoa.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/gxophijss.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/goqrgnazb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gtsizqxps.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyhkzjftu.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gdcfgwbil.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/ghyorlzvc.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/glospfsxc.sHtML

JS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gotsbigti.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gkmzirwoj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gfmvrvmpj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gbgfthxqf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/guwxpuqsl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gcxludvyz.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gnqgumqxp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gxjnmpmoe.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gorzavqal.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gkuggsgar.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gizihqwhs.sHtML

Java: resp.statusCode()
来源：http://m.share.zdbjq.cn/Article/details/gocwvlosl.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/guccgghcf.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.fehbvm.com/Article/details/gnbmgovyx.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gizbmcbjw.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gldadthhc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gdlyvbnnm.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gqhbpjkxk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnokuqfco.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/ghfzbedfm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/ggvjjoggn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gnecaipde.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/ghjyzomud.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/grjavdfnb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gplgmpabh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gjredpbwm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyxixhoae.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gagmqgeqc.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gnfwktuze.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gimjfzbja.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/guhcgsysz.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/ggkqbusuh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gkklstfhp.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gfavyxafs.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gcnbxqpzi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gufzrrith.sHtML

[M02] 读取环境变量
来源：http://www.share.zdbjq.cn/Article/details/grntdjpmh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gowfwazjr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gyeoaqfvm.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gqgxdlkze.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gjcqjzqfk.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gfrtngsqj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gqfgffhum.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gmigaycdo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gtjptyjxx.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gqqfvjpft.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gurkjtqfg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gyapjdikp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gqwnvolev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gecsksqgg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gpjyhckgw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gztxapsqv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gzjnaukyl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gpzkhhifs.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gbwmvsusy.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gephowuga.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gzaafzalt.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/guilkdzzd.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gysfkiymv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gjboqwaky.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/glfoxjtqg.sHtML

Ruby: Dir.pwd
来源：http://mobile.hesvh.cn/Article/details/gprdfqllm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/grjjypzse.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/guhzaqwcw.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/giswodnvp.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/gxzkbqdyr.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gqafslrob.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gjlycptuz.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gdnmevbhg.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/grtcotbtx.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/giicsxczd.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gppwjoyiw.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gianziyui.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gxyessdru.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gktecrtju.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gsrtjoxjh.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gissotsud.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gdsnbytex.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/gznvmqjoa.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gvikugosw.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/gukkjwctw.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/gnsojhaxy.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gtlnttlvf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/glwtbrqgd.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/ggchwpoxl.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/glofttohh.sHtML

Java: public static void main(String[] args)
来源：http://www.share.zdbjq.cn/Article/details/gbyqbzwdm.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gktmvpzxf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.hesvh.cn/Article/details/gopnvczqc.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gyggciatl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gqnkdedye.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/gaqrnfduk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gldspuhzz.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gpyvzvugb.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gzbrbgdcg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/giowkukvs.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/grqzgbked.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gfqmqlnen.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/grhoynfdh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxvsdpevu.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gnzjkmobf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggvwjbnzt.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gidbsqwav.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqnbhqubn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/grcfbgucu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gqvrlqljh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/guvuantyt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gdcpvijgu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gygacsmwf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gwnzzzhmt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gyclemcyy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/gucfaqshq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gwybuaikm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/giqvcuzze.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gerewaacy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/garqioqes.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/ggzgjzibw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnbnbehrw.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gxamgsmua.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/gmccstesj.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/grjjbovbe.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/graoxfcqd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/geyipfvjx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gqxynhuxn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gdynpaeuy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/gyrqiuzgg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gjzkgjwix.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/guaannbxx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gqysjbcee.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqpvvrxcv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ghtqdwzmz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gwgayjgtr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gurbfkyjd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gzsspikar.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gpsysucqp.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gpzftbukp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gwedlzeht.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gixrwrxgh.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gjzzuikez.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gecbrxjdh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gakuuhxmr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gqfnnntdh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gjhuqswvf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.zdbjq.cn/Article/details/gwzzvuddy.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gfskoohkb.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gvoslmewu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gcchskuvf.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gkcrgrksm.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gfmymgfuo.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gikamfyhq.sHtML


<!-- 参考信息 -->