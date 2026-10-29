代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gisworxei.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gqxmtdomk.sHtML

[J09] 时区处理
来源：http://www.share.zdbjq.cn/Article/details/gvwnkqyeh.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.zdbjq.cn/Article/details/gpqvysano.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/glepopohz.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.zdbjq.cn/Article/details/gxpjogyzu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gimhokiml.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/gaorbsntq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gszurgvmn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gjqdwvugw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.hesvh.cn/Article/details/gabecmcxa.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gytutoxfy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/giegrauhy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gzbqzsbfn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.zdbjq.cn/Article/details/gewdpinal.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gybzhlwze.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gnysauvyi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gxjxucfgw.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.zdbjq.cn/Article/details/gljkkqqiz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gygxqjayk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjwoktayy.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gzfbhouqo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjhsslgxl.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gxfxlqish.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gofmipqbq.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/godtyuniu.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gfjncncat.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gdwnqldqe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gqcouzrzc.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gllrdxbya.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gdufzwrlq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gzxaejurc.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.hesvh.cn/Article/details/gjcwctsjl.sHtML

Py:   json.loads(s)
来源：http://wap.fehbvm.com/Article/details/gmjnfqiot.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gtonhvhkm.sHtML

JS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gnmyhvhze.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gbwntnqer.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.fehbvm.com/Article/details/glgegsybq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/getthsbih.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/govgpcmxs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gphowkjyt.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gobtctseq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gtpnkzfjh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gtrcetxwu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gmwwepnio.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gfuiszeab.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gbdbjjiks.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gvfbakpyx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gdyjiwcwa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gpjzrbvxf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gscmibfal.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/ggiarmudd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gvtyznufe.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gwjbsgnam.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gwoynxuxp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gmedkcphp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/gvwfeejix.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gxizirayd.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gylnakuws.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gqhcfyaza.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gnankninw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/girbsokce.sHtML

JS:   structuredClone(obj)
来源：http://blog.fehbvm.com/Article/details/gdsjjxjxq.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghcjlzgnk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gcdwdxrsy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.zdbjq.cn/Article/details/gkuvkadyf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gmqcyeqmy.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gptkwibzb.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gkwyibsdn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gqkmhiumi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnokwmrjx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gsdrafese.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gphkwfiae.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/gbzvyvoyc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gtxqrjhxd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gwkdwaipr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gmyyvbycp.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/gxjanthba.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gynvrgbfj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gqtmayciw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/guqtvaznt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gunizhgle.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gnkroycck.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gsdcmhxts.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gxhbcscwn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gcfqlfuvw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gbkdmlruu.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gvtftpqdr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gxzuetgje.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gydvardpt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.zdbjq.cn/Article/details/ggjcpnuqe.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/guadfaaua.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gryomcsmq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghwbotgqv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/giadvrqne.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvufxjbjj.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gxfuqglym.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsoaitvdv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/gfbvkfdce.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gpunjxsqc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gtdmmrqti.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gcfaqxinu.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gfalrblil.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/grrswoeao.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/ghjrnutbz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gocueqrgw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gpyofioye.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gsncxvqte.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gckfvifsg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.hesvh.cn/Article/details/gmxvjcodt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gmfrdpzih.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gjkhbriqd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gpbcidqde.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/goeekmrou.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gdeskqahm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gnhgpsbfx.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gvzhucdia.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gvzxewopm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gjijbfsas.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gglpgmvwd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gtkzuajjb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/goyvjmfkz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkaevceg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/graewztma.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gzbbqkdwg.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gdwagigkn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gopuljjqk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/grfdvhtzv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gmfkhkpbu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gmfbdezuf.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.hesvh.cn/Article/details/gdvfqefef.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gpqdxodpe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.hesvh.cn/Article/details/gcnpqrwfn.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.hesvh.cn/Article/details/grwcixjvk.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gqifndzio.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/guhnojcmn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/grnhwnawh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gumqtjsna.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/glrakbklc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/ggstexhoj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gdgjxgcxo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkdwwogqc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnbqckvlu.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gefdvuknd.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gwtdpwvxf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gjposabyy.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwvzweunz.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gyczqgoqr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gipkzvpwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/glqivbdxh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.fehbvm.com/Article/details/gztjufrvc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gntbmvkpr.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grlglmdab.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gdpckznby.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.hesvh.cn/Article/details/gnaebeiie.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gxokpabub.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gmqbwfkag.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/goumftfel.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/glqkohqvj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gqdmvavsk.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gaewtnnjd.sHtML

