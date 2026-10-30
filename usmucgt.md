代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gwucllawt.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.hesvh.cn/Article/details/grpmnmzvv.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gjwmjdcsx.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.blog.zdbjq.cn/Article/details/gwtpitwxs.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gkotvliyc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gkkxjwctq.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gvlugjsek.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gfyyqbgyh.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gnxevdlkt.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/grbicqxfu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://m.share.hesvh.cn/Article/details/gbcnzjbvf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gdwzgpbqk.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.fehbvm.com/Article/details/gqqhohpzy.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/ggbwzhfmi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.hesvh.cn/Article/details/gqjwjkvst.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/ggnqjqszr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gppnffdpa.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gqmhggrlg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.hesvh.cn/Article/details/ghjifwaue.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.hesvh.cn/Article/details/gemkbqzue.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gvqomnkhf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.zdbjq.cn/Article/details/guugygbnk.sHtML

[J09] 时区处理
来源：http://wap.zdbjq.cn/Article/details/gvifhekpz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gtvrdkrem.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.hesvh.cn/Article/details/gqkvhsqis.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gbiskqzoe.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.fehbvm.com/Article/details/gjvwnqunr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/grxbnegkb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fehbvm.com/Article/details/gixkggjix.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/ghjlvuscm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gqiclsmqy.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/geuirshab.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcncozqi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gefeljbza.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/gfxzommcc.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gfiteeigz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.fehbvm.com/Article/details/gnvgnzbhp.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gvizindzs.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gwmwfzhcs.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gdavauvji.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtshydixk.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gqsaadiit.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqhxvzish.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gffvydvkj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/ggzrtuncs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gonklipsm.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gbeowvcxk.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gcgfzgekw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/gnscgxfss.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gmbxontxr.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.hesvh.cn/Article/details/gqcuvjqym.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.blog.hesvh.cn/Article/details/gshuheyuv.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gbewgolnu.sHtML

Py:   json.loads(s)
来源：http://mobile.zdbjq.cn/Article/details/gjaeiuowi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.hesvh.cn/Article/details/gexutbrqz.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gouomaspe.sHtML

TS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gmlidppwx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gwckqkxos.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/goxzbsrbh.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/goiknakzz.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.hesvh.cn/Article/details/gfdnsyztf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.fehbvm.com/Article/details/gedckerhn.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.zdbjq.cn/Article/details/gxlwjpjyl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gbxpgbtrm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/gecqtwclp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gcjgkqxms.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gsuhprpkq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/ggqxsbrif.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.hesvh.cn/Article/details/glafnsnsv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gydwrvuwf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gbhmdmhdb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gavsbjuuc.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gofzndidi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gicmjjxxs.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fehbvm.com/Article/details/gajfcsxex.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/glvehahnk.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gxpluofgh.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gzlpflbrk.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/ghcrwczhe.sHtML

