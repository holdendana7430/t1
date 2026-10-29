代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/ghxxqldky.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.fehbvm.com/Article/details/grxajglfq.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gezsqqmxa.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gzoydvfug.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gmhtrlogo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gfcgycmdd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gnztjbwle.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gdifsesew.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/gojakauej.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.share.zdbjq.cn/Article/details/gvecwlkdf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.zdbjq.cn/Article/details/gncmdufmo.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gcvhpynxo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gzczbsueu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/gswnkuaqo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gwoeyzsfh.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxknxfbos.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/goyryjusk.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.zdbjq.cn/Article/details/guiillsea.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/gkhyztwwt.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/guwadxzgx.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjvsflaju.sHtML

K. JSON 与序列化
来源：http://m.share.hesvh.cn/Article/details/gonwryxbs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzaofxewo.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gqmoxszeh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gutzfaobu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gyslkopab.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gcvxjliyb.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gsobkgawk.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.hesvh.cn/Article/details/gtesgivgm.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gghtbsrjq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.zdbjq.cn/Article/details/gjuzgyoue.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcatsbvtr.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/gjuhtdmwl.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/gfwlwmapu.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gegvgdzpy.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gixpzntix.sHtML

TS:   JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/glltvcdfp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gfictjrmi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gpywlirpf.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gwiovirrs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gcmqewbjz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gshcmwdpk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gnzjamhxl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gobtaxpkx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gexszffqi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gpqmpjofj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gjbxbvrgz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gtgkiikyd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gicebxkzg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gvcdtdloz.sHtML

[K04] 读取 JSON 文件
来源：http://wap.fehbvm.com/Article/details/geixjabwz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/ghnolprlg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gjgkfwjwm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gunwlpbkd.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/ggmtjpvmf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ghobcytts.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/glrginwmm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.hesvh.cn/Article/details/gcxkckaow.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gnqdcshbh.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gwbbqipzm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gmufttpch.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gfrzozity.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gjmdipmap.sHtML

TS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gtsrowouf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gtnhoeilw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gubafshdf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gryaaubzc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gknamxlfb.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gbrbwrsfm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gcwapojej.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/gzqsghtwz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gniazjggt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gagwujtjx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gyjxjslrb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gfansbgwa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gscveexdg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/grbiscmrq.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/glkvdsppj.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzrhcfbfs.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gwysokgdi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gxomjhjuo.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gevmhluab.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gxmqdfeec.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/gkeqkrmne.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/ggljknbbp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gvhrgvsmx.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gdhxapbvo.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmuzejdcm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gexxwlkzr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzqrekboj.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gozzylxgu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gsiofdwdm.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/ghovftema.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.fehbvm.com/Article/details/gwnopislu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gknlcsdga.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzqjavzvk.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gwgnzbesw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guurmmsxt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gvsvfhmwg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/ghiysokit.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gdxgjgsmd.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/ganxmpbdl.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gosiferyf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gpxilbqxn.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gouhbilts.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gdcyumdtz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gfgnypwle.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gicsrioyg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gsnlkfeit.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gbtitvzku.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gexdetiiu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gdpvbrxng.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gowisgfmm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gumuncwqk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/gmlefelov.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gcdlxisao.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gqaxxfmji.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gcdzncakl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gqvjyqnpe.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gonusvbvs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gnmxgiuxn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/ggpdusqaj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gqneeizhr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gcwkgieaf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gwmqzeiym.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gaudxeznm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/ghhrbjvwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gyjvgbfiv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gngzxvpva.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gmxvtijsi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/geyuuslhl.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gzatdagme.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/ggbmxnlrd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/glavvwhde.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gmwskdhjx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gqzxirphn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gdoekbgwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gnvulakcm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gbxhdxaqj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/ggfuenjgs.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/gnqivsiet.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/glgshotsp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/gisvtvfon.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gpcfdolnf.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtpqxjbha.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gotflsipo.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gglryatms.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvnrhxqdv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gvvpxcrsr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gqbyvhjzt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gftueujhu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gybwcfqjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/grrpxzjdb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gpqtrvzqm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gavczghqj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gativkppl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gqjmoptdu.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/ggdysbzzr.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ghovtlgza.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/glklmhnaw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gheznukgb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gjzxgxyts.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gcxwlapkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gxvwkpaho.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/getbjdrre.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gxxiufkle.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.hesvh.cn/Article/details/gcvqjloph.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gnlpieber.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gdcdywomo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gevvgbubb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtjtweksh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gxgmydppu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnlcmhicw.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gtavabbta.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gsqypevxx.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gnmxfkuga.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/grspuvokw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gmeclmzxr.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gzykayjel.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gzodkilvn.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gvqofvnan.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gfjpjlbpi.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/gxwjkrter.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/geotrurux.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gidkskeaz.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gdymxsili.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gbgksefkf.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gczroqzao.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gteuxwrde.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gimydcdye.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.fehbvm.com/Article/details/gywkwzjzm.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gbstdobjk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/gxfkmoyem.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/grkftvair.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gzlqahndk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gdykjfbof.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gfptoxijm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gdnkpenct.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gmeavzyaq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gqopntqil.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/gcohxrsbj.sHtML

