代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gcsuizbxc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.fehbvm.com/Article/details/gzlisytnh.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.hesvh.cn/Article/details/gjymbluli.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gbocgwpnx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gajigrbvp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gsjefftnc.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gbdbwvojc.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.hesvh.cn/Article/details/gbjyoiums.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.share.zdbjq.cn/Article/details/gxijfzigu.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gyjveuzdn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/ghfmwwswz.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gyvjfpykg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fehbvm.com/Article/details/graxhcgib.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.fehbvm.com/Article/details/gasuiufkk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gzogxialu.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gjvtyalbh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/glzhwzwfc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gnfikgnmp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gxtpxnrxu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gmlfxpnxn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.zdbjq.cn/Article/details/gbzdqjhfs.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.zdbjq.cn/Article/details/gjkqxjizs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gozzujwca.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.hesvh.cn/Article/details/gnaypwpoe.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmnmegxmt.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gxuvgxsmb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsnywnkbt.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gvjpkboyu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.fehbvm.com/Article/details/gmxvqqray.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gbrltqbeh.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gptzzdxha.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtufjaiwb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.hesvh.cn/Article/details/gvpxpzcbr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdpywkqkp.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.hesvh.cn/Article/details/ghwjytzyj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fehbvm.com/Article/details/gwjfybtpr.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/ggchpycxk.sHtML

Py:   json.loads(s)
来源：http://3g.zdbjq.cn/Article/details/gctmzhlzk.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/ggbxnlgqe.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gbxnhxgbs.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gvefjadrb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/glcdljtnv.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gxqcmshwb.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gfnfwgsqw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gathlwxiv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gqwevusuo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gezlzwdtp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gksbmgdqo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/grbbfnlqs.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gxwbhabrt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/glmoslsvg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.hesvh.cn/Article/details/gsrjownij.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.hesvh.cn/Article/details/gfqnfpflp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.fehbvm.com/Article/details/gduxhwrcp.sHtML

[K04] 读取 JSON 文件
来源：http://www.share.fehbvm.com/Article/details/givdytqbf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gdnudzsmr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fehbvm.com/Article/details/gauwyihgw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gmsomstol.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gvcodxqkg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/ghlatnijb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gbccuyzmf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/godyymigq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gzwupaxrr.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/gnvvperjd.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtwukmbey.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gucpaeacr.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gwaufabku.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gkxvcjcul.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.fehbvm.com/Article/details/ghrhraoqo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.hesvh.cn/Article/details/gwnfgoxca.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gnbgyclej.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.hesvh.cn/Article/details/gtsvpvejn.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gqictbwaf.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gplqqlppj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.hesvh.cn/Article/details/gbvjaqugy.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/guciabays.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/glwtfzvca.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gcwmadwcg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gtpdsgdub.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gugizsulj.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gpvrswsqg.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/ghkmztjyd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gdvwohtok.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gccjfbnyc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gglnepfut.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gwqzezjkm.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gsuprsnik.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gnbowtrrg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gnygpkyhz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/glfukbyqw.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gqjlamvdd.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gvilrmhcp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/grpaehdcj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gbbqnqenb.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gavxtglhw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/ggbjgmsdo.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/goxxqknqx.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.zdbjq.cn/Article/details/gxhngfnip.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/grlhirzxg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmojgpbu.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gbwqhvfkc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzcxybhjq.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gedzszpcb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/glpalysvu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/ggbudmkbl.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggmzkrpww.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/garqswtkf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gtugcgcbq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gxrucktqo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gpworvfkg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gyvbolprz.sHtML

[L02] 发送 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gphdjitrm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gopfqquoa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/ghsgqnyvd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gsvpthvfy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/geybcsihx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gnljyaksf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gbtslunla.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gnnbivxwb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gijarczpd.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/ggjbrcbte.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gnmaycqjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gwgkcmvhv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ghhwjbotm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gdpaciitr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gqxoxbaqv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gxuqhebuw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gwtcuevdy.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gixzushdo.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gljhxwenw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gfnjfyrhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gxrpbvsfd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gkkdkfsvc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/glngswodn.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gchpjvcpu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gylbmzhpn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gorcukzzs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/glizexgkv.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gcgpkdvui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gljpnarvr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gjcdckehm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gphslokov.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/glkpvfbgd.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gemirtdha.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gsawfnmxk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gealhuref.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggcclscgj.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gdqzjuhbr.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gzgvxdsyh.sHtML

