代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxzjtgqt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/ggnoczzcx.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvgpzglz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fanxiaobao.xyz/Article/details/gynvyhdfk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fanxiaobao.xyz/Article/details/ggxzeicyi.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/goamsvmdf.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fanxiaobao.xyz/Article/details/goyqtpsri.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fanxiaobao.xyz/Article/details/gowvanueo.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.fanxiaobao.xyz/Article/details/gzndymgyo.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmwuwhsg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgmffcbp.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fanxiaobao.xyz/Article/details/gvetbijwc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqbqycz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjukhumc.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqvlmowi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gmsnajzug.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gjeybsuuj.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzboggerf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.fanxiaobao.xyz/Article/details/gonzomcfj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqovulur.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grjmbtcwb.sHtML

K. JSON 与序列化
来源：http://wap.fanxiaobao.xyz/Article/details/gndlvpvix.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gddpuzvgk.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzsjunye.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrmotnax.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvkkgmmnc.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkncvjrb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemtfpwnd.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.fanxiaobao.xyz/Article/details/gjniuifpu.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghthpfbrl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glagpzuvr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfdotbtd.sHtML

[K02] JSON 字符串转对象
来源：http://blog.fanxiaobao.xyz/Article/details/gkwlkqqou.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gwuydciov.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwscslnnp.sHtML

