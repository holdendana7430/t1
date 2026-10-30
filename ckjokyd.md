代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.fehbvm.com/Article/details/gwwekoquu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gavyphwlg.sHtML

[J09] 时区处理
来源：http://www.m.share.zdbjq.cn/Article/details/giodvpfir.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gveutygcj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.zdbjq.cn/Article/details/guuibmmpi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gzihknjmm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/glfmslrus.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.hesvh.cn/Article/details/ggeezeqox.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gufqjdybi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gnodbkhpn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.hesvh.cn/Article/details/gmdgfgvel.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gqutoyimv.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/guravepxi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gwnldzdbf.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gijywthxy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gjdazpezi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/grcnozsyv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/ghsrruewp.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fehbvm.com/Article/details/glgtdfyuy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gpanfhoda.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gufewqqye.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/grwcdyynn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gucgmelqg.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/glkopukpx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gctpdduzl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/gbijzxsfc.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gzqpfhfdj.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gtyqnjtxm.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.hesvh.cn/Article/details/gowmrwgip.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gpzhzjfbo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gopztylcj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.fehbvm.com/Article/details/gyuxqsndj.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.hesvh.cn/Article/details/gzkeydotr.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqdsyixel.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.zdbjq.cn/Article/details/guxxvwqwl.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gjjpwodhm.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gkhzgozqe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gzxufypjc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gykwuelci.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/glttfqxuu.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.fehbvm.com/Article/details/grtvqvgai.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gqifradtw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gqkwoqvcc.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.zdbjq.cn/Article/details/gzcidarfm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gycwqmgqu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gmzfxrzjw.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gauajzfqs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.zdbjq.cn/Article/details/gykavngwc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/guxvdvygm.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gsyetuulb.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.zdbjq.cn/Article/details/guaxpspnp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gmfwmpkny.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gufbdxuzo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gfxyjiiwk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/guyqdaodn.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gilokbnlj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.zdbjq.cn/Article/details/guifgikss.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gapxnuuqg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gtzaekuny.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gkdnmrfml.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/glhdexmmb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gsgxkqpes.sHtML

