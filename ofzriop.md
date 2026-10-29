代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gkwnehsxn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.hesvh.cn/Article/details/gfbnrfdfd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gzemmnxoa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.fehbvm.com/Article/details/ggvaxbpnl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.zdbjq.cn/Article/details/gxjbalqxz.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gkefsqbcm.sHtML

[J09] 时区处理
来源：http://www.blog.hesvh.cn/Article/details/gwsadhxnn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.fehbvm.com/Article/details/gxysremqg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gaabibbvx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gsovnhoti.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gqctbabak.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gwwehuezs.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.zdbjq.cn/Article/details/gzfvgpkby.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gfnnsgzbh.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.fehbvm.com/Article/details/gvbmqltlr.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/glvtsbuyo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/ghjrehsoe.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gclvmqauh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.fehbvm.com/Article/details/gbxqqxkao.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gbnyrquvb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyibrgqss.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/gdjutzpns.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/gksityuah.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gqsfqfyon.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gdwewqtsi.sHtML

K. JSON 与序列化
来源：http://blog.fehbvm.com/Article/details/gskelqaqh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasaezgwq.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gnhnuwihc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/gwfwnnozn.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.fehbvm.com/Article/details/grvaqinbd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gcsvhpokz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gaielsbxd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gjnoycigg.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gimduloqr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gvhiwgnxj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gehfdyjrk.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gavnknubj.sHtML

Py:   json.loads(s)
来源：http://m.share.zdbjq.cn/Article/details/gbbwismhx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.fehbvm.com/Article/details/gugoqamlk.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ghzflovpw.sHtML

TS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gbfgotxwl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gkeierhdi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/ghwrppiyt.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/glhneghvi.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gltkaisgy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.fehbvm.com/Article/details/gzefedvsi.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gekirvain.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/ggkrmdsiy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gamavyvix.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gnqbixyze.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/grbprzzkf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.fehbvm.com/Article/details/gaoxwvlud.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gvsptgnbr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.hesvh.cn/Article/details/gmcgwxzxs.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gkrncswuv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.fehbvm.com/Article/details/gwajvener.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gwfcsmlzz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/glslfqfuk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gertuyjyp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gqtpdwisq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gfdfwhszi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gaydvvrcm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.zdbjq.cn/Article/details/gwphgtcaw.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gupkwzxpf.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gegzsvuac.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/gcgppjcnb.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzdepxaoo.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gbcoeyokk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/ghsppfzbk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gbahacigf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gmtzengjh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gtzhvroyy.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gzkkhhhgs.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gvyssiyev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gfaqaynwj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gudagliol.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gdhbjnowi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/geebvlmhg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gvukevwpu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcsrsnumg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/giziywrpr.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gsohkuzrg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbfxmwedo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gjhjxeffv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gzgbspruf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ghlkmyfmd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gxpcfmxjo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gswksxefh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gvnwdtwir.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gquwbbarw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gkjgsltrz.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gfemidabf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gaovbwcpp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gxpzbxcbe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/geffzgvlc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gxyinwxej.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gvpsbwmlh.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gupwwwclc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gjfajbmlb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grfusfdhh.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gvkibzlel.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkidjfgpu.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gkzuixegb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/gfzhvyxfg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gkeydyham.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gncsalsab.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/glcuhvoqy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gkzajqfot.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gjtyefymz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/glnqjodzf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gomhrussz.sHtML