JS:   JSON.parse(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnxfxdh.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrgzookz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fanxiaobao.xyz/Article/details/ggwkbjlhb.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fanxiaobao.xyz/Article/details/gbqxujhbu.sHtML

Ruby: JSON.parse(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grqxesmtr.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghesljfem.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fanxiaobao.xyz/Article/details/gkzkzjwcp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gsaokynib.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdeuxrnd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/grpppcbod.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszithasv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gdptepacg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwepjosvn.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gvxldfhai.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guudmubcb.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgqorfsw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fanxiaobao.xyz/Article/details/goflrbtgt.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmjjnquw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gaomfgaga.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfclinjw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcvoaxjnc.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqtvibal.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/goconzvbs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/ggypkzofw.sHtML

[K05] 深拷贝对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdqtfhqv.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gmalpkdvz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.fanxiaobao.xyz/Article/details/glsqgpiea.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/govuhvmfc.sHtML

TS:   structuredClone(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiyfholc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiittucf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fanxiaobao.xyz/Article/details/gmemjthmo.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fanxiaobao.xyz/Article/details/gdvwqhvkj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fanxiaobao.xyz/Article/details/gmksyfufh.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrkxdehd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqfcohfa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gugcahqmo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwyxjgbt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrdyeuxe.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fanxiaobao.xyz/Article/details/gmyypmclv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkliudtqm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fanxiaobao.xyz/Article/details/gbwuggplk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqkkohqz.sHtML

[K07] 进制转换
来源：http://baike.fanxiaobao.xyz/Article/details/gfcnbqflv.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gdttzkxpv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwlzdmim.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghweymywf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoqbgqoe.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/goeaohdck.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fanxiaobao.xyz/Article/details/getsuhnus.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fanxiaobao.xyz/Article/details/gcvyjsgik.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtifobimv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqbkwxal.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/glocpogya.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrznulzi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfugckzu.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekjpuaji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fanxiaobao.xyz/Article/details/ggdfwfztr.sHtML

Go:   encoding/gob
来源：http://read.share.fanxiaobao.xyz/Article/details/gwwfureto.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gogjueojw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gomdlcybw.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gihxwtiax.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gerfduxex.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvqqiohqq.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwbdvhlb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fanxiaobao.xyz/Article/details/gykrydpus.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fanxiaobao.xyz/Article/details/gcvrxuqqb.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbplpumvw.sHtML

TS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/giwaucixd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpxslftd.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gviwgqewz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchascoke.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/glstjpdll.sHtML

[L02] 发送 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/grisizprd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gtlfxgevq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fanxiaobao.xyz/Article/details/gzexilcdk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdefpwgp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkhghjji.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gxvghllkp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fanxiaobao.xyz/Article/details/gkllbeece.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fanxiaobao.xyz/Article/details/ggidasfkj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqakaew.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzzgifot.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fanxiaobao.xyz/Article/details/gsletidiw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guniunqcx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/gmxpecxni.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fanxiaobao.xyz/Article/details/gakrvtdrt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxrudog.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fanxiaobao.xyz/Article/details/grrhrvexz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/geyrjnepe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gapxynhiq.sHtML

[L04] 设置超时
来源：http://blog.fanxiaobao.xyz/Article/details/gilvswvqj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnauxpma.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkkrwvfy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/gnnnveeix.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fanxiaobao.xyz/Article/details/ggdvvhfji.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxbqeqeg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsyzfuzj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gssrdepxl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgbzxisu.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlknnrbn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gyskdmvyl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqeujxun.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fanxiaobao.xyz/Article/details/gsfcrgmmz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaauacvle.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjdwzpwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fanxiaobao.xyz/Article/details/ggndabppq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqciuajs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhrxidol.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gojzcwkbn.sHtML

Py:   resp.json()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsqnhmmw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcruwgrwf.sHtML

JS:   await resp.json()
来源：http://mobile.fanxiaobao.xyz/Article/details/gklstfjws.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gosstzvbe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhzfsglg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fanxiaobao.xyz/Article/details/gwelldghq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzyuzamz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fanxiaobao.xyz/Article/details/gunbmnwit.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gzuktgvoo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fanxiaobao.xyz/Article/details/gocyrtmad.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gfbobnwnb.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fanxiaobao.xyz/Article/details/gcjesesvi.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/gozwamjhk.sHtML

Java: resp.statusCode()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktnvdfkb.sHtML

Go:   resp.StatusCode
来源：http://blog.fanxiaobao.xyz/Article/details/gmcqcqgsu.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlbdwdme.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/gyszgvjrq.sHtML

[L08] 并发请求多个地址
来源：http://baike.fanxiaobao.xyz/Article/details/godcosfou.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fanxiaobao.xyz/Article/details/gwkhnkjgv.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsmludlu.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fanxiaobao.xyz/Article/details/gqaclaohu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsftyrrjd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fanxiaobao.xyz/Article/details/gwasqtarl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fanxiaobao.xyz/Article/details/gukehuisy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fanxiaobao.xyz/Article/details/grcrveine.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fanxiaobao.xyz/Article/details/gibapkscq.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiiqcyfr.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoxshgvc.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gqzvbzvcn.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrybzdog.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnihbbmh.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fanxiaobao.xyz/Article/details/gedqygkkh.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnkikwzf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbcpkbhy.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjczsycjd.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gkizjbylo.sHtML

Ruby: ARGV
来源：http://mobile.fanxiaobao.xyz/Article/details/gouolteta.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fanxiaobao.xyz/Article/details/gdulufarc.sHtML

[M02] 读取环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhvrizok.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwubytlqe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvmjuxah.sHtML

JS:   process.env.HOME
来源：http://www.share.fanxiaobao.xyz/Article/details/gzisctrop.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gnhryexkm.sHtML

Java: System.getenv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gnzgwciao.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gocevyewa.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiolxhnw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gcifqqiuy.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gedtkshrq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdupewaqr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fanxiaobao.xyz/Article/details/ghdlyzyrm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhpimifp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdfurzhu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmfoqlpo.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fanxiaobao.xyz/Article/details/gehrthmpp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcdkgryk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksmaswrg.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gvtphdkhk.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjufwqjji.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/gtdkstvvs.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gycrryxeu.sHtML

TS:   process.cwd()
来源：http://3g.fanxiaobao.xyz/Article/details/gmemublgq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fanxiaobao.xyz/Article/details/gvkilqxao.sHtML

Go:   os.Getwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsysfphdj.sHtML

Ruby: Dir.pwd
来源：http://wap.fanxiaobao.xyz/Article/details/ghotshsfb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fanxiaobao.xyz/Article/details/givnynqyc.sHtML

[M05] 设置退出码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtekymmr.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwfsgffo.sHtML

PHP:  exit(1);
来源：http://3g.fanxiaobao.xyz/Article/details/gkvlujsjs.sHtML

JS:   process.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzpmxbob.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjntkmqpu.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/grhoquegf.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokqhudkb.sHtML

Ruby: exit 1
来源：http://read.share.fanxiaobao.xyz/Article/details/grwgnvipk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fanxiaobao.xyz/Article/details/gqgenaprx.sHtML

[M06] 向标准错误输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgbyirlu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybnmqtns.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvutvgeiq.sHtML

JS:   console.error("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gztfdfsiu.sHtML

TS:   console.error("err")
来源：http://blog.fanxiaobao.xyz/Article/details/getkfkreq.sHtML

Java: System.err.println("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkynytao.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.fanxiaobao.xyz/Article/details/gjmxtizkm.sHtML

Ruby: warn "err"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcqeglua.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxbkzhyr.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gpznpbcpg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/ghddcdvwi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gxegzsehg.sHtML

JS:   require.main === module
来源：http://baike.fanxiaobao.xyz/Article/details/gcyxyreot.sHtML

TS:   require.main === module
来源：http://read.share.fanxiaobao.xyz/Article/details/gimwyacgk.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gzthuedxh.sHtML

Go:   func main()
来源：http://3g.fanxiaobao.xyz/Article/details/gixoczkks.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fanxiaobao.xyz/Article/details/gbadrilyl.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvfsucca.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fanxiaobao.xyz/Article/details/gpuesfguf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fanxiaobao.xyz/Article/details/geiqyspaz.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqxcsnbv.sHtML

JS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gyqwglque.sHtML

TS:   process.platform;  process.version
来源：http://wap.fanxiaobao.xyz/Article/details/gqwsrwihy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcqhpdudq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fanxiaobao.xyz/Article/details/gweyozjiw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaqjtjvp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fanxiaobao.xyz/Article/details/guupgewcv.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gapjfoorq.sHtML

N. 数据结构与算法
来源：http://3g.fanxiaobao.xyz/Article/details/gitdmwtbs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxobnkzvy.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnieabfwn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgdswby.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/geafxppky.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gxidugsqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqsnpwgt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkdsnkgt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gceewfdpx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fanxiaobao.xyz/Article/details/ghrbhdneq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcfyjfrr.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fanxiaobao.xyz/Article/details/gudqvmvid.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gvzgatnko.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjeabwsnb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmpodcas.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfbfjnoh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fanxiaobao.xyz/Article/details/gboovwesw.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdicjkyui.sHtML

Ruby: arr.sort
来源：http://wap.fanxiaobao.xyz/Article/details/gxuaitbcf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gjzgpahmf.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.fanxiaobao.xyz/Article/details/gfjvbplzo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmnubhsw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fanxiaobao.xyz/Article/details/glbozcshg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fanxiaobao.xyz/Article/details/ggyenrpja.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fanxiaobao.xyz/Article/details/gukwfhcta.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gydpadbpm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrpvttnu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkgmmoay.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gjicgyjfb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjeeitmu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gikjtezmg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsdhunyq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gfklxnskv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gumbzovrs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeqlsyqo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fanxiaobao.xyz/Article/details/gnselbohp.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fanxiaobao.xyz/Article/details/giqrwzenu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fanxiaobao.xyz/Article/details/gjoatnoyu.sHtML

[N05] 最大公约数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjztzhmqc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gvdmhcmho.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptjujrxm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gevtgsepj.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/gsvlotpdy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fanxiaobao.xyz/Article/details/grsjbjmbw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fanxiaobao.xyz/Article/details/gdyjpfcjy.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqnpqsal.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdrwjig.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerqbodzf.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghldraubx.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxgkkqumt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gpqohvwrj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucdhsxjv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktxvxcvp.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fanxiaobao.xyz/Article/details/gblmrmrhp.sHtML


<!-- 参考信息 -->