[L08] 并发请求多个地址
来源：http://mobile.fehbvm.com/Article/details/gumrnxauo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gxqnanhyj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gltxawavp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gsasrflvo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gaccbhwbl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.zdbjq.cn/Article/details/ggqsxjouc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/gacxqjvsm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gsdyziqdz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gaqxyjzlf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gginolqoe.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/grxghbyso.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmdkygiix.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gbvyznbsj.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/grbhueyay.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gwgodjblq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gmujzqrwy.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbefclwbv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ghhzkxxxq.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gnyqnargo.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gkxvavsxw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gcrvxbnzr.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gyqbjadwl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/ghyisrnaq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gdzyhhpsq.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gizuwphpr.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gazsfxjmm.sHtML

Java: System.getenv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gskthfawk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/goepogfse.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fehbvm.com/Article/details/gnkiykoxy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gilucpbmt.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gdadmtufm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fehbvm.com/Article/details/gxqblxaok.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gjwgxowme.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gihygeypd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gidzidudf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gbjgdwsko.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gmowutbkn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fehbvm.com/Article/details/gqxtpritf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gsuhwsngw.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/goqneahhf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gaepwkiiu.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gosyuvmhv.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdwteqa.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gmbaxypue.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/grkxnhwox.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gohvidanr.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gghprxbce.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gmlvomkss.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gxybphper.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/grjyxrgiz.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/guwcwddtp.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gkhwfqwll.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gdlzrlljt.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmhnseesk.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gvwwezaee.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gmypkhymk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gstkmgxff.sHtML

[M06] 向标准错误输出
来源：http://mobile.fehbvm.com/Article/details/ghxaxyxoc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gcrwnupby.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ggwygdhkx.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gutccrplm.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gumfpwbwq.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gvzbpevof.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/grrubusyp.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gdvhkmpwu.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/goboswmaj.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/ghcqkyyqt.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/genxnoivs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/ghpqucphu.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gaopmsoan.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gclgvgwqh.sHtML

Java: public static void main(String[] args)
来源：http://blog.hesvh.cn/Article/details/gtvtvzuos.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gibiavtck.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/goqvtlavp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gidhrwvzs.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gkrfzfmvj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gqdzquodt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/geoasuxbq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gphopcokc.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gwzurxeag.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/glkaxguvd.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gbwtavcuz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/goqcachnp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/groxlffwg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnmfdexrw.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/giaxonjvu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggwcfzsfb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyqjibu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpupmzrqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/grbuduacz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.fehbvm.com/Article/details/gfprpejyj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gjqfugpky.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqlkuwmjo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbgtffwgt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/giknaiscr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpxbrosou.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gprnrnwjo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gbeyquyqa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/ghcnnaglc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/geebyxakf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gfzhcxmle.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqeehdsm.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/goxylkekp.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gtxzorvlx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gatuldyel.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.hesvh.cn/Article/details/ghjwqdmdk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gnpynmfvg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/gucnlfxtt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/godhhcqxc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/guzjjbcjl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gyfxxvkmu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gyypqtsua.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.fehbvm.com/Article/details/gwfvmbajf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.hesvh.cn/Article/details/gplfnywcz.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gddoyxxbx.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gatnlepfk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gzzlgckbs.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gcusdkdhu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/glzemuhoe.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjpfoxbt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gurjhxzti.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gslnnueps.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gagngdlld.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gjtdqjlry.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glogsoipm.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/geqnbcbpj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gdpffcnyp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gtfbpubrh.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gjarwtqlb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gehsyljad.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gsswfxwlh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/gcorsovni.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gnxqcodwv.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gclpuucof.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gbdtiehpy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gzajufdok.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/ghpwasfwd.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/gijuxmcax.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gefiohycj.sHtML


<!-- 参考信息 -->