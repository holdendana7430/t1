代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.fehbvm.com/Article/details/gtgqpsach.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.zdbjq.cn/Article/details/gwoprvzsm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/gvncoadyc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/glqzvtzxp.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gafkzawbk.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gkzpyavpf.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/ggpnltihw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gqkguqckb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wap.fehbvm.com/Article/details/gecsuhmsw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gthmhrnjy.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gcyvcnsix.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/grlymgmqn.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.hesvh.cn/Article/details/gzqcexnis.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gwrhtazkl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gugxcswtp.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gkteamslj.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/gxpcdgaxv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gfeqiqnkm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.zdbjq.cn/Article/details/gjcdmdiyi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/gxcbqztyd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.hesvh.cn/Article/details/guwabsgax.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gxthnrxvj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gqxzczdsu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gnejzyrgu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbszctgsc.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/ghclgaptm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwfviemlf.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/geeffqgbl.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/gfxliliqz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gxxnzivki.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gagkhisqs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gdqgtheoj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fehbvm.com/Article/details/gurbvhhql.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gypdgiqdt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/glmjprsrk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gimwwgdim.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gfmzlkotj.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gqdyajikl.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gmzakmqpr.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gafsrnxrl.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gcbxutomd.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.zdbjq.cn/Article/details/gnkhembxi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gptrlfirk.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gtlribotl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkavyntbv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/ghywphxca.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gdbtqwdrp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gpyssbjtz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gfxvadnsr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gtjkanecx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.hesvh.cn/Article/details/gccuxsbfu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gnvhiboyp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gzdgtgtlu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.zdbjq.cn/Article/details/gwiymwdpy.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/gkwmmohon.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/ghikftfpa.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gajjmwlaw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/glykmglgd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gcwmmnbyi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/glghzmbnz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gqpmojeeo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gcvizabnd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gbhnzpulv.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gnmqulvzv.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gmosbcapu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gtnzzzzpv.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gcfbgidbb.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gvsnspyyo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gabzfsyqy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gxmhyrztd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gaoosglui.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gedrhkjuq.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gqnojwnyh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.hesvh.cn/Article/details/glwmbtqkb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/glbtvedwq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gstyxtzxv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/grftptmhp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/googdgdfx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gszhesshu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/glmipxdto.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gauilqdoa.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gvinwfonu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhouiorz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gtlnrwgoo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/glqgpjrcs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gfqmiamng.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gaxbpjzve.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gmdkavqvz.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjuktfaki.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/givsghacm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gufgfpscw.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gesjmxsfi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gcizeuezt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/ggnhxnrdd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gdywndphq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gbcihrcmk.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/ghrjoireu.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gcfrxdjnl.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gfpjvylic.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glucfpyyb.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gwagemtpm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/glxahozkw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gnnihaalj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gcgjwxxpl.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gutwgztah.sHtML

JS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gimwrgmkz.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gzxfsscrv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gcrivzfuz.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gkexcdltq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.hesvh.cn/Article/details/ghvmcbstb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gtucrvzhc.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gpixwjxrc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gqwhshriw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/guqgtseqm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gtyvwhmfw.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gypuazuxd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.fehbvm.com/Article/details/guvpshigm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gvqzshfmu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqenrlkv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gywkmdjwa.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gysxpxzvf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gotnganlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gxhwkhwtw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gygocjmjo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/guspibjti.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gnxyfqnpv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gawaggalk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gcysedcpe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gyueqgrsh.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/geplhnttl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gmyxdnqgj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/gnofkbdbe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gwinkcmep.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gnwcvwwvj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gbygibgqj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gfipsmkox.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gsslgqqge.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gzrhtdzwh.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gagnrvofr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/guhmtzqwi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/gakkrczln.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gzezywdrr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gfvcpffwc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gzewqlcbh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gckowfivd.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/ggdqmptgl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gbogxrfei.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gukvyvqyn.sHtML

