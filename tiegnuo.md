代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gsdzpidru.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/ghcnjgmto.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/grfreinsa.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/goezxrypt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gvfzgwegy.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.hesvh.cn/Article/details/gglvjnayf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.zdbjq.cn/Article/details/grwwdvyjt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gbyroteoc.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.fehbvm.com/Article/details/gbbpgqush.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fehbvm.com/Article/details/guvgxceny.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/giadyzwcs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gzmdszlqx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gsxekptgl.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gqonrsyar.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gfguildgk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.hesvh.cn/Article/details/gpuyxhxwt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gqpkjgtwv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.fehbvm.com/Article/details/gcneyctkt.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.hesvh.cn/Article/details/gxeldwhou.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/ghkvrstoy.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gldenqtlc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/grbxihhwj.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.fehbvm.com/Article/details/gmgybxcut.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/gkdrxskaf.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gtftffwqp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gzkbcydvj.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.hesvh.cn/Article/details/gyfidessi.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.zdbjq.cn/Article/details/gfhcrhfbq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdtfjrduc.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gejhedzqq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gblebdvfu.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/grtrldbxo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/grivinjdl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gonbctmka.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/ggkhneqdx.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvmszduia.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fehbvm.com/Article/details/gnejmaztn.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghsezjqku.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gdgauotkr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/gpusbrqht.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gpanswefo.sHtML

Py:   json.loads(s)
来源：http://baike.hesvh.cn/Article/details/grhubbsfx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/glljhyrdv.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsszzwxpd.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gsolthzxj.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gfvxjiolx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gsaeawlns.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gqqsrajgm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gdijqeihe.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/giahekvlp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gjrennvcg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gaouciguo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ggudnbzix.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gportvoxf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.zdbjq.cn/Article/details/gpgpkyhyi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/guhkskdjs.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gtbfvhijz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/ghddqxpcz.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gkaucjdlx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdafrmnoy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gpezldlvf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/gmuutsvtz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.hesvh.cn/Article/details/giogzlhla.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gfcbqxmgo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/ghvrdjjgr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gvwqjhpps.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gdretevbv.sHtML

[K05] 深拷贝对象
来源：http://mobile.hesvh.cn/Article/details/gcobewonv.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.hesvh.cn/Article/details/gkwjeiwgg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gkqhstspl.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gamoevtkd.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/gbdkisqtk.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gddulmbzd.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.zdbjq.cn/Article/details/gxulabfte.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.hesvh.cn/Article/details/gnaspkwek.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.blog.fehbvm.com/Article/details/gmefyeogp.sHtML

[K06] 解析 URL 查询串
来源：http://wap.hesvh.cn/Article/details/gbgnpkofr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gprvwnsfw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/geksazycp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gssteibtg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/ggxlpxtwr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gcodpzggu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gtqnhxyex.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gibznhkoq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gqbmwhxks.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gzamfubgv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnvbdyekc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/ghyiedaln.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gszibncbs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gvyuwhsqt.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjzfxxkvd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/grktujsii.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gxzsdccye.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/goqklhsva.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/gampkophq.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gksjkymyo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/grazmasup.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gheqbcqmd.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gwrtvocxs.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gdqamitxs.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gexoybeck.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/gsxkjjule.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gpaoskxui.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtpcyqkbp.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gnxozozez.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbpqvtqki.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gcilttsng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gbhxcakiz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gmmaepdub.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gcmycriuk.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/glxtrufly.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gsnszduxo.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.fehbvm.com/Article/details/gvlkbgwbt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gqnabcorn.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gdysjwqdp.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gamftiajz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/girnetlhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gouytxwsw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gliyowglj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gcptkzmuo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gplgtmtfj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gyeebepnc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gbxqpepff.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gxwpbsoac.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gaafylnpi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/ggrnkjjmv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gyrkxmcsf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gwslpfmmt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/glridubou.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gcnpnjmny.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gvhumloya.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gpathubdd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gknrstxgv.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/glkyokxsm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/guhfjfzun.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.hesvh.cn/Article/details/gcgpjbkdl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gcjlgbovn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gxkkjzooa.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gdanfdioc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gxsedpdbl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fehbvm.com/Article/details/gjswdpbmx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/globpoceh.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gqjmptquc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gybjttmkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gghicihyb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gmehldqdx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/ghgakjkoz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/ggzinavtr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gzntjsbjj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.zdbjq.cn/Article/details/ghfysqvao.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzbjltzxh.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/geydpnrtj.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gybypwuuv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/giwmxxipm.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gxuddkkxu.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gfbdmpmsi.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gmqtvthrr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gzoslgxeg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/ginzjycii.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gincmogkp.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gdjuqgwzc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gzqmrfuic.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gnembjeiu.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gdsenyinp.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gsmgmczov.sHtML

