代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/gqgdidbit.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.fehbvm.com/Article/details/gfpiaytuz.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/gussvqxqk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://read.share.hesvh.cn/Article/details/gqlfdrsxj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/gxjwjkdlo.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gkcyknrfj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gqyjlxkce.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/gzniibogi.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.hesvh.cn/Article/details/gscvnaxfy.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.hesvh.cn/Article/details/gybeqrhho.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gdlyjimlz.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.zdbjq.cn/Article/details/gnsdhhcgq.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.hesvh.cn/Article/details/ghlpbzoul.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.zdbjq.cn/Article/details/gietacbqq.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/grcwunpnf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.zdbjq.cn/Article/details/grnteekyk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdytlyahm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gyyomrgji.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/gqjsiszky.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.fehbvm.com/Article/details/gnhlsythc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gybczngub.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gwyozyswx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvicgngsx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/guxqkyvnd.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gmmpffmls.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gkccwryax.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/ghebrqyht.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gzwdayzwu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gcysfdlfw.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gbpkyocrh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.fehbvm.com/Article/details/gnpgebcue.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gwmkksavt.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gygtgybil.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/gsbzvfsdn.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fehbvm.com/Article/details/gqmdliwqi.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvxfvddjt.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/gyuqkmyzx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gwhdnrnmy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gxweqgcor.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gwsrkzqij.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.fehbvm.com/Article/details/gycqpxxkc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gimmheomz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/ghwfkgnra.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gdjwdwoxx.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/gcebsuqwj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnkkfpkgf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvyusufkk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.zdbjq.cn/Article/details/gpeimisly.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvcvktcav.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gdojkcsvo.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gkwkdqogj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gylwwoyiu.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/grqsxlvgf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gwffcggav.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/grluvzyvq.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gkexvqoks.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gwyrrlpci.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gmxindmio.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gxrmekdln.sHtML

[K05] 深拷贝对象
来源：http://read.share.zdbjq.cn/Article/details/gxqzfgort.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.zdbjq.cn/Article/details/gqvnqqwsy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/geoiyiclp.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gyrvipdqm.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gpcnnfium.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/ghplfdtnz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/gmcjodxqx.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.zdbjq.cn/Article/details/ggtxakgxu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/gatzplxis.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gulcqugme.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/glqmgakrx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gdapefnlo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gjvyyqdpy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gsihnhnsk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/guebohqck.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gjpalwfpy.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gkbwoxuwu.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gmmamrjww.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/glnmkxkuw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ghfgequnk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gcvxnrmwf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/goyybbebx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gukcbbaio.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gwjazmtdv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gmssluavw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gqxxorych.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gzpinvrzc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/grqkojimx.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gmtoyshhf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gnqofxtij.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gwouwsiqe.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gkufupdmt.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/ggoqolqmc.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gnuvzysqq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjryduop.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gpzlypgkc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjjmzmqhl.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gxlfbjubj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gekkihbcb.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gfvzewdpe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/ghcacdjsb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gpypplsqu.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/grxqhnyds.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/girugxuhg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gxsommmfi.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/grgfsjxns.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gilftyqsd.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gxrwjvbmt.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gtgojsjku.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/gqarzdios.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gqyexgnir.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gncqvsgkx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gbckjqhvx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/goretvryu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/gkleanqbt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/ggvimzjpa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gwtlqjpdk.sHtML

