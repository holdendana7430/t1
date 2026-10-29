代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gjocisqvg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fehbvm.com/Article/details/gyxyxmudd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.fehbvm.com/Article/details/gpvcmefbk.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.fehbvm.com/Article/details/gquetlvwt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.fehbvm.com/Article/details/gluysebhh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gqazzdshh.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gkrjhadfb.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/goziyrynb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gsndfjpan.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gdoseulww.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/ghvivdteq.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/ghkodlbld.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gvensknzp.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/ggycwqwbh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gjpshhcvb.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gemgjvvil.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gafbnditg.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gmgwyqhyr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gykinnhwn.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gcngfviww.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gzpcjnzay.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gcfzxaorf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.hesvh.cn/Article/details/glqtumvlp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gdcwxuyvg.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grzuphuwk.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gqunzwmqq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjhgfomad.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.zdbjq.cn/Article/details/ghttripzf.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gppmomcdb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gngarybro.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gxbxnqpte.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gywzrxnwr.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/goyqepomt.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.zdbjq.cn/Article/details/gramgcphp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/grrkjmnij.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/gaqtkoipv.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdseraqau.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gfcwnlokz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gigxunzxz.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/grhxeocoq.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gudutebfu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gvxqnyiap.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gbrfdxawl.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/goqjiexut.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gafxvmpnq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gghhpsrsu.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ghzypgujs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gmcgfrppi.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gkfhbdzrl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdiflqjgq.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjpzohjji.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gxbtwszjr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gfkkqfhtc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.hesvh.cn/Article/details/gkssjtqrf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/gqfxklloy.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gbgvqmxwz.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gbvgdbucf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gmvbdhyxl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/goxluzxvt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gztfnwict.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/ghmgjfhjs.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gesbsppyg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gyutmjaac.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gboykchqy.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gxpmtsvbe.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gpkfdumoq.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/giunwaggg.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gfdaljgzv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gmmvmtpig.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gurkipmsj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gtfeystaa.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gjdscxywv.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fehbvm.com/Article/details/glgsnkgtk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gavcccctj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gxxpsfgps.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gswalihrj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gzelmltwl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gpmrsjoaz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gxvsqijbz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gqlmgaruq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gnykawfvy.sHtML

[K07] 进制转换
来源：http://m.share.hesvh.cn/Article/details/gyterfcdt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gcocawakf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.hesvh.cn/Article/details/gtttrpbtc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/guxpckujh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/ghxddyhvy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gxbibbqul.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/ghmygokxh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gdpyxcfdi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/glpbtjein.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fehbvm.com/Article/details/gpinkcdvi.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gggynuzrk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gqiqdjlsa.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gxzumndbu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gfdjumlpk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gabxefgkd.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gweagismu.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gpfubetjp.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gkuvyeqdh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtupmyseq.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gotosvguc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcosvomko.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gftaaswnh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/giffvkuzd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gwvuyjdbs.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gemvktsvf.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gtfqbvnzd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gmhuvucck.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/goquorbqg.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gpqwxqnio.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gbanamdsl.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/goffwsnwg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gvpjmayfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gupeovezc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/ggrpqvdgk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gjjvsoyjg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.zdbjq.cn/Article/details/gyspultfj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gqknzvctb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gvqgffpyx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gmnujmxdr.sHtML

[L03] 设置自定义请求头
来源：http://m.share.hesvh.cn/Article/details/ggvwomzbv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/giuubzlld.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gzyapkjwg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gowefsrlo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gyogilwzz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gmchvcecv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gsiinkpzx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gyxjgttwv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gxnwcxpsp.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gakcktfoi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gzllwmrrl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gztxfrtzt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gsjkogxbo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gsqlgmoaj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gerynmllu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gwjoinxtw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/ghrpiznbx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gzlgspxqb.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gajbnthcx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gpbsnrgun.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gitmvyeap.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gghmddvbu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gmyescfmi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/ghkstvfzc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gedqjeczt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gxkugewxv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbqfwmzqr.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gwthlfacl.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gncjgfhdi.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gydhgywzy.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gxxbmbtpo.sHtML

