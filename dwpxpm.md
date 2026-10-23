代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3uruvtgmc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3egapnuxw.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ayxdgmky.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3nzmbopmi.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3ephuhhvu.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oiwoiqfj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kmslytjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3daowxcbm.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3truxkxaw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3aasmyyev.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ttcypcoc.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3alezebsg.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3tguqkbhr.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3uvfyjthd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3yqyihwcs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3ojpvwahu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3krzqjdew.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3tfkfgiun.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ssqpqbof.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3rlckrhbw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3egmjjjuy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3upskfltd.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3aejtfdtd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3volijoub.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3phjeaeva.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bzwqqrpi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tjpabktx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3tslnispb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3unbmhttb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3vyzrvhvm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3axngymmo.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3njiodmie.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3qayonvlw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3lemafifp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sdifedgi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3plweikrt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3nrhpzmst.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3lnprodde.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3oxcbmvkl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrefapya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygzpndkb.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3lcghdfqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3advmxglp.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3memnasei.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3qrserxee.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3dwilxjln.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3oawrvhzc.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3kevgjpff.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vzqrbvrt.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nepdoffw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3dmacslrr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cqijnkno.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3rumjjrvx.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fpxflbze.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dwkgqyzw.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pdbzkvfo.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pjawgcmx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ljmsfgqb.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ialpuckp.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3sxvgcpmi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjowehis.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3ovdabfsr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3madoarsf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zkwwczyr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3pwbmxtzg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vichlsww.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdnjdal.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3rerifetw.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3vcxudgkg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3reqwazwu.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3ntiiihxd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3hdjroxwk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ijrioccs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovemkprh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3sgcsocgi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbjoyrk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3hklttpky.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3swruuqkx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3iivcgtqu.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rlwpzaky.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3zcxsjnlw.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3xvifofii.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kmouprgs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bpyjfvmx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3ydzhirpc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3aicgonum.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3ardnyfuh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dtbfhhvm.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3cijnqrcp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3gofrjaox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3ssmikcld.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fqruseli.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sqokdpps.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lxbkhovl.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nowwbckw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3qqiadqeo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xrdzezaa.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcrjexyd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pmbpgkbg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zqniamma.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xgpqwigt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3waqqcisu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ywqwtmli.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3huigcrrp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3eiwyebrc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rhxgrgyv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3crtizeew.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxfpyfd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wwwupjwn.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ljdysqre.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3viemvpym.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3hbcclsel.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mswlvnpz.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xmcferyh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hpxlfhhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fotvsqgl.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3eyeyvlqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmyyghxc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uvpwmkmr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3xjckydaw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3viypmfsb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ynmuungi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tucquqjn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3zfxvlztz.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vpykszid.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3oswkmfao.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ofkmnwoc.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ysiaxfea.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xjsdpekn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lxijfzgm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hckwwkph.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rmfxsreq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3crnooxha.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3wuwxnxmt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bsvljyut.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3gbeijebo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ucsvjiym.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bsybqfwe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3jmdzmfra.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3melkgann.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pvjyqyms.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bwmhioia.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3axudihup.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ywkbdioq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fqcwodub.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3hdrybnsj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3netvslvq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhrshmw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aamsvtqv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vrljoaor.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wkyliswd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wmgpyjcd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mvcndkdn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jdxbigra.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmkvkh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hyahrxpf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3odnesiof.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bfyveygv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3jhwzlipz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3fphdwzmn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uzqdqfgx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3mcvrbaaq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hbcuglfh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3hqrfrrbq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3brdguqkb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3szmhemeh.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jfofzzhf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3fnqbkrmp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3aasfjpow.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gglqihqp.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3zhctwftt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ptcwmwyx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ihdxfwvb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3wpsxlntx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wqzpmjnc.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ullbvest.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gnfcsfdf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3crfpsadx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3eqcbclmu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jplojllv.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nupwmnkz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mwtoxnbi.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3figsmtxo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3umnfzmxy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vuilxhph.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bckujrgs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ahqhinec.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3fxinzrjz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fvgyafay.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ndedoeme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxmcxtrf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lnzbuwhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oinfhvvl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jxsienxg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tioejasm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3jdgrutux.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ckfiumxo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3jkckcbcn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yhebftxu.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tpnkqvhb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qqbgaljm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3krepruub.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xctpvwyb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3knkrpoht.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3aplmmdcs.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3bbhrtdbw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3idnaeftm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zumuwfvc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aqngsibc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vqzdolgw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xkovdqbi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3pqdpvrmp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fjesqasg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3woccvwen.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3mottaqiu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iqmalgyt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3lblczquq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dwkbpgma.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lxixqsdj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ddqrqpck.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3thhyurie.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3wlqrxunm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qhyqvele.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3eesxhuba.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3htobzbvv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fiyelwap.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hnopfoua.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ymytgsza.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3pslkjkqg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3fklxxosk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhcxhgip.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3bbbbwojt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hlchlyue.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rffirbrg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sijbtpca.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rjcfpkun.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3masdejvx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cotzvnhi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3knhsxhpg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3pyiogwme.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tquviusi.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lfesqewg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dvnuanfj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3prmzzhnn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3hntybsqr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3zutenpzq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oiidzjbp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3cttmoheg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sfeqzeiq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3wjwwkhos.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ugqslzjf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tbbrawgh.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nuacsdpu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qyviwekt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3jrbzbqhh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vpgjwirz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3xrknnntv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bieqdbzw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cfnyttdc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3epnsuxwa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qeipajmo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jkuyenok.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qompxjcp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3psrovjhi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ltbjnqcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enxlteme.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3hlmqvbfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vgwfprds.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3axuocbws.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdgjehdw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bvgtcrpb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xjznpbvh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ytsyamny.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjswnpvx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyiaaghn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tqcsotca.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlriyyuc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3abiafakx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3imktiipq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3koucmzgq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sdiwcsdg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tjzogjoi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ocezsxlm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zcszsibb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lflvkgyg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zhyouywh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3plvagwbm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3oslgswse.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3mybandnc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bhialjfg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pbjqgrdh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fsvisriq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3vhqsknep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gydmsige.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3adbfmoys.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3ybhutaek.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3iorseykv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ljhtiqbr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bxjhxmew.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wbyphvrw.html


<!-- 参考信息 -->