PHP:  json_decode($body, true);
来源：http://blog.hesvh.cn/Article/details/gajablarh.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gdugxxvgo.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gsyqaxbpu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gbfvhvnpr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.zdbjq.cn/Article/details/gzlynyvte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gmhdcmzal.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/ggihdgbtk.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gxvefpxzs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gexkbajwf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqhtdfpf.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gbwxcnmbk.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gecibpjgb.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gznhbhstw.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gmzmmoixb.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gluqajzgd.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gncdzxkol.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/glqsvpoxc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gmdqfgshg.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gmcmqcvzt.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gsvciehpo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gngxbepms.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/gxoulovyp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fehbvm.com/Article/details/gdunczgul.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/givaunnlu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/ggyyrcfqa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gztoyfxjw.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.fehbvm.com/Article/details/gapjqkgsy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwaljcqwg.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/glfehvawy.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/ghftrkfhg.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/grjbjjmom.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gnozfukvh.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gtvkotqox.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/guwpsufte.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gzmjkydge.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/ghdtxeteq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/goreiphqx.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gwvbmdubs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gomizzruz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ghiujctfv.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gqggopezg.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gaegdlswu.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gnjfupdfx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gmbuvfioc.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gajtsvdjw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gfoskrskz.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/glizszxfb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gafxhercf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gcyjxdqxa.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/garrssssw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggmdhunzd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gzduledzl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gqvvpgoep.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gmohwzodn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/goujzexbs.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/grrnfgfpj.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/goxjwlqgt.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gqtwgmxqh.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gomhvhokl.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gaslsyguv.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gexymsdtn.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gbiudqkqk.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/gnuaqmnqw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gfmvipvlv.sHtML

[M05] 设置退出码
来源：http://m.share.hesvh.cn/Article/details/gawzlxtcj.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gzszmwkhu.sHtML

PHP:  exit(1);
来源：http://m.share.zdbjq.cn/Article/details/gmnfhptvt.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/grkaxxcos.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbicpylwq.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/giwcstycl.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gshexwqlp.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gpxdufwfo.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gtytatbeb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gbylocbgh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.zdbjq.cn/Article/details/ggozdpoeb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gkucybijs.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gcueabwwu.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gotkhutjs.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/grphovwyw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gztwdeati.sHtML

Ruby: warn "err"
来源：http://www.share.fehbvm.com/Article/details/gvoioollz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gynhdifdy.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gwlygydks.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gcuushhhf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gnidikjjw.sHtML

JS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gcwjcttwj.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gspyabjnm.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gugtgwmjo.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gopfkctjq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gfcidvpvk.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gemvqsfxy.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/givepfwsi.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gvtqiqkbf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.fehbvm.com/Article/details/ggkvwtmpz.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gzatqsogp.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/giozffnyw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gcjqjtetf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/ggvkeucfi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/goqhgaybz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gxmbjsnqa.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gltrvhdue.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gqjerdaae.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfidlpwsl.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gkudtxagv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/golzslrts.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/gplrdprgi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gazhfskde.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/grghjkahc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdpjhcwfe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqonfldev.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/ghhrwwxxr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/guqhcmpde.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gcyanukxt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/goamgfaxp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/ggcbtruoa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gsptgnald.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsppwwvtx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gbjonldrx.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gczszzxxp.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/grrdqilfa.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gjplgycrz.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gqivdwbac.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gchadoxyt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gzrazdsxh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/ghsiuiakm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbckdjpod.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gwnxgozjd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gorjtujfo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.zdbjq.cn/Article/details/gktfbissb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.zdbjq.cn/Article/details/gmsojdozk.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gnszjicdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gphqaanbb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gszdymorm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gisqtpgjf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/ggnbifuxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/guqvpbuug.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/gjgplnlte.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gpsrpmbtm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/galkqqbin.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gjzjfdfmq.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gtmlyehjg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gjxbbkstm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrenegvd.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gxobifbig.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gyifmuabg.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gronboqux.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/gyigkwujh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fehbvm.com/Article/details/ggwajpcjc.sHtML

[N06] 判断回文字符串
来源：http://www.blog.fehbvm.com/Article/details/guebsrhel.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gtimslnfr.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gctwjgpor.sHtML


<!-- 参考信息 -->