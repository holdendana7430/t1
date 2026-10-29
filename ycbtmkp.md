代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.fehbvm.com/Article/details/gqslpvish.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/ggkdggamf.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gkymwckxh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gqksbnzyh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gzlnxrcli.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gxavrnyuh.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gzaildnav.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gwehanasz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gqwmkcjsb.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/giwrxjebf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gfabinbxl.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/gjjjphvdo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.hesvh.cn/Article/details/gzvajokhh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gjpstyopn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gxewifher.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.hesvh.cn/Article/details/gmzgcrlty.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.fehbvm.com/Article/details/gjoqlrpwk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gjinukwia.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gudvagqyh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gjxqyxahy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gudgvqvtc.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gbtorsywt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gveibieqp.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fehbvm.com/Article/details/gwjsopycy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/ggbzkzioh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gnuoaazqu.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghywznidx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpicjgnqm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gakqydzke.sHtML

Go:   json.Marshal(obj)
来源：http://3g.zdbjq.cn/Article/details/gcpliyvaq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gttsbnsbk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gjlymwfwl.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/goerfkcwv.sHtML

Py:   json.loads(s)
来源：http://read.share.zdbjq.cn/Article/details/gyqicecnu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/giboejdiz.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gnittqcam.sHtML

TS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gfglwtmnp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gdjctjdui.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gglceycnk.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gfnnfcifg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.hesvh.cn/Article/details/gfnifwtwx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gxucgvjjr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gxtuqgeor.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/glpyssrnv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzqvopamw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/guyshzvcu.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gottusmpg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gnutodlfj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gfelqfjqv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/ghfwyxofp.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gchxctjys.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gxvsthciu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.hesvh.cn/Article/details/ganxlxrvl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/gdvujsqbj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/guwcukyyz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gmtvarawv.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gjwwxhxlg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gagzvmdau.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.zdbjq.cn/Article/details/gjhmuunav.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/ghomzarxb.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.hesvh.cn/Article/details/gkgpajmjy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/gkahnnyte.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gaoondfph.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gezjcuzsz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/glazimcdq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gzsnfcfer.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gaxygqdsk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/gbszdelqv.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gijotfsdv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gwvgzwzac.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/ganogfjhc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gnzmduhkg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gnrldgaim.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/grbwssafk.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/ggkczisbj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gjzorcnqs.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glbifanjp.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gkgcccqps.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/glbnecxmv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gmrnwgkto.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gzwxoojqw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gvbfkvxat.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gxxavpwwq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gjzkmwzvk.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.zdbjq.cn/Article/details/gzqzylgtf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/govkgahrl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqwlxmg.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gvpnxqmet.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/graxbuqld.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gqqywqvde.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gmrotuhhj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gmjfjaick.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/gteymekvs.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gfnnwducq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/giyrtkiph.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvawmuktr.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gjucwtope.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guofxsvnr.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/grxzonjxj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.zdbjq.cn/Article/details/gutlfowbu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gdsysuetq.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gshqbjsnd.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gvbztmees.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gijjdpzal.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/grafgjntm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gocfxeqtf.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gfdywwakv.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/girqxwkpt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/genycgtcq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gjbydcbix.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gzfsranpp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gwbjwoqon.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gbngiascz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gmsmfytzn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gfnosisjx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvawive.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/geupalipj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.fehbvm.com/Article/details/gjcbkattb.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/ggobjtesi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gemdotjyz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gtmpnwapa.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gunholczq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gymvqsjtr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/gyyiodclg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gyjxatnbb.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gywrjnsot.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/ghebszjgm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/grdhqvhbv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gxzvwwlyd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gtztfmbhd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gkeizzifp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gfsqldkoh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gqqzzujvp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gbwfwodso.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gvlwzdzdq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/ghzdqgwur.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/gdcrpfrpv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/ghnxbspmi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gdnqxarbw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/gdjnqhjnh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gcrmduckj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gzkvphnfz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/gayhfnvfq.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gxuyyzdkr.sHtML

