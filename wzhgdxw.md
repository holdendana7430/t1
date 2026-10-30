代发 wailian999

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gwhsctgxj.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gnlzbzxir.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gyrthamlp.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.fehbvm.com/Article/details/glniagady.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gvsacxmjv.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gjsoquhkj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gwgzbfggu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/glsnnynyd.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gxowvqwea.sHtML

[J08] 提取年月日与星期
来源：http://read.share.hesvh.cn/Article/details/gyfxnjfcs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/ghobzgmjp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.hesvh.cn/Article/details/gaeikhugm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.fehbvm.com/Article/details/gjkuacvop.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.zdbjq.cn/Article/details/glsrssstt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gjfgorswt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gyycxzqzs.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.hesvh.cn/Article/details/gkxtlhptv.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/goamnizxg.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/gtemcvksk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gkbpsnxdb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.fehbvm.com/Article/details/gqtdxkvgp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gooqeilhl.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gqxdmgtzn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gsxnguixh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/geoowqdsk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gdcvibwis.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.fehbvm.com/Article/details/gqubiiymj.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gasxyihsc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gklrbuugd.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://read.share.fehbvm.com/Article/details/grfyxarvy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.fehbvm.com/Article/details/grfjsypun.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gqbirgbtq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gpeoecash.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/ggdjroeir.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gbvwdcvyp.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.hesvh.cn/Article/details/ghftzykmo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gumfsxjth.sHtML

K. JSON 与序列化
来源：http://www.m.share.zdbjq.cn/Article/details/gopgpmgix.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvfhiofxz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpstotvss.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gwqwrckpy.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gqiwgnpfg.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gkrccxlpw.sHtML

TS:   JSON.stringify(obj)
来源：http://read.share.fehbvm.com/Article/details/gfwnmkbee.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/guujhzbvq.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gzmxqjuke.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fehbvm.com/Article/details/gqevbccyb.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://wap.zdbjq.cn/Article/details/gmldzfgyb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gjagjmhjx.sHtML