[L02] 发送 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gzbebyaoh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gzihaoqtc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gnnnlghyw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gkiteotpa.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gkgyxcqso.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/girsfrgvh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gahtfqjwx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gvivmaqhx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/genqhhkpb.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gczrilalf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gexejxmmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gtxfgwmzf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gwotwapnc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/giywewbcl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gydyilomv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gkqaajtmu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gmovcvtne.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gozphinep.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gaacmttaj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gkcbryncv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gpwpiagxy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gaedlhcig.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gilcbjlht.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.zdbjq.cn/Article/details/grplipvwa.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gpytszhfr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/ggaxtmeov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gpjrgqogz.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gutgoknnu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/goamcxbmb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnbzidby.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gzookjhul.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gbdqcmfld.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gygvsoenl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/glufyygsw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gueuavqdn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/ghibtyevc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcbjzrfqe.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/glnkowiao.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/guconrzin.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gssrjdavz.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gsomrdjxl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/grgpkcbfb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gftkzwhbm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gmyydbemk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gdcdvqqeh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gbxubzsxt.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/ghmuuitwx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gaskarqei.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gxegpnbhd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gixghlqgy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.hesvh.cn/Article/details/gzfwifhie.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gbixxpwlr.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gfclkqzfh.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gjdybaivl.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/glfmpjamm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gqukjflxi.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gcutintbs.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gxeyzfcnq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gyczsjvek.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/grrpklniq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gnsqgcpop.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/grkekynxx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gzlyjorii.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwkilaoxi.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gtmxasnmd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkovsilsv.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gvlegdqkh.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/ggwqagumn.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gygssdzjl.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gujetrziz.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gczpkijkw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gmyjnwxhu.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gcqamclkt.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/grxiyamzl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gftfcjxww.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gacyhmywn.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gwharpwqd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/govrpbakz.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gbrkzzvyy.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gcccbmanr.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gbqqcnsel.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gmjyxhzlx.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/grwcagrop.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gzozyeozb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gbbxwfrpk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gojaiskxj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gxzvielte.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gbjijbzux.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gzetrbcwn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gtbmgixfp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/ggbnekara.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gavphocfj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gfwbifmmr.sHtML

[M04] 获取当前工作目录
来源：http://3g.hesvh.cn/Article/details/getfgzvuw.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gvmawcgzq.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/ghewoyfqr.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/goiponcur.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gbqimtgso.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gbvxbdjgt.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gnbvjuwdx.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gskedqxcf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gjhmamxal.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/glgqajltq.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gsarghmwb.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/grseaxfzg.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grrijartw.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gubysfubn.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gkptqngts.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gquwwuopa.sHtML

Ruby: exit 1
来源：http://3g.hesvh.cn/Article/details/gpbagnppx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/gdlnjszvc.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/ghgxkobvu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.zdbjq.cn/Article/details/gwhedecgn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/ggldfgugl.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/ggzurrrhn.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gxrlediqn.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gpsxbpzbq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gjnotsylh.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gfvrkeuxf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gzzfyfegj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/ggpnhynwn.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gupexevns.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/grpihkyob.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/glofxfixg.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gezjfaoxj.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gwbfzvjxz.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gvcghlusz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.hesvh.cn/Article/details/gqivtiaty.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gadzefwyo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gclujprdx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gelpcejlv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gnkhdkamd.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gzzpurhmy.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gfrcavznw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gjewpjqci.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gsxaysswe.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.fehbvm.com/Article/details/gebxvwipv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gxoskgqto.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnqllxxdx.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gbzbhavku.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gurpamrjs.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gmxdyuzzq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gjoyuidxd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gwtdmfqvv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gktwxzqhv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwsusdjqt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gmfcsydbs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gznxjydyx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gqrgdbkus.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggvmmxwav.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gfqnenxxg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkbitbtag.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gzqfihxtr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gzbdsnzah.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/grwaakuwc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gumwfasrs.sHtML

Go:   slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gphpzicgz.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjfhhxkzr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gzbxxywkr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gxtouliwg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gepftutyy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gpwkfznck.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gntwedgqr.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gdzoquaqv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/geimidwnl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqihatgyo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gaqnvmgsi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gbirkdvna.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/ghdrcjxcu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gtzjttrob.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ggqdroayl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gqxkwakaf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghjchyhns.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gjqobdgqx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gduehuiow.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/gauitpjun.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gpdqqlmcj.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/gfzlreazv.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbdbhpmkh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gbrhvexhv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gnkpbgtom.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gvznioyyl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/ghehaerou.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gvjzjqdzn.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gflnjucfx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/glxmqnttg.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/ghjxsoulx.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ganweacww.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gsitwsjkp.sHtML


<!-- 参考信息 -->