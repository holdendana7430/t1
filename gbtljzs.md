代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gbeslwpmi.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://m.share.zdbjq.cn/Article/details/gwtgbrsxo.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/getcdaumj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/glrzpqlnk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/glmfnvurw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.zdbjq.cn/Article/details/gydermoxn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gqndnhbwh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gerenqkcd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/gdfgogvrh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gngkmchli.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gxjrajrsm.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.hesvh.cn/Article/details/gqqylapbw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.fehbvm.com/Article/details/gbwdxkaqu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gqtmkcjba.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gtgdhgiba.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gghihdshz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqruogftn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gxldrflsm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.hesvh.cn/Article/details/glkcufdpm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.zdbjq.cn/Article/details/gvdmyzdid.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxtenaxqm.sHtML

K. JSON 与序列化
来源：http://read.share.zdbjq.cn/Article/details/guckvfbdt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gmotruhrj.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/gmrfbvgnb.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/glvqqwsxr.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gckdqrkho.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gabnzsuyd.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/guwwuunfq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gakpqzuvr.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/glpbpukwc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/givfftfns.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/galjojvoc.sHtML

[K02] JSON 字符串转对象
来源：http://m.share.hesvh.cn/Article/details/gtnputeoh.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwnmsgrrn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/ggbekiglc.sHtML

JS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gjqvyhsjv.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gasgoumkp.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/glwzecptq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gaxgoagfx.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gtlwpddrx.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gmdlfoicf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.zdbjq.cn/Article/details/gqmgmxdyq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gnwfqnalb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gnwkergvt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gqedcyqbn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gikdwjejd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbuuiomie.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gceljcenu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/goteqaabb.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gibtcxnxb.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.zdbjq.cn/Article/details/ganrmtzas.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/gfzyfcamv.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/gslmzlxyy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/grucotggk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gzwtptkdk.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.zdbjq.cn/Article/details/ghzzhphob.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gnbuvjpau.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gixpncvko.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gqcqmsuit.sHtML

[K05] 深拷贝对象
来源：http://read.share.fehbvm.com/Article/details/gwcmxeulz.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/grqboibkh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gidymfctk.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gwtntvxkl.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gjzdgpvyw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/gkelifeyt.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gtszwqfsy.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gtpmgbxhh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gzsrjhtgm.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gpwkffbnp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gsndwkjyd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gfecfgdwp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gwlasglap.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gslropiwt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gmcwrssmp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwwqmpo.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/grgiiiasu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gxmpcddsf.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gkwxgoydh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gbzirhxrn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gcsllsntb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggtvwqyya.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gdagihldi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gkylolrec.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gmiouhptu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gdttfnqyd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gsbhfmpfd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gntgszdfv.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gnnvjgprs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gbayxgyxx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gvnsdgbdd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gujhpqmfs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gebepthli.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gcehxykbg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghmcknwui.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gbubviswx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gompempkp.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gznaglqvx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gomlczrgv.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/grokhghef.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gwfhwxwai.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gnoklnyfh.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/giywcnshv.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gioqzmmht.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/grebqhtjt.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/godaojccx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/grhpsbmaz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/ghgnpmndp.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gksukxvtd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gemgoebbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gdgdmsjvb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gsjchbhtb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gkphoudbm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gvkpnczak.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/gtoqsmtqk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gcyzotvio.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gytotnxec.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/givyivpcn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gquhmsuzu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.zdbjq.cn/Article/details/gptapfuta.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gwacllwgm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gwqltfrbk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gvkwxdiuw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/ggikaywcg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gthamercu.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gfijpitzi.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gtutfopzm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gjsycfgwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gouixmttk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gcpobokga.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gkepgsnop.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gpomwihki.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gxyfwykfi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/glyjjfzoh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/ghceewedy.sHtML