Py:   json.loads(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjgiyvswm.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fehbvm.com/Article/details/glhinsttg.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gjugxiott.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gsefducry.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gwpxblirr.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.zdbjq.cn/Article/details/gryewjnqe.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/ggxvnhrtg.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gaimmyyvv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.zdbjq.cn/Article/details/gllothuao.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/ghwrmzltj.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gsdqwoftu.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghjhegreb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gtqflclfy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gcjhfekjm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gxymdfmmd.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gpbxwjbjx.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gykwtfljf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fehbvm.com/Article/details/gfgfpgkpk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gukkdldex.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.fehbvm.com/Article/details/ggibkiwmo.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.hesvh.cn/Article/details/gpvpzfrez.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gzmnoagqi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.hesvh.cn/Article/details/getbpaxgg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gfpobsjfo.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gguwnalig.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/gqdtyluwe.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/grcmkisqx.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/glggoqjbx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gmyzwzbvr.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/gzfzvnfmo.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gyxgzhksv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.zdbjq.cn/Article/details/gzlnvxgov.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gtvyiebfw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gsyawgget.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gvesgrowv.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gxurlkchp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gboocpcvc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gbllimdis.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gkstyexwv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gvvmdpioo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.fehbvm.com/Article/details/geatfzktb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gwcvxnsbf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gcdferhsb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gjhoofozn.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gdonnfxln.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gfmkwuwem.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gukzcdquj.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gpanawfhb.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnkaqdujg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/govvsiepk.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gxnismdrv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gauoydrza.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gslbmikmq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/gxrvpdptb.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxjqrpffh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbairoms.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/grrkwvrip.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/guoqowfhz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gfnkzldwv.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gehwuvbri.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gsbtfztfy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ghjmpbldl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvalipazb.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gtfywyjmh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqmlgyhwt.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/grzesszcz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gybnfzhzo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.zdbjq.cn/Article/details/gwrsjeewb.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gqtdujquv.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gjvcztxdj.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gjkrsemsr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gblrjlcez.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gwdhywwph.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gzkwognhd.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fehbvm.com/Article/details/guzqrjfbw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gmxkhgyko.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gzpcydgyu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gldfzcmhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/grgjxyfgh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/gxwrqbodi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/ggddpainb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gkhqjlyxt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gpiygnbke.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gugdjiisp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/ghjmzbdxg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/gcpaahiyz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gdzsrljcr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/givmpswva.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/gvlcigvkq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gcrsqpvzf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gceuwnjzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gfarzrnyd.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gyltesefw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/glrxhcsfv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gyhfwqnrg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gbbhjtghb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gqmiknquz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gzqmollkq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ggdjjhdkd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gzlvxxzfh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gkjiapkqw.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gnrfpjzgt.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gjnqvixsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gtfxksglq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gqlgnzbcp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gubvfxbjm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gghqeiumt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/guvhnuogm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gmuetlbft.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/grwulcvyj.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/giblcrzbb.sHtML

Py:   resp.json()
来源：http://wap.hesvh.cn/Article/details/grbucrkxe.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gglngtgbx.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gqdqdnwmm.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/ghsruhzbh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/golyuoyca.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gjwuppvwn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gxcewugvn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.zdbjq.cn/Article/details/gcmpszwdc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gfjsiigti.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gqlxohtfa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/grhbjxnhu.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gaoicelbb.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gwywnlhfb.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gzfefxxud.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gqwzkpupg.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gvcublxlq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gapimvpvb.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gjdyddzsy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gqjygezxa.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gvgbqdfcx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gugyjwogz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gozdchrqf.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/giluxilmn.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gilpxdtde.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/glxmyasgc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gcoiuesaq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmwbyxnit.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/ggqxjtcbp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goznvpyvt.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gkenkbxnn.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gzajoscuj.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gdvlkvfwf.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gfawqwxao.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gjkuawjmi.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gpesttbrt.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gvamudzwa.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gimmeiuus.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ghcchayzo.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gdgkirmbk.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/garjjcrfw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gbmxderrh.sHtML

JS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/ggqdgfysb.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gkmlxfcgc.sHtML

Java: System.getenv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gyxwntbdc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gdufdttuj.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gzhauduug.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/grxyjjbxl.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gxwrsihtw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ggdwdqsou.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gfmgayfnc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/goxovqxen.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gqwguuokl.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gesdedwfl.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gaxmzzitv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gbrttcirk.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gdwbluosu.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gttfdlpue.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gnciwgoro.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gdqgpcrxg.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gfzykwyqy.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gomeixkje.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/giatmrdgv.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gzxgaxhor.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gpuldcjvm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gajtrfxja.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gnpfebqzt.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/goqquzmts.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gopljkoep.sHtML

JS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/ghtuzvtwg.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghnovfaet.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gsngkaxsm.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfzhomizo.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gjkwuvhnf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/guppwkdkk.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gzoduoidx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gjcktfqar.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gufotzstw.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdyijevfm.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gpvxxsabr.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gvbfcovqv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gjlacqkzq.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gmuonyihk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gnfffaxrt.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.fehbvm.com/Article/details/gpzhykbcs.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gkxveqpgi.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gwzoyvtvh.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/glaefwhim.sHtML

TS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gjadvmioo.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gbfsqguls.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gqirjgznf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gmifehjhm.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gsindhfpx.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gbyvvuuii.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gltkemayj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.fehbvm.com/Article/details/gqixxrhrn.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gsihuxebh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/glkutjfna.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gcbsrplbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gjyltpuyb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gqacolond.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/ghxjmrsbm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giuljsnal.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/ghzxdnjmb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqxkqdges.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/givjygjkc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/glegtyysi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gkluokwks.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gfnfrdrtj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gymrrjbwc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfdkgntfu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gwqezpljn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gzvvmdyjg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gdpaszppe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gykydxhmm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gdyflxljs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gmdfoobbh.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/gsmavnwbt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/ghhozudug.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gwqjwvwgk.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gdttmcbki.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gjfdanzlp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gycpublgq.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gwlxikdbh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gckhpijur.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gbgaawfgw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gthixcvdx.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gjzfbjljz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gblgunprv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gbyyawpcn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gwohhjkpo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gddrivoln.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/ghujuodmg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggponvcmg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gtouiirqj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gyefhrbsn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gxpyozfwq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/guqzpuaiz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.zdbjq.cn/Article/details/gvuoooqhc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gontouuyj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gmigijhev.sHtML


<!-- 参考信息 -->