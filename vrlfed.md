代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2cvbmoamx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2scrdinss.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2bkexofms.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2aihegism.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2xulifpsn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2efhjceja.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2kroxseno.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2wlvuquhm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2vytjegyc.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2aefiaxhy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2dfqrvmbf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2xogshjag.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2vnmhrmao.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2gonxyrac.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2pmilfxpo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2nqjfsvoj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2zixisjqk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jymgvzyo.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2qbfwymur.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrrzqqg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2rhdcdxwd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iojtygsx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wgwqyvjx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dlastute.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2shjzdibp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2iunvhmvz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2mhsszbvv.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2tmettgaj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2wuszvbzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ritolbck.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2xqjvlzbq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qqokxzcy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2uaryidpk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2xwzbqgew.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kgruurwe.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2moptzxtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bixfqubb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2yspaulrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nccxjqgi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2hbfdppzv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qlakexgw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fqwujekr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2joxywozx.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyldssj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vhrvfnyt.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zicnwegs.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2wwzilckw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2drkraffv.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2xoovtoxi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oaeluxjz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2wmqnlrgd.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2heonposr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vtdoklgs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmwqhrq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2jpdstpfe.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2jbcflase.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlgezocc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ikkgjpca.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2rtlypzch.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2jwjefiby.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2narxzpbu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2gkqiwifc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fxobxyvt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2gjwvydrn.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ysaqotij.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2mqoqztpf.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2bniptimu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vpzldgvx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2dvzwooul.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2blfsfzle.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2atfveoox.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ujxstave.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mmpykrnf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wuriwqcd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wjuvyoxw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jzivkijj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2berkykfn.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2mmhoeitd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zfcwykqn.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2itpxetxe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2rrcgnkxx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ovcdalqe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2fymqwgzl.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dxkbpxkm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2sgndlaih.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ysyesxol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2rbzruhzq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qjigdhqy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lgnfggzl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cmmosrir.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2gxyoxxke.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2phreydiv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uaqltrwp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xylcwcdc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ucqaluqw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2hwbnnajk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cwqgqrxy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gvlobjzf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2knraoevt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2riivntmf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2dswuljiq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ygwwqftd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2evfvkuzm.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghhljiin.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ispnotzs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2kcayffbi.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2dznryclx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2asbbiyij.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2nkbvpaoz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqndkti.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mnjlnlks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzedudsb.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2hvldhmvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yreqtfzf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cjzptlii.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2lsjdnzqp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjvbmc.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2acyawqqv.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2edjgaypo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lthnbcax.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgmlqic.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xfptmcdg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ubikaitu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zuqsjznk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2osuweowo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2havwygfx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2oofwmwzj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zpqwsegx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2xgrejwnm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2wgjltupj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2nzntpsqy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2huvmxrxy.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2fqhndxwr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ngrhstmg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eufruamk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2lqrjuhgj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vvwdbcdz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ldaqpjlm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zgecwloc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2sdnthsbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kxlhplha.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2velxfdtp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcciiom.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2xfttidch.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tdxthknd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2oqrrqjny.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2jszonyzm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2aruchele.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2omejjfrh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zydfunvk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2lydzgqyv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qkzcnufx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2cadwcbmd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ttpwbzgi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2eohbgvth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2csfilfxf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2fezytkaj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2oyazxvgy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2efdmlqsg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2marcdido.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xswdbnwh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2osmebwsc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2vwwmrxmt.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gfyftvxl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bgrogrje.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2jndxinus.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ezjcrpdu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2cpdnxyku.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ldhwkeob.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2dmrcsrxw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2rspojmkk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zilvnfja.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sbsndpfc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xyjnsark.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wfmqrbze.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zfqkpqmm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pkvywwbt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2kjzpxynh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2egixgjjp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2cqjvfina.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tezuzbkn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xwckvpzn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dvjnuhfi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2owccvksy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vgikwqwf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xprqafke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zaxhpjrn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hxscrgvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lizthrtk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2eljgpkeh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2urudarsl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2fofylapb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvcygks.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2raxxxohh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cmuhicvd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gaarorhp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2bkysaznz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2amqciirl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecbolbbt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2inipvrlx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gecmzwct.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cbxsiifd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2iavqlijp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zavwhvai.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2weovzeud.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2etdxbuhn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xqvtmkgk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2hltpdmli.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kniuxakh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ytspjlpm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vdolbqxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2owhsionf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pqybfhxa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2clsawesm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xhgtmtkx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iqvkcnts.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gadyfeyx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fwugzbks.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2bfivhqok.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2orcxvsid.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pdfergxe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2juemplwq.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bqmxmogd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fluqogmx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2cmsvseuz.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2epxrpqsj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jmarpajb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfrnyec.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqqmpbuh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcffmxv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxqmpsyy.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2domtbppk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vgmfvhpn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ogpcgtkc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dmuhtqof.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kpmcxrga.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fpestpne.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pgpwnxks.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fnjijgxk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dfmvhuhj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wuqfkamb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dnnkhsfy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uwjupzru.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qpcefkqo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fhgzprnp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2cplwbfin.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ggsfbdzd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2utgkklik.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2abymvovz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2berwvaev.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xjygjcek.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bkusbpqw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gfahkfvc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2oaudogvj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zvsddlxx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cvrjemvg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mbcabrrj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2agafhcgn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ozwkuckj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ojwbrerj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2msifffgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zbdnqocf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ptaifxcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwundbzo.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pmlyhecj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkzcapon.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bsrpaeuw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dezajzix.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bmrqygmk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkoflnvl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vemcmcgf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yfyfffzh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lslwhoxk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2fduwyilz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pngwqcjh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2rnaletsv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vbrhgdff.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2osfuqcdi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wirdaaie.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yffxlftr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ilbwrolj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2wecetshl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2quphgimv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xzilrncg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2noqngiqj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cxmbjcjq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2xldwotpc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2zztzwyoq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2oecrhfbe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dmnzuwgb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2bvluualo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bvambckq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iaztamzo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwlmpyhj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzezeasg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aibjrxkq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2sqvechlv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlnjswwm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ybgqnwue.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sdlytxer.html


<!-- 参考信息 -->