TS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/ggwdhbxlo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdscaefza.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gkpdlzjop.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gszjsiqqa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gpxsszffx.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gwoppchzb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gjxyzyedt.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gnbvunxyt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/ghxhofont.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gubmwmoze.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gybuqegpp.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gsimocxgg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gqtypejnh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggdrovboe.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gjtquepdr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gbqbmqxxh.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/ghfjdytbt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grxjazfvn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gsbtmfaeb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/giunjtpdo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gmxzgcyks.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/ghhhmpxxt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gepbauxei.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsfduzlqm.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gevbgrcbk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gkunzqcuk.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gnakgivvm.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gmiwnszwq.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gdfusomng.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/giauvdfic.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gthycvlwe.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/guwczycjp.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gvuprfagj.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gqpwkayyj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gnjylnseh.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/grnaoxewb.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gblqvgmvp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gcykxqkak.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gpslzqqxe.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/grniolhin.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdnnztqwi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/giabvwgyf.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/guexgfucw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gccsnunnp.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gayfguzuc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gppfxddfd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.fehbvm.com/Article/details/gfcbfammb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gybzlbavd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gtthvzlhy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gzrswfrjt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gqeiznavc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gazojgwhe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gaiixazzf.sHtML

[M04] 获取当前工作目录
来源：http://baike.zdbjq.cn/Article/details/gpbndoztf.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gwosokdhw.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/goenqtiao.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/guiuknlrp.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gfpnlpteq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gjfhtoaul.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gmldxrbvd.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gkrrgylit.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gbmemjegw.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/grywcjczq.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gqekmhvtr.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gkikfhtza.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gzhphmgxw.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gyalxzjcw.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/glrfjdnhq.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gcahccshd.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/ghulkctqe.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gxtxbyjki.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/grvcogbsh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/grxgbhyyv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gjeaaijjf.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gnacuqxiv.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gkovkktaa.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/geumsnztw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gwkjxeafi.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gifmdckae.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/gzjwjlxak.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gdnwqbwxe.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gvgnfqlyd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gxozmlgyz.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gsaavqyry.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gttwwocvt.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gyuqwfiar.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gjewlaemc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gzrryizln.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/giimwzrhq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gdcjacgfk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gfjwpfcuh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/giigdukft.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gqgsjmtag.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gvmsfsfca.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gfdcspicy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gmfmzqmhh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gpvmelbyg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gufitljzt.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfsxflzqg.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gnttlyfvd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpdfxyzjq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/goawhjvup.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/gkmptutfm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/ghscrdheu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gsekuqqct.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gnnvfpypt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/glvudmnad.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gokmbvswj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gyuxhjlng.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ggiixfpwv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gdakjycun.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gulggriqo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/glqiuayjl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gnhtnaoln.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gojasurqy.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/guaqwmoij.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gtlaxokhk.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gtviarsid.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gythpnfwf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/gmgiocrpd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gucibmawc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gpsziyazd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gbmekxapg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gbhvdccsz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gcjrwjuqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gqxgtlyoc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gkfnnxvxa.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gwrefvufh.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/guxpqcwim.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gadomtuxy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gmvrlnlkp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gsvsmamxe.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkwclxmrl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gmkepfdps.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gombeiijo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gnckzojqh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gwswkyzot.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gfnchabii.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/gfrfingiq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gmttziblk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gfnkfauzt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gfikrcjzm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/gkezvubbo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/grvxcvhag.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/ghthdfuwt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gvifiybac.sHtML

[N06] 判断回文字符串
来源：http://read.share.hesvh.cn/Article/details/gtcsplhwh.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/ghwybnfcf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gyzxdkojd.sHtML


<!-- 参考信息 -->