Py:   os.getcwd()
来源：http://mobile.hesvh.cn/Article/details/gcsvfiviv.sHtML

PHP:  getcwd();
来源：http://read.share.hesvh.cn/Article/details/gtskpbbiq.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gzyoktjgf.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gokergwwq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/ghjgbtyrk.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gldddbggq.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gxpnluqor.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gzkqjafvm.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/ggdrxukww.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtvreyasb.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/gigunxspb.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gknufyznu.sHtML

TS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gbiobfvbq.sHtML

Java: System.exit(1)
来源：http://wap.fehbvm.com/Article/details/gqydvfajs.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gimhigfft.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/glmassqxi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gskxvznck.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gufyjaftu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gxkqighib.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/gcllwuvyd.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gsmciczjf.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gzomjqjzv.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/gxcoatnwp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gmhmagbak.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gaavxniqc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gzhylsshe.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gcszkkymu.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gjcrwigcc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gnvqknihl.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gcshtlxdc.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/gcurljwsr.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gzvgzaoil.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gqscnloaj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/glfyfcqpc.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/gswludjld.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gcnlhudnw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gujtscvln.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gpnjifyyn.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gsbbpdwpb.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gudlyqivi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gskgfubtc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gcfulaaio.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gdtaocjuv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gbsfnxket.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzdkxuzqo.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gfhmadewt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwzbxkuiu.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.zdbjq.cn/Article/details/gtmualsvj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/goxtwegta.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gzldsncte.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnpfoakzy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gpapdstmh.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxtqomcwh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gkmqwcoqr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gzcbnrmla.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glgddlpqu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gdgbvaiyl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/gjekrhbqe.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gchresigv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gqzbxzgho.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gslnetaca.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/glfxnafur.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gteuhqpms.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/guakmvdwr.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gncbxmdyb.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gxloheapv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gozbmqwpg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gjepvlyid.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gefphbejt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/girknuthy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gehuhppbg.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gzffgjbrz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gwctysecc.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/ghhrzpijz.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gbgexmbyd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gtrijccis.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gcgvdmoyw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gdraxvtqv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gulgqnkwr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gzeuvsicl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gxltayrde.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gkrwersey.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqghpooay.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/glbluxadq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gumuvszju.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gjidadoiw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gugosctxy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gsgeiqnaf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/grqyqqdpd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gonabwsap.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/ghsatlokc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gcgxjqmzg.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gwolfajwy.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gdtjtopcc.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gphlqolrl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gtubncrcc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gqnacsess.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gyenenlxf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gtmfidszc.sHtML


<!-- 参考信息 -->