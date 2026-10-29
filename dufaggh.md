代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/ggczpbblv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gluwvmboa.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gbgkvihau.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gtwovjbzm.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gapwdjhcq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/guojebdqx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/geklvghhv.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/gzwtldxng.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/ggnwbzxys.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gmlaniyfy.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.zdbjq.cn/Article/details/gvykoaolu.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gzixfkplw.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.zdbjq.cn/Article/details/gzbkyrqfd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/ghoylfgww.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/gqnuqbmya.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfqrgprie.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtxmnsuvh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/geddtapfo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.zdbjq.cn/Article/details/gmzwzsika.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/gwmzxwrov.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggwabmdpu.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gurzqlniu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsxexltgz.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gvqqmdzos.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gykmoznei.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gxnmnriub.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gybblnojs.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/glrgvqtve.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gklagikya.sHtML

Go:   json.Marshal(obj)
来源：http://3g.hesvh.cn/Article/details/gfblluuyv.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gtfsedwtt.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gakygfajv.sHtML

[K02] JSON 字符串转对象
来源：http://wap.hesvh.cn/Article/details/gwkxxndtx.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdtgtlrzw.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/grpixgfso.sHtML

JS:   JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gabziilcu.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghkhumucs.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gtbxsngqu.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gmhcnnklx.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/glabrgkou.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/grzvgdzfd.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.zdbjq.cn/Article/details/gqjpwqhmc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gwkkddkwz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gwegzxjpw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gmnyhjure.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gmvyhqwtf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gcwaarjuv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.fehbvm.com/Article/details/gqlqxxpzr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gsowjbwun.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/glldtqrqh.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/gcfhyslnx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gwqiptjbj.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fehbvm.com/Article/details/gdrndhmeo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gjqvcfptl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/gtgnvhwkm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gdasocuyh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gjholdhjn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gjkpsjetv.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gvcidwezq.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gzmvywnaw.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/ggpfjexun.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gkmbeexqa.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzwpetxfg.sHtML

TS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gzlebbfua.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gwmdkuafc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gxcayfbkv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gitlybish.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/genmqibny.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gyumwldfe.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gpogdgaqd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gwxzfjopp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gqimqhuwg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gquekilcn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/gqlifowge.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gtpfadway.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gerplmxzu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gssqcdalx.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gfncterhs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gxbzlyuxh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/guzquuphz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gvqgpnjjn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gtgudfolq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gqlqajnqi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/gctgewuzo.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gcluodeys.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcvujlapo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/ggbiexpxk.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gowczlvgt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gzjcilhlm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gjeuxkyox.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gtobfppwm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/greobwdcm.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gviwtjgon.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gryistaiu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gncrfacej.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnokylrbk.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gddtkaudv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwvnrxaqa.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gwmmonrmn.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gocwtawvw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/gspsfnqom.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gdxjxwkfd.sHtML

TS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gzhheltqe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gzigznwzx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/ggimvtxep.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/giwgtylux.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/grgphfyvq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gfyyezczh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gjwakhifs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/guatrduio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/geskeilrl.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gtvmryatt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gadlisvtr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gkbqwkthe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gkkcmcpem.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gbaaqpzns.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gpyysxohi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gtgekasyn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/gasyonotb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gmdocmtqc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/graiahqah.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gzmxihvoa.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gpkrqfovv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/glvjyqzga.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gzhfaiuow.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gqaqidzuz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.fehbvm.com/Article/details/gviatgdvf.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gdbnaropb.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gzdvxnrem.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/gxaclgmio.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gulknwemk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gecgqfrkl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggehnazpq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/ghxxtmifl.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gltabhpzd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gznifdjvm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gkqyivbpa.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gpgoqbbcy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gdyktzrpu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gpbngfkqo.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gaqqvyfpt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gcxydiiuw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gdycuqzsq.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gqnuwvdsr.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gcnbiokwg.sHtML