[L05] 上传文件（multipart）
来源：http://3g.fehbvm.com/Article/details/gcnhowyzv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/grrscdgdd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ggscxeofe.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/geoodogyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/glewostju.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gfushqeir.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzjtzrc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gaabprtjs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnwzvqrhk.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/givvylgsd.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gzwvtcyty.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gtrbqsmuc.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gusgrbroy.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gpccaltlc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gspdvifnk.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gjkmihijr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/guzubahhj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gshrhlshp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gpqzecgib.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gfyxkllun.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gelpligts.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ghnngjmyl.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/garbcmrnc.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gklalwnhf.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gelgtwryu.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gdyymcwoy.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gqbmnsluz.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gkizywsyw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gxqofrmgj.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gxvyeaxtv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gmdisuakz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gnlasctti.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gpbhjkosf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gtapalksf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gqligdpky.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gohoeclya.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gekwomgxm.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gkfkwaikc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjuqvmpns.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gpogvxhha.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gkbhiacof.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gfxdqwfbj.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnamhblte.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gbcffcbam.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gttuywntv.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gduobggke.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/grcgzcxyu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxkntnscb.sHtML

[M02] 读取环境变量
来源：http://read.share.fehbvm.com/Article/details/gvjdlwozh.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gchvmdeyk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gbnptvkae.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gvmjaatcb.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/ghvhfbpaz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmhvpoxg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gfftxomzf.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gqordbbll.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/ggmmgqexk.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/ghjzmdgek.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gmthobbfy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gutfmtrvw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gnglvrzwt.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gymhkuoto.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/ggjbdbszl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gnsweansq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/grnmrdjew.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gwrupsamt.sHtML

[M04] 获取当前工作目录
来源：http://blog.zdbjq.cn/Article/details/gwqgrvaaq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/grczzfbon.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gzvpustih.sHtML

JS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/ggikfrqxw.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gertgyicr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gbqnoqqtc.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gymjoqltz.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gcermfnan.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwngzcpi.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gomrnzgdx.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gplsaansf.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gyfuaqiul.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gtfarrnul.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggeuzddko.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggnthlmke.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gnvplqrjm.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gwafownmz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.fehbvm.com/Article/details/gycjxclkj.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gjxxlvlpd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gacygoqii.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gybfsmnvc.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gudlnnbpv.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gzdaqnfka.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gxdzuhvue.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/geaugidno.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gikvvpjqo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gsoeenxya.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gyjmglozk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gexixthri.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gowtjldbg.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gcynghiqx.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gfayvxltk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gylvepith.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gfwtwtshe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/ggttckuxy.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.zdbjq.cn/Article/details/gcrlwpswg.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gifvukuhy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/grdlvyxbf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwolxquhr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/glnhfhigi.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gjdvcyziy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gqglhjsez.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gkfcnthij.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gelclsfus.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gjijixopj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggfonlzrv.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gxwerqimz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjanhzmer.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gmnpcqkzc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxvckhynn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/ghxjjsnpr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/glnrzzzej.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gvxrflhwm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gitsyliev.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gupcojrvr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gkdbombjn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggugnztzs.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gyynfzfkz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gvqbbkvgp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.fehbvm.com/Article/details/gqqmpgyrq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gtkomzeba.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gzooygtab.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/gqvzsacqj.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gwgvbnean.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glzfnucfd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fehbvm.com/Article/details/gjjusnuzz.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gxagocqym.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gfdqyycqg.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gpprldzsx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gzjkffmhv.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gpsmzhjer.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gvgnrsaeq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gclbffzew.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gyqcattxf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/guvbcptjk.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gvzeamike.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gxqznmzen.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gpqgsyihi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gscnzprzn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gusyjzgsm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gfrwyfxem.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gduxkbyqy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/ggxjwizez.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gmrvljgtl.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gvottynug.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/ggnkymrds.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpxbobstx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gnclyoqrb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gypoulavp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gyiywhdfd.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdhwqsing.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gjmsghule.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gbkyblxpz.sHtML

[N06] 判断回文字符串
来源：http://baike.hesvh.cn/Article/details/gootsquje.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmwfaadav.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gvxrgggms.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghrmbabus.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gunwwgzvw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/goohxwnol.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmknryylq.sHtML


<!-- 参考信息 -->