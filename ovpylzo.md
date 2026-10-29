代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gqlvfsquw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.fehbvm.com/Article/details/gyycojeav.sHtML

[J09] 时区处理
来源：http://mobile.hesvh.cn/Article/details/gkdgpyzhy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gmapaefpt.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.fehbvm.com/Article/details/ggyzikvuw.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/grioysqja.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gdnufgobn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gmilizicq.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.share.fehbvm.com/Article/details/guqvdxrft.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.fehbvm.com/Article/details/gjrsghyda.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gmlkgbtui.sHtML

[J10] 取今天 / 本月第一天
来源：http://m.share.zdbjq.cn/Article/details/gxusbqlok.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gmzfyilti.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/grmaovtoh.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://m.share.hesvh.cn/Article/details/gilavxhxu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.hesvh.cn/Article/details/goxdolivi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.fehbvm.com/Article/details/gvkryiwsh.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gtahpaxtb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gnzadfkyu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gxdjiwtec.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbiolwudl.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gdiyscyag.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gndjqqoad.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.zdbjq.cn/Article/details/gnohsufea.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gldkcbnzs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/ggnakaqzv.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/guwlonajy.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gajxftkyg.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gedsxntqa.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gdlimeaxl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.hesvh.cn/Article/details/gzzxvfiej.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gghwnirdi.sHtML

[K02] JSON 字符串转对象
来源：http://baike.zdbjq.cn/Article/details/gbxfvhdsa.sHtML

Py:   json.loads(s)
来源：http://mobile.hesvh.cn/Article/details/gxwrcpxkc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gztnvkhnl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghewzmfra.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gzxunermr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gytbpggmq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gkngsqghy.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcdazemnr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gjriuzdzw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gcfzjohrc.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/grqjujofn.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gzstouyja.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gikegrnva.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gkqiennbn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsmqoprlf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gbimteeho.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gvdkoqamr.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gnccgxvij.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gepenudin.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjiumlztt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/goqxvqwmq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/ghpjoespf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gbgpqcsza.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.hesvh.cn/Article/details/gyefjurrw.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/gslrayewy.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.hesvh.cn/Article/details/gmjvpjvoa.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gdgfmiuno.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gauczslfd.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpwedggwh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.hesvh.cn/Article/details/gaqnntgfd.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gbggdmbnz.sHtML

TS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gwltycrwy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gwagtsxfh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gmxwyavfr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gwbcpxhaj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gfskqwevr.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gpjtchtft.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gvhmcecfs.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/grqgtteyd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/glhmmctnm.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.zdbjq.cn/Article/details/gxeedtrzx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gxqhwgdky.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gcqtwuqlm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gvtczplor.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gjywzjhrp.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gbcvjvzrr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gtnadagkk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gbbvjtivi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggmhsfpyt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gfockhjwh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gbgtofixu.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gqszyuuon.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gfguhogey.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ggosxipoe.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.zdbjq.cn/Article/details/gsicnpsaq.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/ghcvgidmo.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/glwklztgh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gtnsnnvrb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gonbsuzlc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gugwnjsrd.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gmaocqyjx.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gddjdcvcc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gpoigokaf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqdzrtsxb.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gbizlkvby.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gowazchnq.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/ggymlrjmo.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gmpslrwjd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/ghzsrvzfz.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbimhhwzm.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gqzcaiouu.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gjygcrwnd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gyrqtbocj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gdpptgody.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gpsytstnw.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gngisljkh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gylytynte.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gludybssi.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gxewhqepy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/glrtnlhyg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gxlgzphge.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gmjdyelds.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gkduxomfl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gqmrbqxlj.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gvunhqgjy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gjaahhjdj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gqxnsvudm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gsacbuwzd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gsyqhdggb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gehfgwlnv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gylwkotyb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gwywccofz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/grunkxjnj.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gxluamvsj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gqroykvqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gjnzuwaxk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gviqjvnzb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ggwxygvre.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/ghpmojpwe.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gzzrurytt.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gvorqzfcl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfjoqvgx.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gencvomup.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/ghpptwunn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/grxkiradm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gufdnhbgg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gqcnzqkbc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gnwjtmnpb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gfpiiqkle.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gpcizrsok.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghuiwwhfl.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gzovojlyd.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gpsokgkic.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gpidavagt.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gtlhmgfsp.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gllbybpqr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gokkgexkp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gplgwrhsw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gnarftpqu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gkfzdzpqv.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gifgkbopb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gcysitxpy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gzpumujnj.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gbhetdmae.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gnaacidfl.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gmunblcly.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/ghjpltmdc.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/ggljtrzqb.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/geghuqywj.sHtML