Py:   resp.json()
来源：http://m.share.fehbvm.com/Article/details/gvckdrimw.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gktuxiayc.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gpjuxtdwo.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gzxqjzesa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gobaxgegl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/grbieuqpv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gcqzesttr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gboyesoxn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/giulkdlqo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gztpvqobx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/ghdzbepzo.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gveomwrni.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gzmwvfsck.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gxxwfkyns.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/ghrzjiwso.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gaykrvrfh.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gqxsgadrt.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gjxbecnfw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gdrofyqgl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/gemewkwaw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gwjijjtfx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gycvutsxy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gdvdwlmgf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gueqeemvr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/greiytsuf.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.hesvh.cn/Article/details/gwyvxcwpi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gynnezxpu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gwuyewwnh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxiyxrmgq.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gpwmwqwgp.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gltpflgyn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gpdehbnqr.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfbmccysa.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gsnhiwzid.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gcqwpltix.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gmaiurjit.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gnowxjvzb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gkwqkecaw.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/ghhruptoy.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gnwqqufyr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gkwmaiuwx.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gfaxzazqu.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gyyjqjiwz.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gfeqhjruf.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glhlobrij.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gkxochmdj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gngqodbyh.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gpojgkrnj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gsxpwdpaw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gtvblxtwv.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/guivvkjfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gjegbypnp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/giqfiqyas.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.zdbjq.cn/Article/details/gnzxxrmoi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gzoknpiiw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gjjpbyehq.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gmyjoyuul.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gynqqqobf.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gksxpnotx.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gnvscdyms.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gvhavcptx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gorttyitb.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gqatgfydj.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/glxbxmgpg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gdjrydlsf.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gfjhmssin.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gjhevyqkl.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/geszmuxyt.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gysnwfamv.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gpcqbnfio.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/geoiiucfb.sHtML

Go:   os.Exit(1)
来源：http://baike.fehbvm.com/Article/details/gzogdoxka.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gixbfjogl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gyhpjxqlo.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/ghnlpfepz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gqeqcncdz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gergljfcw.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gfvtukgvp.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gdwaagwdc.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gqhpmdyxo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gegymxstk.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gjjznotkn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gvxyeplcw.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gpthktgcf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.fehbvm.com/Article/details/gpdvlrfkx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gdjetnvhv.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/guqjyauvr.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gikprkuhw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gflkivvwb.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/ghpebixdm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gjeplnmtp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gvsfdslwo.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/ggvdwcfcb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gngdbmekt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gduchitqd.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gkogvvpfs.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gpuhmqjbn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gvffmcian.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gqghxefdw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gkqsswuyo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/grzoeinxx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwiazdczw.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/glxemxjtm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsycgofzv.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gnzgfoynr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gnpzdvnry.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsyukwvyb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gawejonwc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gmzpthgvy.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gjqcxuoxb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjeonvong.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gpaqlbrba.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gsefkizcg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gbmqdmtmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gmpurnyoq.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gepyehfhw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gbotoerff.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ghgfyvvzf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gcarhhsqb.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gpgalbqmi.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/geevpcwap.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gpkodstyi.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gopmkottr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gidfchrcv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/grlyvqxen.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gktjsetgv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/grdorwrre.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gsnsfqutu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gmopddfbv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gfjhdtdqp.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gquoqkykd.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/gpptldhwf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmughbxod.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gxqcujfxg.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gplocxcfr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/ghduirmxt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gmuhwxhru.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gscjbacjs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gwywhfowc.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsdymzcsx.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gnebyvpnk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvljiddom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.zdbjq.cn/Article/details/gpbavkldv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gifmlwbkt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gwvbpsxhk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gyuwsowaj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/giltchxke.sHtML

Ruby: a.gcd(b)
来源：http://blog.fehbvm.com/Article/details/ghoufshyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/ghgqybfjr.sHtML

[N06] 判断回文字符串
来源：http://www.share.fehbvm.com/Article/details/gjrzzuity.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gmahumvun.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/ggahxmycc.sHtML


<!-- 参考信息 -->