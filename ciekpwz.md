代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gufmhulwu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gvmbwvjhy.sHtML

[J09] 时区处理
来源：http://3g.fehbvm.com/Article/details/gnkfijbrv.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.fehbvm.com/Article/details/gnekzwmnq.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gwshsbjyg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gshvdzbry.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/glctewcxg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gxgkxvcks.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gtrqvmkqh.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/glygzwlaq.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/giqwylbgo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.hesvh.cn/Article/details/glejnpiat.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fehbvm.com/Article/details/ghnpqnbmh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gaopoojpu.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gapbdjavq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gwmfsdgvi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/guerpgaqa.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gdeitiwxr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gqxyxxnzh.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gyoyuksnl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmzncnwnx.sHtML

K. JSON 与序列化
来源：http://3g.zdbjq.cn/Article/details/guvnsbnrl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbysbxnqr.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gxckwagac.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgzocwaz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gkprgztvc.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/ghpsnjnou.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gnycoxizm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gaisxayqa.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/glbqnafbj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gldisppet.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/grdvsgbaw.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/golarfjhe.sHtML

Py:   json.loads(s)
来源：http://www.share.zdbjq.cn/Article/details/gmodkpzvo.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.hesvh.cn/Article/details/gzwqgftyo.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gxufobhdc.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gktwzptrt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gjafodbbr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gcnwjsxtw.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gvjqsqmhz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gpjydqeqy.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/giuixmnpg.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gwhpqpuwh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gvsjzhpig.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gjpavlsak.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdvtcdhk.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/gvlmntsso.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gmyohhihk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.hesvh.cn/Article/details/gluxyaqso.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gurmmpyza.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gmyjztoak.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.hesvh.cn/Article/details/gycqpkuyj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gtuxqytkt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/genzghhvu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gycixvekb.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gwjfwjemy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gmnfrcsom.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gptmxasuj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/giasomayt.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/goarnizri.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gisdzvlqi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/geeboalea.sHtML

JS:   structuredClone(obj)
来源：http://wap.fehbvm.com/Article/details/gciukmpvh.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/guanannhd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gfmzizxhf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gslizilja.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gagezsazr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/giwfhowgb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.hesvh.cn/Article/details/glougfotr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gxuzamvhr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpjcocadt.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gtivaddbd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gaqkttcny.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/guiambipf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gigvbqdpv.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnahhqgkq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gvvsgjbfr.sHtML

[K07] 进制转换
来源：http://3g.hesvh.cn/Article/details/grhqepowa.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gonsyidpc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gdntijhjw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gfpyfvbvj.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcbbuyufp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtsrqthx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gfmawhema.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gfsuwhcaa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/grsfmskpo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/ggvmstjmg.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gqgvuxowx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/ggsleheac.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gvvihsadm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gxnierlbr.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gnzgreibv.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gqkxkxydb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gwzurxabb.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gnlrbamis.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggubdyccn.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gtuyagals.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggnuqjqdm.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gzpnhfyko.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gqybaiyan.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gtijwkoyd.sHtML

JS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/grrahmrnw.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/giiytxtwb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.zdbjq.cn/Article/details/gnkpkfcui.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gvenavsef.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gkzvvqdma.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gyxtuvsof.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/ghtimyfws.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/giuhheogy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/gbgkebhph.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gjzfaelez.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gyihuhojv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/grigerkqf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gjdggzwhz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gerfownnk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gralhcnia.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/geezupfke.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gydjholnh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gkpouomyk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/guoiguukw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gnimeqvhg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gfupkuzpo.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gkktczqzc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gxydydxge.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gabontebd.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/ggtkzsebr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gaklstpms.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gmpspxjse.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gmmnegjgz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpfmsdjvh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gcinbxgww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gqzymdqmr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gjfwncqpz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/grrflqoef.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gblsywgxx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gncghjmns.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gdzykhjzq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gudfbftww.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gmwfkcjxi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gpbgfkkme.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gncristoj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/gnrrzdchc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.hesvh.cn/Article/details/gszldeomq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gcmmwoing.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gqcrmfffo.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gvipmjkyq.sHtML

