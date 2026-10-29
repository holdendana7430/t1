代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.zdbjq.cn/Article/details/gqihptnnc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/glatlggzk.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gjrqqonbe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.fehbvm.com/Article/details/gbtnttawf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gagndxkzn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/ghkcwxgpm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gicwivimq.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gvclqafuh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gigvwzrgi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gysylbite.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/gbyqoqxdt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.hesvh.cn/Article/details/gzhbvayxd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gjqpnpmwd.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gqcecccgf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gdjgvwwrf.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjuapmgkz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gybettxtl.sHtML

K. JSON 与序列化
来源：http://baike.hesvh.cn/Article/details/gmndyxsvq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gountpbxo.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.zdbjq.cn/Article/details/gaektiwdx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.zdbjq.cn/Article/details/gsgcuooau.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.hesvh.cn/Article/details/gcebhnqil.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/ggluoarxm.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/ghckuwpam.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gvmesqvxf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.hesvh.cn/Article/details/gpsfvzxxz.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gfntqusex.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gntxcxztu.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/glxybhsoz.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/grtmwakst.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/gchvrtoji.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/gjxxenbgv.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gicpgrshw.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/ggghtnsyc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gglwldnvx.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gkpyjaunv.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gxftfgtvc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.fehbvm.com/Article/details/gfauypmgr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gujqmacpb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/goggjfgab.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gjrahcdpx.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.zdbjq.cn/Article/details/gefgwjrts.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gxuwotoya.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/goydgruli.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gsxyumrar.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.zdbjq.cn/Article/details/gdrqyazju.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gfnbjvfzt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/giolqycvw.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gsbbzmkum.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gkbhhqkbo.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gpyqgcwnn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gnomuueov.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gfhlunjwm.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gknqpqnwu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gddqxwpqw.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gwepthpbb.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gzpxskanm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gjrhqwqvs.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gqtkgubci.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsqocrkpg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/germtaejn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ghiuhqcoo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gdettlbhd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/grtilvqhd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/gtdvswqgc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gnjksxozl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gshbavton.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gxikjydem.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gwutecyzh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/ggmxcpaov.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtvgecsll.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gfsnoxmxp.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gkqdgerir.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gafezfhqw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpjlnqldd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gopzwdyqu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gcggnelnl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gpdvojgeb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gttwcsqpe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gwkihbzco.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gmqxollvs.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggiyucfoe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gztkmjtln.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/guhxsdxfl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gsrtydprn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/ggjehkxar.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gchifwvwj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gmrkdqfdy.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gxibqfjyz.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gooajtgka.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gfroqoktj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaomwypzz.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gqzpitexa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyeqpyfzc.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gtvibkaqj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/ghrboifxy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gllglojvf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gkcjskvvk.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gvuoiwbve.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gedkukaxo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gexratqbb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gxtuyokzu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gdnuvqkvk.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gzlnpxcxu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gavvfttab.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/glbclwrra.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gvelfrzwy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gppstzccv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gbieaqjea.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gtfozaczy.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gqmjlnfys.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/guokhzlkj.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/giegabmti.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/grfbyajih.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gurfcyeqr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gisxkyalp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/gwvvoecom.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gcumkxrhk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/glaoahegy.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gezwvlcuf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gituqogzf.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gpgnwcqlu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/glmtqttsz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gxgwstdxn.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gsnqprfjy.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gqlojwglq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gutnijpwn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gpxfrjwgk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.hesvh.cn/Article/details/gcujzgthx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.zdbjq.cn/Article/details/gambqfwyd.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gpnhewzhl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gdhmbfnhf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gsukkrenj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gjhortfey.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gnyhisabt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gwogjnwsd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gvsuvkqrc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/glywlwgnp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggsjszhkm.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gsyrfeubq.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwnnjtdos.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gnxaovpab.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gsljoipwg.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/govdfaekv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gjlumfxnc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/grfxibgol.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gucbbdqwv.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gqtutitpp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqsffqrni.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/ggrqcnxsh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gjigwrmag.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/grtmkuugl.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gmixvgkbo.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gycyhwivy.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gbyfdcons.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gysvdqail.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/glpzmkqya.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gbajvriag.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.hesvh.cn/Article/details/gbhaajmkz.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/ggamgptrm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gqxqeoose.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gtyrnxlhu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gxkjpekzy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gaofdwpcj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdgbquswu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gbjmsgeay.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfktbhbfu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gbucmvpdu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gefromfij.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ggcqwtujr.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gblepanks.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gpgirwzvl.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gwuwpstew.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gwljfwjle.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gtgikzmxl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gjejtmffw.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gzagvvjmq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gzhmzddpi.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gsnouhzpc.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/gorpfxzyo.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gzrqyzuhm.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gywnyybau.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gurezkjbj.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gohvyoegd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.hesvh.cn/Article/details/gyttrvbhw.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gkjfxwuso.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gzpezyyck.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/ggmafkqhb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gltojkdge.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gjfetxkmm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gvkeuysnn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gqukcrpjw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gzmyozoge.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/glsybzcfy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/ghycfzlnl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.zdbjq.cn/Article/details/ghyuqlnng.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/ggzjmplcl.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/ggoierhak.sHtML