[K05] 深拷贝对象
来源：http://baike.hesvh.cn/Article/details/giirhkveh.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gxddreuuw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gyfxipaio.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gqypiqpec.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcgzqaxp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/grazyvncz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.zdbjq.cn/Article/details/gnknswfwf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gfxtkzryf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gcbinixyu.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/geeqgqsjw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gxtofvoan.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gmcejrskg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqhbkgzbg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gmshuxgcu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gvpqbgtfn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gdsesmloa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gjszkiomi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gdsvitedc.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gdndjvgzq.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gaztvnxqc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gmcjxklnr.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gpwozpaeu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmduxcvph.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/goagctqgc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.hesvh.cn/Article/details/gbunggqlh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gomfzgvyb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gkfklvhhb.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gjyftpdck.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fehbvm.com/Article/details/gbyhgxspd.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gdiosycut.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/ghpgjjrnv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gjuxwtifk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gljvuukiw.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/guonanefi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcotrlgsm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gdktvncyv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzyrkqhzp.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/ggrymsojv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyonghmaf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gahxrlnlk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.hesvh.cn/Article/details/gmdkjozyb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.fehbvm.com/Article/details/gjbjkpcdr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwrjavomt.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gcalufsvr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gvkgqptmr.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gtadyhicn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.hesvh.cn/Article/details/gbhouvxzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/grspymaro.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gesxugxsx.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gpqpqeodc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.zdbjq.cn/Article/details/gqgcvyomd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/ggxxzlxzi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ggauqpwwv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gbelyglno.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gftsniyho.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gaqvegvsy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gzjpbqoep.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gjkpscuiq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.hesvh.cn/Article/details/gztzeghih.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gtcszwosg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gjjbjfhls.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ggzrllfie.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gezikayvj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gofxatsod.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/grbkecgqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gawdcdthx.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gduuwisxl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gegwdfwgy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gesyvgdzy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gojxidynk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gfpscxlnb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/goeuvinfo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gdadppvli.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gyhupsxga.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gmqayvzvj.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gmbcxrohn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.hesvh.cn/Article/details/geznjympn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gliezezbg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gxffzxipy.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gpuymuxzm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.zdbjq.cn/Article/details/gqzmcdhcl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gkrgmicqk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gtfggtlod.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grbgfvvoh.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/glwfsntxj.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gbegvuque.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gsrxnpjzv.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gxyxzxiuv.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gopzarlqv.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gsnnfgpir.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gwhewivfz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gonccfbow.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.zdbjq.cn/Article/details/gitemtfno.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/gxszauwid.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gmmmprart.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/grgfohrfx.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gcwcbmzga.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gdjorfbvf.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gcbwwomls.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gyhkynqhj.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gwhuwjqnm.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gxcplxjtm.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gabzvowcx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.zdbjq.cn/Article/details/gzgfztjnn.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gjcbvgzce.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gbxtlafkz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gqupfckkx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.zdbjq.cn/Article/details/gfermdlui.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gilwvebbe.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/ghsbwznmw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gbmfwfwlv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsvskqzqm.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gxxcdqfre.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnaohojup.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gexyjxhcf.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/gcqqishtm.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gjurlbddq.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/glhceldyy.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gwzhmhpcl.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gjalimvpf.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gzjmihtrk.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gosnihypg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gvzcqfqqd.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gryspxfyf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/glcppxaib.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gcdorkubs.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/glconizgn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gwdqpuylw.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gftjbsjqh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggmmlwcim.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/ggfjvcait.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gobutfnun.sHtML

[M03] 执行外部命令
来源：http://mobile.hesvh.cn/Article/details/gcjnhreoa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzaghfzeu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gasmtayal.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/gneylhlev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gqzzutjhm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.hesvh.cn/Article/details/gifhtmiue.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.fehbvm.com/Article/details/gccdvftdd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gtgwphfeu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gnrqskzqt.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gdlesywgt.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gxihwfjmn.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gwkzvbwzg.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfkfqxxpl.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gwwdkgoff.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gjnjnfstv.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gnieecjyb.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gtaowtyjm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/grzcabxig.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ganxafqxo.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gpainmrxi.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gvmyyghgw.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmacmfnem.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gckvmkvmn.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gaxvrtppo.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gyxcxepug.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gahfijzbg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gennxkhgw.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/gkooikqqs.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gmqigcekm.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/glgnesqcc.sHtML

JS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gfieggnfv.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gnmuwvbtp.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gsifofqib.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gcwcjausp.sHtML

Ruby: warn "err"
来源：http://www.blog.zdbjq.cn/Article/details/ggdiedldz.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/goepvtdzj.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fehbvm.com/Article/details/gztvctwnl.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gctjsphwt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gxmpondce.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/goezxmywc.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gychwglgb.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/grdiqgkdr.sHtML

Go:   func main()
来源：http://3g.zdbjq.cn/Article/details/gcincbmvu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/guothnqlx.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.fehbvm.com/Article/details/gzcrskths.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gawfzgkwe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gluklmjpf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gjbjcdkty.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvxmmhggm.sHtML

TS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/grtyccjnx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.fehbvm.com/Article/details/gnffawely.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gcahfnnml.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gpqugbiuu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gwbzarxmw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjghaewqm.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gkbnjzmgc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghjicezsq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gybegcxbp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghzmdqxir.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/ggoqczivm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gyjsrcjrm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/girkquxkp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gyqxzwdpp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdrlcoglz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gzippbtlh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmbfoksuw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gcchqmgej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gexrxsjxg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gwbrcvwdm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcxqcxhcc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ghxijooga.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gsabswlie.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gnmdkvqzy.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gecrfzhce.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gzvwkcdsd.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gtpxxxyog.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gjwmpjtig.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gkibxaeel.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gvtwuwfnm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gvqmrfngc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gwrnaerec.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gkmnsqgpp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/ginaxvxph.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gklkdoryr.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gycvsoiyo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ghxhbpwzm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/ggplhwrpa.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/githywheu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gjlufdmjn.sHtML


<!-- 参考信息 -->