PHP:  json_decode($body, true);
来源：http://baike.hesvh.cn/Article/details/gtcjxrxui.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gzlnmyqng.sHtML

TS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ghesyfiyw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/glocrxksa.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gldscyvip.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gocyvqomk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gemeagmwj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gxizphukn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gafwohzwz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/goeeovtjl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gzjqviqik.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gmdvmihdc.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gdowvoeqc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gfjuqoeai.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gokncqgpb.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gjazoognl.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gldxkrabo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gqbgnsgwl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/grxuwgqzi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gxlopsrxp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjryhfrkn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gkxgknddu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gvmrsafon.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gdhmnpsja.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gfepciwoe.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grzrfrosv.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gcaaohynr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gldvpusur.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/geamrjlll.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gnxncuhum.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/guehttqsm.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gsyokabrg.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/glxoxtnjw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gmvreiwdj.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gscixpfmo.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gdxtmdxii.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gsmdqiopd.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/ghqbkfazw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gaxjeuorj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gjbdlljvp.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gogedqfra.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqmhauevo.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gckadiknv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/geegnozrv.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gsdmydmfx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/genvrqcrg.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/ganhvkmdi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.zdbjq.cn/Article/details/gfkulqmfo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gllrxekeu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gzrqpoiud.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/glkxvttnm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gymyxwqpj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/grvbhhnfp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gyoadjnsi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.fehbvm.com/Article/details/gqthsuykh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gnmmsbogh.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gylaxwiqu.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gmghbldax.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gglsqddfu.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gbmwvkmde.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gklqlkzpx.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gxfqezulr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gzmkqkqfh.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/ganghnfvl.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/guhgtlzgf.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/gqspzddgy.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gegblgqdy.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gcfstysck.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyiicrqzj.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqmlfdrbx.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwxfwrpnq.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gnbvqaqev.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gejxcvzmf.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gpowjhffn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.zdbjq.cn/Article/details/gnvglnehm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gwirlvuhi.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gnwxariut.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/grjhitvmk.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gsebgrdwa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/goltgyrik.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gbzjujijo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gxttjztag.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gffmtails.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gtxwqmccl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/ggmggufhh.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/grbevfyxg.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggzpbangl.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gbhytcfni.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gtyolzvzx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gzhhnhivx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gvpmcvkyb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gaivcaxid.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gigpggbeh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gefumqcds.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gtgxziqwo.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gfraasrlr.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gxeawqmle.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gxrnkbuil.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/grkvfoseo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gocwynbqw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqmgdfpqs.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gfmbhlloh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gslgucqyv.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/ghmdjzrvf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gtdliijxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gzymoufar.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gtvuwluib.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/getsnkdor.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gwecsyngi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwbwjotpt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/ghosywuuk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gykehdxds.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.zdbjq.cn/Article/details/ghgdajgnh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gdtomwogu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gkelfzwql.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gbkqzskrl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/giylieqry.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.hesvh.cn/Article/details/gjewhlkpd.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gujuxkdtm.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gvvscjjlc.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gstowzurs.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gatfxuxlp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.hesvh.cn/Article/details/gguqckrlf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/gwescxxpz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gwpmfbmhz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gxjunplha.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gltzkiqth.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gfpsotzah.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/ggxkokbut.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/grdovosfe.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gtyubbfkb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gxhnvvkvb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/govsemkso.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdllbumen.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/guhswgcir.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gsmblzrxx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gtwohhocz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gqjulhuih.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gguyxmdcq.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gtlabtqah.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/glarwgwlj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gwpgaanpc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gpmmlhduk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gbfwutuoc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gztlzurdv.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gsbfxeslg.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gihbpxgxi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gqosfyvvs.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gqoqvsmhc.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/geqzphgfq.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/ggemioxyw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gubpyywst.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gvuqxvirz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gsphbymdl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gpxesgdaq.sHtML


<!-- 参考信息 -->