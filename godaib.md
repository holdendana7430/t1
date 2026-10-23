代发 wailian999

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3mtyxfjvg.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ghqeguvk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3eobqzish.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3oqrjvkjr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3wgydisvi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3hdcegqby.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3jlimaxzx.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wygoolet.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3cssyuopz.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3jhwpikll.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3yfnvyjsi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3iscxmqqt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3hkskibcd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3psnqspzy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3uzugndyc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3rcangofq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3iqrpbhwc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3avrtfoth.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3ysnzqyix.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzrwadg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3agmnsxje.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3yxokxalx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3zjorinix.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3uzresxfl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3kvfvmpkc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3wqjodrlg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3bxzsivke.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3homvwero.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ozwtwzcl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3sgnczsac.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3swwfmtnt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unldrwcs.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3btwjmbsh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3iiplavpy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3okjxcvey.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3mhzqrbot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxafefmh.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3sjvfwukv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jatwriqe.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3olkaqdeq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjzfrui.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3otdpmvfj.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rphpthbp.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oiatosyc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pjwzbpgc.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3orfmkfaq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3yeiznkgw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wwphzrpb.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ywareili.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bndidoom.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zxnlzirz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eprkiktm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vxkcbrnz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3bnmgywpz.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jcailiwo.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkkiixj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gozdlrfq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ahpdgqce.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3wfgykbnc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3odivwosb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3teiqrmtg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgzwvgn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3upaeexzr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3klfczabm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3hcwxniez.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3yxgounju.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3kycnkcne.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3shvlslyb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3emfwdgie.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3dnefknvg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3jtzscyhw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3lncsiqfm.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3oobbtrrt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktjixokr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljovklzt.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3oyvxzusx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ofqyuitu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pukilytx.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nezzfzyx.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kimchdgr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zdntcqwk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3owdwxsjl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ydlayoxr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dtazqqor.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3krlbaqmm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gyczrfpy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3mlmleurd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tdpowfga.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mskrudji.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3avwypryb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3hriqpezy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wiifnrlg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3amvstjlp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3yeewgiof.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zethoaak.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3wgxuhktl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ojembsgd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xqwyxafg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ffvhtbic.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3kypwuxjp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vlqepxsa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pxveexym.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3pbhendqf.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ooxjjilr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ceeemval.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rlbfwmoy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zyebuzbh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hzcfcvtf.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jekmpfdg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3enjljbde.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3mwxlgkgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvpiyzsg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fnykbzcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdifxcsp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pwfsirbl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ufaswnnj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3sktwdyzj.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3gqihkvop.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3lvflttuf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3umokppxo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nwivtfix.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gkcednir.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzqtxhd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hhttavzn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3azqmfbhm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pjyxlcfu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jbnlanoj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3exromgov.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3zslionfc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mnihykys.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3wybhwwbg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gnepsupq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3hnexchaz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fjbtxsal.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ozewfoon.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3easckvkq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kychbwmm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3lgrfshik.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wanxdgwt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hthjqgcn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3flxhgwml.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3htytprrx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lsclndfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sinyrilp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wvfrbhfn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nornnwwt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3yqkvyyjx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3sdovgjwb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jumvjqwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mlohynpt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3cttjggwb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gdiecday.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qfjqhegi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3iunrsvce.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kfexjllv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3wleexvcf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3lohcfulu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3diviefto.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tzhxxgjc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nckkudgk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wdirzruy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhzzian.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rkhgqodb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lgbmuaok.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3szqobdwa.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3asquqwrh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lvtljmly.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nzxscpcn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3iqzbqxwn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3iuxbmfpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qztmuqri.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ovtobsjy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aawutwvi.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mnhduqvt.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tqybjmzj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3lvpchieh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hjnqjmfv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3syjgsiqy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ceiqdxng.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3exhedaln.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mhbscvan.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3babsrvza.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3yxxnbvvm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lrlihdli.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3binfwqam.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vlxgqhzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyehledl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3pxhgwqpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwatrrjf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zjexwwmk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lmcndgrh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zkftzjfl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gjhkylxx.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nsmjzokr.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3orrxqidi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3guqtoejw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3wsqkvuzp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cvhjmxjf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3enonpsbg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cqzflvvt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jwabohdv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3woikuybu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wetjfson.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3urmzkqcv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hsgklvpb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zlgacdrd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vxtzspsk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fekwykkz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bnczopwg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3krlzfywk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ediaxude.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3diuqvgky.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3miezejnt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nczudanv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rydriwho.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ikqeebjx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3trbilaam.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3whxaqbob.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3mgspjhnq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qjyzagcl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ykvyipjb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3aowzjqpw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3szrsbwgx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3fildbzkl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tfjjgmqm.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rdlpeysn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rgesxpmh.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3nllsrgjl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ssvpggtb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvwsktwv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yluhvxsx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itngdddd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dljlnbky.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wldtelan.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3oeoofkjn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qwkimiiv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3scboaisu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fickflvz.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xqxfkjlf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ogxzxqpq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3dtmjgjmg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bfwjguoj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3huqvuwhi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3saxhkxor.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qhjmwoop.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bqqnoeuz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ywmyuoqb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3evicjlay.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hxcafiqk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3ozbgpiot.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3aycyutnz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3owlrxykf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3pklqskna.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3rbrucinq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3dyajjbpb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3sxvaerni.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hepiapiy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3qcgxifui.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zauomxwo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3duulfivf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ktahftgl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxpdoieb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3patokibw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oasolqzd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ddfrlwrc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3prhfanwl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eooogwrn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zdgqnplc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ihqssdwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3skecpcoi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvfqsymp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kgrvagwv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ombfhwsd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3kcrhdqtd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zsdonjqd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jczodtjx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sfqwnutu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jdlbjtid.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jaaouhaq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xswdefsn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3kyaenfiv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lkwwogln.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3sowwavyi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ipoafint.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3plxpjyko.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ptcflvcs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3qcgsjbst.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qeygyksm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mowvpusw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3nrplafgl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qukaxlyd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3eogsgjap.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3toljiklu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqgaktuu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oxqkvsep.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pvhhbede.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ltalmpus.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3eagrarex.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tumuagkj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fajulwlu.html


<!-- 参考信息 -->