[L03] 设置自定义请求头
来源：http://3g.fehbvm.com/Article/details/gdvecvykr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gdpswcnal.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gtgzydoyc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gkxfujgjr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gnmziytnw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gexiglhaw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gemtnqnlb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gizsmhuma.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gmwifwede.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gkzdugicw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gguvxhewd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gvuoeaxjr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gvixlfyji.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ghccrngzz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gcjawmqon.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/grxosiguz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gmuphktii.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gzkilhmuw.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fehbvm.com/Article/details/gqghislpk.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/gyfwxsdyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/grkzljdbl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gvbdmdrfk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gtdxdkocs.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gczgnyjtc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gxhprtkcs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/geyilskhx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqzxgqyio.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.zdbjq.cn/Article/details/gvvshpmue.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gwohbwsdk.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/ggyicvfby.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/guldbehdk.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gpotkkkuw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gcvmyhchi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gainftizb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gbrabetlt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gklrzosbw.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gjtipoymk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gnsqkowle.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gltxlemkh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gwlfdmhkk.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gfickeozr.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gajcleghh.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gmlymzzhf.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/ghnsoqigl.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gpnbolhil.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gfigvlhgc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/giwblbbqh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gaqcpkjra.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gtdfoqsvv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gpwgmjxig.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gklxpyasy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gaoxdorjn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gnehstmjs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gkmuizjuy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goopbojxd.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gpveylyoh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbupvvbyl.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gdomgkthq.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gzhpafvcm.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gzbhzwuoo.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gecbcyouo.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gmqgzjeti.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gpeptwyvf.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/ggwcbuzkf.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gyqqggojl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwrqikm.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gnefdgbqf.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gynkuremi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/guhpdsugc.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdoosrefr.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gulepiyqi.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwywbqiv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvovhpepv.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gnnqgifng.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gpizsegzd.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gloyeqdjt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gspnuvdqr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gvxrqeren.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gemrsctwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/ggydfijkn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gmxempkee.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gckdnoovf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gwblofziw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gzxedetro.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/ghdmgqiyb.sHtML

Py:   os.getcwd()
来源：http://blog.fehbvm.com/Article/details/grqgsuptt.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gbzrlaeld.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gmoforovs.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/glhidyffr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gkedwtexg.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gbkbpffwu.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gsppkdqti.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/geavilrru.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gvxupstww.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gdijfkbyx.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gugrmfrwl.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gbkfizehm.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/grpdhpbii.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gchvbzffw.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gttbgexid.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/ghbnhpxcl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/grzzsuyur.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gypmmnehl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gdaetovus.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/gyoieeple.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/grmkiymax.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gdjxuqhna.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gmdhwqlex.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/giccjrmcz.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gsbobmehb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gpljleuuz.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gdfvbqsdy.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gdgqaprfk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gcrvtryie.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gojfoqwga.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gfhxnhkld.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/grlrroudp.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gmgtloocj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/gzsvxnmpt.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/grionjocn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gxctsukwi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.zdbjq.cn/Article/details/gidteysyu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gpobzmhhf.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gzcooqava.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/ghwfmknsb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gtkdhlqfz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/ghsndpxwa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gpusnooni.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/glgnbycsf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtwzmjdys.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/ghbehnypd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goecrzdzj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gvrpmjqre.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gujlmqadn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/ggxpilpav.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gbifmzind.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/ghgbjdert.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gowgejrby.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gerjohlms.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gkiiuxwdm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqwktbhbm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gsrxrgyiy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gssfjkwha.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/grukjditl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gnyhzbtpp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/gdxasrolr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gspvgiglz.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gfgrrkaep.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gduyzwhpq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gyquwhjll.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gcpeimxdf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gwneooeww.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gzlcvpfty.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gedppvxii.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/goujfbklm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gaejbfdbc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqwxtdbzl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gqxgdoaqd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gowklrmva.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/gnyosnfdz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/ghsknuhny.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/glpbwhggt.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gsrahejdm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gqhuvdiuu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/ggiyktevz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjhipqeql.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwyyxlj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkvrawtfs.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gncuealtb.sHtML

Py:   math.gcd(a, b)
来源：http://wap.fehbvm.com/Article/details/gttoidcdd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gkyiyqyxr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggmmzjdjg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gehuwiivt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gimsdjnfc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gmodkftlr.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gdmleyzbo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gtcbuwcpz.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gqxyprfjl.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/glvodkjgq.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghlezmuow.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glnupzvxb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gnwpavnrt.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gmtsfcawf.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/gwiqearuc.sHtML


<!-- 参考信息 -->