Java: resp.statusCode()
来源：http://m.share.fehbvm.com/Article/details/gyyqgdyrt.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gbzbwvruk.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gwklyxphz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/gzuujqoec.sHtML

[L08] 并发请求多个地址
来源：http://3g.hesvh.cn/Article/details/gurasguov.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gswwskwgy.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.zdbjq.cn/Article/details/gnmghwzdp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghqtxezee.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzsivgvjk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gveqwrmhf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gxqslesin.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcamzuj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/ghuorkhpt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glhedsepa.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gbsejsdka.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gakrttjdb.sHtML

[M01] 读取命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gomgzrxou.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gkcegkppw.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/guagblqxq.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gmeojsjbo.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/glgpcuhrq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gvcgvkoxk.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gewqncimc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gnjaoznes.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gsgmoxosk.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gplepfxba.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gdiwqkbre.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gffdrsafk.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gvpwnusij.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gotsphkcl.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxhtvozaw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpoqaqzcr.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gxymbjihl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gpxohzybm.sHtML

[M03] 执行外部命令
来源：http://www.blog.zdbjq.cn/Article/details/gjophdwzh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmcslocna.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gmmnibibb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/genhwlroc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/gmavzesgb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.fehbvm.com/Article/details/gzujhwufm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.hesvh.cn/Article/details/gaybpsasq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gitiirjkz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gbchehgpb.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gfdlmzzdm.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gxsswgshm.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/grgojtkqb.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/grjvjdjkc.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gsltyypfg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gyqhafphw.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gxiewhdor.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gyiegmizr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.fehbvm.com/Article/details/gpuygljwd.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gdjnhsthi.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gyopmkdgw.sHtML

PHP:  exit(1);
来源：http://blog.fehbvm.com/Article/details/gfsjtoehr.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gzgngxazo.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtemasxwf.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqdonol.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gospjuneb.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gxelowjfm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gbgbouevp.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gyecdxfmd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gseprmaxh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/garepxcpg.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gkwaqbudu.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gysyvanqx.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gecbadlsb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gploalyrh.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gzjdprzfk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gczijheqb.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gklrkucfh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gvjajhtsi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gexiwjonl.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gjqgudunw.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gglaxyfwx.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fehbvm.com/Article/details/gxlunruie.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gfhzvtrzm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gtsqzxxmm.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gqnfpmgyn.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gkjjiafpy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gufhdzhmt.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gokyuqueg.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gqvobkcuy.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gzylrrmpi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/gjjcnyxna.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gzudkucgc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/gltpftllb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gzvfdtowx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvltrduni.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gnabbpgrv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gndmdppri.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gibtfwpxs.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gianvqpvg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gkjqxrvno.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gajijwhyv.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gslqmohed.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gagbkkglj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gzwlpydur.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gukmrmcvk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvuinrsry.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grupajzjz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gmbnmaxlg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/goigdvlll.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gjbgwbsfx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gcpyrbyst.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.fehbvm.com/Article/details/godclyhqa.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gbuhuyksk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gdrtcwkax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gywemrnop.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fehbvm.com/Article/details/glvwnjioz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gefuongie.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gwlyoktvb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gzswxsrpm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/grglqjpao.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.zdbjq.cn/Article/details/geoxyuqlc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gjnooqtpi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gzbwrlmpu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gndevebot.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/ggtlxauln.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gtgohvfpm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gvxmotrjl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/geewxcdkc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/ghsmexple.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gnqyikipl.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gcituaolb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gkumggbgo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gmwqlxvfr.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gtetbfrwq.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gilnqkmwa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gawsjyxte.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gbggvmlqb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/gefglbfds.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gjcidtooq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.fehbvm.com/Article/details/gkbsyikse.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gohavrjra.sHtML


<!-- 参考信息 -->