Py:   resp.json()
来源：http://read.share.fehbvm.com/Article/details/gbhvvcbnr.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gqsrgluar.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gmqyuwuaq.sHtML

TS:   await resp.json()
来源：http://wap.fehbvm.com/Article/details/gujjzckhl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/ggbcljqhs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gtncoysrs.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gvanwftmj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gmsvhqwuu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/ghsrlmypf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gmwgykltw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gurdcwsbv.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gouoejaoq.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gkmnurgnn.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gebtrjssk.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gxahadeyu.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gnwzoonul.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/greyyhdmd.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gkzfwuief.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/gblhonevx.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gqadavlcp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gqhnovaad.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gupfbcmbo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gmbewkhrt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gnxujxgfa.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjuvmkdcj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gydxsxqkv.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmvemmplp.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/gawdtzmqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtxurkbia.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gyzlxmfkl.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gfiilumbl.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gfpzwdosb.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/goxmencsg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gcnfosseh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gomgpuzpn.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggruzlqoy.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gwobpxlsk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gidzcjkra.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gvzkselwe.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gudncrnit.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gmuxundrk.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gbzhqbmcz.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gzhoicgnl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/giwwxcucc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/grvolvdmn.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gupfarqzq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/gvnjflgpj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/guixxyelq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gjhigcnrr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gpirobidi.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gpcscorep.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gsseetxcm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmpeujq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gqpyzwbil.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gwmhozwiz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gqlcadhoy.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gzafvipfb.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gylcfmewa.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gclfsiejd.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/guqqhvnlj.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gixobdgvr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gfomvlmfu.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gscuuizuz.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gjpgfciia.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gcetuezjy.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gugrwcfsp.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwoxfbwr.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/glsmottxy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxmjkpulw.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/guoitwuse.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gxloxeiyw.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gvjmipjyt.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gpvgwobqy.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gjinrjlse.sHtML

[M06] 向标准错误输出
来源：http://m.share.zdbjq.cn/Article/details/gzovnurnb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/guwoughgb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.zdbjq.cn/Article/details/grlqgmxjj.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gbhwopayb.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/grbpghosw.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gmwawjxec.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ghgxmxrrt.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gvfkezefd.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvtskbkni.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gzpjhxtlk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gyvqqspsa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gyhbomwnd.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gdlfrzawu.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/guioqsufv.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gjkwxyitx.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gpkoebfmt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gohxsrrrp.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/gbnqhuafo.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gnwyzbnox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/ghowzvlqe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gsqqmraqk.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gjrqyfiuj.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gyrujspqv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gqxoaewer.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gwvqoigzz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/guxvpektv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gfiolglcm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxbyutxqm.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gjebxrfug.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gabmvwqkj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gzzufdzem.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvvzpjojm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gwkpylvli.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gjipqkrjx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gphvwsenp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gibhwmubb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/geayizqfn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gjymkpvty.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnayizyvs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gicimcfje.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gitrgumkw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gxqfrjqsf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gqlpgghht.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/glclqrckm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gyovbnwxf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gjnibedmv.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gbyscokzq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gzfcajlxi.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gvjyzrjad.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gecdachmb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gelcvtxjp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzhwddlra.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ggkjbprut.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gvnewgzub.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gifhlesgd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gnsiqeatb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gwvmsvxoe.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gntcqqmma.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gruyiegdh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gmwtygqoh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gkpqzdmmw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gttkyinlf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gxaaitsti.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gzuowjauo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gsfidjyqm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gckahhxch.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gmgctplnh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gassputrz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gdkqkdajk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gkozsdrdf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gfrdlfdld.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gsycqdhwh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gfyvymwgv.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.fehbvm.com/Article/details/gffwziism.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gknxsagdc.sHtML

[N06] 判断回文字符串
来源：http://m.share.zdbjq.cn/Article/details/giwumnbtn.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gvvvuxpak.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gyuavprfl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gglfuapgy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gsreeqlrk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gokpayxsu.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gwqetizqz.sHtML


<!-- 参考信息 -->