JS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gvjwunwgw.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/glxrqdmyg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/ghngdbtjw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gjvupwrjz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gxruxcudq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gvopmwurd.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gfbjvnzfi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gayiqnvco.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gsjhnqmll.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gsytdafou.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gviwtydpt.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gzyetysfs.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/guznlbxui.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gndrdegws.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gzrkrwerq.sHtML

[L08] 并发请求多个地址
来源：http://blog.hesvh.cn/Article/details/grplzoxzm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gnmajmssm.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gbycroycw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gipyfgecc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/goyzypecr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/gfxhjjojc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gjxetwmmv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/gzaimhilj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/grhcarsdt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcwftwmti.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gyvybexou.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwuvocgsh.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/ghfmptdzm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gorshyjpx.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gdjijzcir.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gysminntd.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gbhlfwjko.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/grsxqkmxa.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gbsgbjpds.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gojxmihxi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gbwpbxqsj.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/glohxixul.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gshvylbjw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gfhtegpcb.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gkclthvmp.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gscwdnqlk.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gfwoigyli.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gtknxjovi.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gvtbrbobh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gotnrktoz.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/geubwekry.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gykwqarfr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gfjhxpvle.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gltewckff.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gdctxbcmq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gykabcomn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gmnuzfqkp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/ggcwpqgjk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/gsvwjxhcx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gzznlshpu.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gxeklxdoc.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/glvqnozyb.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/goxwzapby.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gykaayqqy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gsujvedju.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gvwtuqnne.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/guvnsczai.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gnybqfcnz.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/guwbcdgyr.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gqohokvsl.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gtlzpshhh.sHtML

JS:   process.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gwmchygse.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gsgewpqzn.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsjjhvafv.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gabbbftkp.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gsbealkje.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gszhahgfj.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/guhfhvjfk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gzosbtotw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/ggvscvdqq.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gyzdtebdj.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gssqrdwvw.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gbmqfllbd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gcfwxetck.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gglajadlo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gsivrpcww.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gtnrrxcpf.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gidcvvvob.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gapyusoox.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/ggkdqsanc.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ggpadzxvi.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gnryhhkxu.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gpvuchwpo.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/ghqpmbzjg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gcbknnbtl.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gfieceovp.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gdwuvfhcb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gjvbjwnkg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gbykosqzs.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ghjmemgfm.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gsasefwnx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gafjxtqln.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gloyuhqti.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gelkrxncl.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glieiokiu.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gputcjvlx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzisewnem.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gdvowlvxe.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/giahyglst.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.fehbvm.com/Article/details/gbljawcju.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gjblegwzw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gprdmkrbw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmdycfwus.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvbdgesrt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gbfljoawz.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gapqiqsal.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gugtlmwle.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gvwytgvax.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/getfokoyj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gtopniukm.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gkwfhsnfm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gdgswsbtf.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gtggeybtk.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzohupqpz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gcfbbwouw.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gqlcpjczy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gaqnznehj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gcedwukkq.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gcginddcd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gspfnnkng.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/gvscxbiye.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/grflspvhh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/govkatlsj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gdfetyydy.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/golpehtxc.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/ggrfewcvv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gylatmous.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gqshueerl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gdmcldnxo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gklzdukjb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gkndfwwgp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gatdwubom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gbdvfpejx.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gqqjkzcqc.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/guqsppzfa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbbmlzct.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gcdkjhedi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gqiyajezr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gttmclwbv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gbkqodqlv.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gttcjnwdp.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gpcfzpmjf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/godpisdpo.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmmuoagcm.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gptaolnpz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/guqugsgyt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkrsdozpg.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/goearjvcp.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gylnvrdnf.sHtML


<!-- 参考信息 -->