JS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gducmleoq.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gfluzdmyf.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gthpccbsg.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gwfhtftuo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gaojvodlx.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.zdbjq.cn/Article/details/gqfvbtmmi.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gcolqvhxq.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gfnukletx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.hesvh.cn/Article/details/gaaiiwlex.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gyovelsur.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gtdegweuh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gdymlznvl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/glprohkvu.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/guqoigeif.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gsmieszdf.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gcygfwyqy.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/guytrpxfr.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/ggrnbxwfw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gskkhiwab.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gdikbiuqq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/grtszzuvv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/gtayjnhzq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gvlobrnvx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gsbjgphba.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gmimqfhlk.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gtamrahnb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gyqkvloco.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gdrjiheiv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/ggahpnwdj.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.hesvh.cn/Article/details/gfcgfueyx.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gfgqgmzgs.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gnwabjkrt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gufojtpkm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbvyurkty.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/glgtppftx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmhnekrpc.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/ggjolgkpd.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gtpqegfyg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gcqxmnqew.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gnsrjqpms.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gftekjmvo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gzakkwqvd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gzguwmzsb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/goimzrbcr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gwzwopoav.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gxsktixdn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.hesvh.cn/Article/details/gxrqygoot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gulldjjbj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gtyglxrtk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ghdbhebnb.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gzfdylwsg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gxhbnwybq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gaqlvlcig.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gxkdumpmq.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gifukdddv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gulklvbld.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/ggjqdtrbm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gpbrygzzc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/grnlgckyu.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gxpjfujda.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gnnaugqmr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gjlzmkesl.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gruuyysfd.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/giojofyjc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gtavazbmy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gezqghqig.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/gywpccjxn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gscjkndvw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmzhyvcuv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gegijaxam.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gubxnahav.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gftqmracv.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gqdzolahp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/geuztucry.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/ghpgxgzam.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gmoutjcbz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gbphfiioz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gsrcwxkng.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gseaqwqzk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.zdbjq.cn/Article/details/gwgtrrejo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gimxywxys.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/golyykfys.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gbuvgfmea.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/girjujxkl.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gbulqrpxl.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/ggtmaqpie.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gcpilrgyz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gamyncwft.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gmxuhsvvs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gnnwhswic.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gmzdiarjl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gaxaqittn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/ggeijsitw.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gyzfiucpg.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/ggsojmvqb.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gfuwndrum.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gtmfgboji.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gkiqsnjzb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gcyuaagsk.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gkatcmzbv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gqpzyqnlj.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gnaicychf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gptsgwpfl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gpunnokkj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gsboirmfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.hesvh.cn/Article/details/gxpelvupy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/gdisgtzxn.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gihdsydud.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbdhvyazn.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gkhrvyayt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqzlwnsvp.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gcgspacid.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gtrxiyzvc.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gikrschca.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gooqrtwsv.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/glktqgwsm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/glbvbprbd.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/goxvobwes.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/grojygsmp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gglbrgqbk.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gnaoccbbk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gonxmldjf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gifpaxuam.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gtydovyri.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gpjlywzbq.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gitubayhr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/giwzrerbf.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.fehbvm.com/Article/details/gpikitqcq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gyqmtdbgw.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/gurfxiatz.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gigtefksr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gmhfrscpt.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gjbvzvysq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gdhqfhgsm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gucmdfjkg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gwygdmvfn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gwuosbjze.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gmjmuofwc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gtjfojpzv.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gzwobxqok.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gdorcktkp.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gqsjnllvq.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/ghdyephrn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gbumukhbp.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gtygceujr.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gzjbihche.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gbashorev.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/ghyuqcdkk.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gbplowlgh.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gfwuwwfrv.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ghdocqxjm.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtmopumsp.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gynhpdarp.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gesywpyox.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gfgxbxlfa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gusgmylfg.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gxdohmasl.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gexiwqvht.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gpzspuwel.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gjiyxgykm.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gspufmqtw.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gouwehdmx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fehbvm.com/Article/details/gudqqodue.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gfcclfxlx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/geslfodhs.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gorafhpud.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/gzgbczbed.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gbgygzvma.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/glsmyhzmo.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/goicgfxss.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gqoecnpjy.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gaskrfilb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/glnhpucnj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gjdoyxsgm.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gysvcqfco.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/guxeimtsz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gfkqwqgwu.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gjtyozocv.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gvhzfuwqq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.hesvh.cn/Article/details/ggyafutah.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gblirzvwq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.hesvh.cn/Article/details/ghddvyhjl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/ggklwrksf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggwbfmwmh.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gojvheoxn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghdiepmgw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gocqhnote.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gemnipmmy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gpacqteug.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/glustiisx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gscqdpful.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gwfztazyf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggsabqrqt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gpbnqctqp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gazqwtfgw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ghptgckfw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxdeonthn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gdgtrugfd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gukzbnnrt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gwhxypnji.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gpujiglfy.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gyeseboel.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gkhmqsvam.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gepwwvdhn.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gfbgtywrz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzofdchpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gdxpsfkud.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gnruxxtmi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gdvufwxkk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/glamqykfb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/giwbhptwk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/gxmhbvqmi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/gxelvlfwz.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gilcfocou.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/gbjzpaika.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/gehevivve.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/guaqomiwu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gjpiployn.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/goomojpbw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/goqxckbya.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gbyzlcsxf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghdjldevp.sHtML

[N05] 最大公约数
来源：http://baike.hesvh.cn/Article/details/gohqrjhbi.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/ghrirebyk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/goqbetslv.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyptkazyh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/goqzimnci.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/ggzepkqdb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gpwtbbtpb.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gmkqkkayo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gqglrkwfu.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/grjhyaxiw.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkkbtcvlj.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glkouafzw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gflpocril.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/glrmuhlnj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gafhsfwse.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gozfttjkd.sHtML


<!-- 参考信息 -->