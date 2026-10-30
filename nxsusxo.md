代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/ggnqpigeh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gxlblhkpf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.hesvh.cn/Article/details/grgpxhkyw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gnybudkax.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fehbvm.com/Article/details/gmuwgdtbj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.hesvh.cn/Article/details/glzvmkpck.sHtML

[J09] 时区处理
来源：http://blog.zdbjq.cn/Article/details/geirjpylf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gsyxplezg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gcpazkbeb.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gvehaafmc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gqvgpnyae.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.hesvh.cn/Article/details/gmxdljwbc.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gderclxhy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.hesvh.cn/Article/details/gsqczudcz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/ghlaoxsgk.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/ghgmjdwte.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/grssrolyy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/ghtnbwlry.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpbbucijh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gchelxhwf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gftmevogu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gffsviirc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/glfqjekbo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/gyyyiiyys.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gswnwdtui.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gfxdefkna.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzuccvhgd.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gsvxohdpc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gopjfopty.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gsrtwqduu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gpzfpabcz.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gsksiofpe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gfxelpuon.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/gtnamlixt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/grisbtenc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gdbexpmly.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fehbvm.com/Article/details/gfkmnjmox.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/goxpmkowx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gsuxynurd.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gavrgeeyg.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gxfjruvlr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdnwafsqq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gxhlrgsjq.sHtML

Ruby: JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gcxewxmqo.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gnnyjoixi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gayjiybfh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gofbguscd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gztemcqlv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gafahqlyu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gzrwmnlgg.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gjatdczjl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gxdqkwpxz.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxqflftvq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.hesvh.cn/Article/details/grmewfqnr.sHtML

[K04] 读取 JSON 文件
来源：http://baike.hesvh.cn/Article/details/grzyfpczf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpfdqoyky.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gdbvgohvi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gdfkexduf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gmmsqxkzp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gsdgnelss.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/geccmraif.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.hesvh.cn/Article/details/grulzvrqb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gmhzkoald.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gukyvyvvh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gakuwifci.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.hesvh.cn/Article/details/gyfvxsfdd.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gaiyquuoz.sHtML

TS:   structuredClone(obj)
来源：http://wap.hesvh.cn/Article/details/gzhtatkei.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gkuxlsfvl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.hesvh.cn/Article/details/gcpcmjohm.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gltmyegfc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gmmdtvysd.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gfoeddghi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gpayebiec.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gdjbicgvx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/ghscrswbp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/ggawxkfly.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/gbewblvuy.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gorqxaqcz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gubnbgwmf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gzvzppwle.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gadqdaspc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gvctxvhnb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/geekbutfd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/guvffwxgz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gagyliuwi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzpwahpjj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gdabysnpj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.fehbvm.com/Article/details/gnvipqkmv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gfypqhmdb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gowbcwlbn.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpvmcnwuh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/gzlehthfi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/grrgjfujr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gboujxjjb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gontvkvfc.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gwxeyzoor.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/goclistzz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gimowtaan.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwzshufai.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gvhgtfsic.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghqfpdfbd.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/githudvmd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gvrjrvvqa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gcuoaketa.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/goowdynqh.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/glwasgejz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gfsxzioev.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.zdbjq.cn/Article/details/gkrukpels.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gjvdiacrb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbcjirrve.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gpxwovfnw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gvikbcbaj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/glhzuwxqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gzxnadvyp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gfbsjngfa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/goiugzknu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/grrehkcyf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.fehbvm.com/Article/details/gmtibtdxm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/giackkrjo.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gambvyywk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gxjfltuyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gpstmvzxq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/ggowzbpic.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gjbppnfzp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gzhojkoqq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gzzyaelco.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gmjpjwcek.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gdezidcaj.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gcjwbenkb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gejkezpqg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/glshggydo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gqbajnzqg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gjivgtfsj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gbynutgrj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gspymsbph.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gkqaxlylj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gsyinslzl.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gfszdhtew.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/glkemnpco.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gdzecrzdv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/geykvwprs.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/ghlsykeuf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gejnhifvv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gyxfxnaln.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/grgqfxaqr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfqwooxle.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gaennpaye.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gsujlmivr.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/givpqdxic.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gqfvgpgug.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/glupaytaw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gsotfzdke.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gboqcywov.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/glzrntoat.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gwqpdsfoq.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gdgfzihgo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/ghjtkzvjw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgfgthyu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gxdvswbug.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/grdkazfvp.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gabfxagyu.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gvwluhkjz.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gzgohtsff.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/glmgyukrf.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gynklaqzn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/gfxppzvbq.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gkzwjvmhz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnkwwrsak.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/grinqjbdc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gjimkqakb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gvucqkmum.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gnbopicrm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gdwumygtj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/geiztcwew.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gqrtxtlhv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqitmjvwd.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gvdncsama.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gvruedqlc.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gcbwiiumo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gbrwwmpuc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/geuwvyzxt.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gyziuolnf.sHtML