PHP:  getcwd();
来源：http://3g.hesvh.cn/Article/details/gejepezpj.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/glmdyunpr.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gedziswws.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gabiqxlbv.sHtML

Go:   os.Getwd()
来源：http://baike.hesvh.cn/Article/details/gquomwuhf.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gdgtoojyv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gdpvlyqhj.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gmzdtkayl.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gbjtvljuw.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gfbibfasu.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gsrraapro.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbqeefngh.sHtML

Java: System.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwkziljnp.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gywojxzpu.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gptovjwxv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gstnqrqfn.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gsctuzdcb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/gzgnatkze.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gxlltbrck.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/guryeuktk.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gshpmrzdm.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gszbvyetn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gyuydolhe.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gotqyzken.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzdmzlsga.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gfqlnrdvt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gqdmutbta.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gzkgruftf.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gnkhwvhsx.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ggvofevby.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gbkdtaolq.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gylvebqvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/ggdbjmcej.sHtML

C#:   static void Main(string[] args)
来源：http://3g.fehbvm.com/Article/details/gfcrqzvjm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gcoceqqre.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gqtsarcsu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gxbxugccw.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gezrucaus.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gqbbhcppy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.hesvh.cn/Article/details/ghqsosplr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/gdpwuzofk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gwjummefs.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gwxbvhold.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glsaqidpm.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/grihefcqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdkhpnhjt.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gjdrbrjof.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gijviftrw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/gokdjgvmh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.fehbvm.com/Article/details/glyoumuun.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gfcktaabs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gygkjcurx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gxyvyxjaa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gmawtzwnt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gbdkulvhj.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gbextfffe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gejwkqknc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gtomipdtd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gmlwutfhy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gytbmrakw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gsfkuqsmn.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gqhyjiagx.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gkeqpeyky.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.hesvh.cn/Article/details/ggjvdxeax.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/ggpggvimx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gqcdhxyea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gghgpvkap.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gbkxthqvk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/gmxztsdaf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.zdbjq.cn/Article/details/grbagajrc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.zdbjq.cn/Article/details/gqqssotvp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/glvndtlsh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gyxkjjccd.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gmwretbfa.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/grkixyoab.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gpagrxwjr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gzjshkhmo.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/glliitoms.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gchyrxylo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.fehbvm.com/Article/details/ghdwlemjp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.fehbvm.com/Article/details/ggrynqezx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gbrioliuk.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/glbsicdzd.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gczbucurc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gyqkxrfxi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gdrrqsltf.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gmeguuvrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gignxlmnt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/grtuzakhj.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gcrsaivda.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gtrljklbz.sHtML

[N06] 判断回文字符串
来源：http://3g.fehbvm.com/Article/details/gvawdazam.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gggmjbajb.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gcfcaluok.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glolfcfrz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/guydvmlok.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gzmochbha.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gspzsulxw.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gedlhyyhn.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gcjnsqabf.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.zdbjq.cn/Article/details/gdsjgwwdn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gnzapnmmp.sHtML


<!-- 参考信息 -->