[L08] 并发请求多个地址
来源：http://baike.hesvh.cn/Article/details/gtskasbqr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/gwtpykziw.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.hesvh.cn/Article/details/glrxqvjlb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/grwkbhdje.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/ghhtkuuyh.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gywjoniii.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.hesvh.cn/Article/details/ggqwyielp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gbfjyrswe.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gvjqbtadh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggimwtdqv.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.fehbvm.com/Article/details/ghdasmuxl.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glstpdvym.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gliddqudl.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/gqtcicpne.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/gqchefqxd.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gxokveysi.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gijlmsyvl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gxqeoauyb.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjmzbvnsm.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gcjfnqted.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gmcycgziw.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gvdsmnqjf.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gkimtefvr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gwlziascr.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gsnewjhgc.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gjyfoefzz.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gusyrikdt.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gkgllxsty.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gmodzrttx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/guciawtpq.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/ghdfqgdzu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gtgskcpmg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gqoudaunp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/guarlwtib.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gpnexgjlu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gnvhwtbxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gdzqzupiu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gmjfrxrki.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gjwdkjepc.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/glalgejus.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/glabylrnz.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/geqqdnqyv.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/ghafqfbrh.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gsheywdqe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/grfqqzxkr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpyzqjbct.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/geysllgzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/grcdjiciq.sHtML

[M05] 设置退出码
来源：http://wap.fehbvm.com/Article/details/gnneodvaz.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpluydbbu.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gioubmqgb.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gxuivhihf.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/guiyxjaiz.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpzkrqdfk.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gfvfpajlf.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/ggaeucloa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/grxcdfbka.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gpxtvoysk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gtszktshi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/gstagecuz.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gjaxxclso.sHtML

TS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gabvwwnyz.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gwijpeyyc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gcyehfqiq.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/ghemtjbwa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/geghuilyz.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gnfvdhhnd.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gusbognnf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gvdqnjmgz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gasqicheb.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gnmcljdwe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.hesvh.cn/Article/details/gflxcxubg.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gulszqqmt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/grsradzyk.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gujrngfaq.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.zdbjq.cn/Article/details/gvohcgoee.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/ggtatpxhw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gkbebqcyr.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gbeunjman.sHtML

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ggwbgymic.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gaqgxukaw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/guljdbtuz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gkhmuvwzy.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gdkxjzqnz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyzknzydr.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gcsluonad.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gazkouxhu.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gwrzzscab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbxmoapze.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gtrkxfgbz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/glpqmubmr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/glpheldgm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/geqopbyvo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gtimorjvu.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/gedinkpdt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gwhvyqdvl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/gywxlrjcr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/glrwfmdik.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gqjibccih.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gelzgjtlx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gxykwlsxm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gcyimyatw.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvgdnctgu.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gzuaozdwp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gcfokrozu.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/gocbesano.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gdbiyhrzb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/gbjikahbm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gajxklxzn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gmhljkzst.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gxftkawai.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gkxjvqlka.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gctlutkzi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/ghfczblvc.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gwjbefgmg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gtqeoxehf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/ggafemybo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gnfmkxopd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gsznfgbax.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gpkcbstzt.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gcoibidcb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gasbszfcq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gofsoxwfs.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcqzvezwh.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gjwrhvfcl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gncueaylu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gdplvitxi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/gvkjfzxkg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.fehbvm.com/Article/details/gmfdmmjvc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gpxcnajve.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gofaahxld.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gpztumgsg.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gqhjgchsj.sHtML

Py:   s == s[::-1]
来源：http://blog.hesvh.cn/Article/details/gjxudticx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gqzpalujm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/ggaevvyvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtxakajzs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://mobile.fehbvm.com/Article/details/grbpdckuy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gfcwisvjm.sHtML


<!-- 参考信息 -->