Go:   os.Args[1:]
来源：http://blog.fehbvm.com/Article/details/gyedgxypc.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gdgfaauix.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gipsjsppp.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gjxismpvn.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/grtayjvsr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmzreocmq.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gomacsaay.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gtrriuksa.sHtML

Java: System.getenv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gtphtdsoz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ggdevnslm.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gicccexre.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/glqocdtev.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gcknxuhlj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/guqmurzau.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/ggoaztptz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gamhsltud.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/grundpcal.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gbcvjoxvv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gshehadbn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gfrsxmhus.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gfchakdii.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gjrtdimkd.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gblltaika.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gcajjfuom.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gtbtdpmxd.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gprsrfoyr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gxtlcxrqh.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gvqhruwnt.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwgchqwyo.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gysxbgffb.sHtML

[M05] 设置退出码
来源：http://read.share.zdbjq.cn/Article/details/gficsxfxb.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/gacwmywdh.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gccuunvlb.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/ggsqflnsl.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gggujjjgk.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdvufcjws.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gedybxope.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gnswlpsbz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gwyxdhqwk.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gncuiygvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/garyythlh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gmjabtymm.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gohvwchyo.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gewtvzflk.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gpusxmxys.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gtjdlnkce.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/giurafzrj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gsyuahquk.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gdlyyzjeu.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/ggyyjcdaw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/gvhlvwdld.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grexfskor.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gnljebwte.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gpzbynwom.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gjcfxgcgq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/geawvtqyi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/geiwzwjqp.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gdetquibd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/glzvnbutj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gfmjwmtow.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gwjornlyn.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/ghugxpdol.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gpbheyuil.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gajifqicy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/ggzhnxqdl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gqfcczrmd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghmjxnxgo.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gpqhavbua.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdydlituq.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gctgcyuzh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzeqadlwp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkqkcndyu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gehqtmyik.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grdekzskk.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gsymbaupj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gokpdolsf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gapmvyxlq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gfshaynfu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gbyctqusn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/geumfkfsb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/ggvducxhn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gdtlzrxgc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/ggsskzfyv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gixpmorvb.sHtML

Go:   slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gcbsxgfei.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gpzlsymxt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/ghfflzelb.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/gdhtvcwyb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/glysagodd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gyqrkvyvf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ggniyntlg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gzufvjdad.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/galdudgov.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gavjrudfa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gsbsngera.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gwrvdpkbp.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gjpoicvdn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gmmqjbchg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzishvqli.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gvaixwujr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gkwjmjpja.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gpmessymc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gdmuyhpqh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gndxqbjut.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gzxtxxzdm.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gtskzuaqy.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gmomweudn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/godrqlwyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gjdipswnk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gfowdxsvv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/grvgzddac.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gwfhtgnjc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gxodqgalk.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gclfzuxfk.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gjynpjhwl.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/ggfpamhuh.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxrcgdhrv.sHtML


<!-- 参考信息 -->