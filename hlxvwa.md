代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3sskvjqbq.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3frzztwmr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3eyfttwjx.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3vzqybyoy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3dgeinstn.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3plrazjzf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3amzztmka.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3qhfrnlka.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3lzamvxjx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ktykwaza.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3qlnmipcl.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wiyqcxnr.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ihqehppp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3fvnktiip.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3umvwvnzr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3flslbccy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3fnrklism.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3fxpvlqav.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dewdfasq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3akucstsr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3epobcmrd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gskawqmd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3yjbkpepg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3imjozknh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3kqvxawpm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3czdjtvjm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3gxiunpfl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3auyvtvua.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3mzsrbugo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3yoavahpw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3clxfupkp.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3anxcbyvx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3gmafgvld.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3jpmtxycl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dklgkueg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3hmhfmbhn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3dondxrxn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3dfwenmpg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3gouqlixx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yftzdski.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfrpmzsm.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3ftwzykoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rghtyepx.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3cmwgloib.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ioxnphvu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lsjohurx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3mkkbskho.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3iccmbsep.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3kpkympgj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xkowrlha.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3cdnejlpx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3hxihdxed.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3qlsjhojg.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bfuzoygt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3wcjcvzku.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3rizmfxtm.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtqdcskt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ajmsyqsu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3gyoiulrs.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3uildxvzt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3nsexdtsx.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tjonvudl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3vmmbiwhz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3divymsei.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zeokbyra.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qveaugyj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3iqyyfclw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3avbdjnfg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3rhqdkbtw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gmlepacq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfofiyrl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3trarhbwr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3uiqglkzg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3rizsjfxg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3wnaudqai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vwnwfzbo.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3ybhenunf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3empvyxlj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3zptcopny.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3ihzzbwrs.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ypjhxzkl.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3ufvisyxc.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3cezsbtfi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3artqndqe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3rzmecefi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3tssbuhvt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3lhgjpozi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3etjouyee.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jlyngmyk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wetgmylz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3lxyvdohy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3mblvxpcl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fbckxvrz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lnsmnzmg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tddatpzi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mmglncwk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lkjhujou.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3eftxbmoh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3vexwgllr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3eymyulld.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvomtnvw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jglkxhuy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3bcsoskmt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dkoorpra.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwftawa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ipflgwpq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3akevvfuq.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ljlihqax.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rivlmuoq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cronowcx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3axdssord.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zczmuuro.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qczfurdr.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvcxaqt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3olrewasw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrqfuyxw.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3skxnjbsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkymzteo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3klgepnml.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jfgkconj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3kvysszmy.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ieifodhu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bvogwwkx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3cyazagpz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3dnfmhmoa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xxyggbuu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhjnydu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3llulknhv.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3jotflsbj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3eodmpvlz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ihfogvkj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bavnpidt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3veewspfp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3pzbduzwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3djhvcsik.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcsyfelm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3bpmxyckt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3obdcuynx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rgjrmevf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3mgckwmbb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uzmyjyfy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3cjsescia.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zvyziuuu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3wgqcjokl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3pqdnnapt.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3czicgveu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3spnpajuo.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3peoxtcys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fpltbrpy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tpugdfrw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qrjjezvm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ccazpvrj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3oewtnqpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dtmjjthx.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ilfnbplp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oyelpmpm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nxkcgocy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vfphpcbi.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3wighdcxt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3vrmmnsqu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3tqlixlcf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fehvxtah.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lrqmgzjm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3esauhpoj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hgdsmspx.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eztyxwdv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tntveohq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eybmlghh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bkjimfut.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtzrttc.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3atmcpxnc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3cjsgfzbk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rmccslbp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3abuxuqcx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3zeofydmz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jrhokpho.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tyygujlm.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3fguchgbs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rzenywfx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fgjgzncd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3texsaexi.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ubeldqik.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3atqgavwv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3odiwdpnf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cvygtaag.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oerugsjp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3rcnlgzwc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3cchatccq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3etlptkei.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3qbpjujar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hqpenqjv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jkwvlfbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obnpqpvd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gurbdjwh.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hjgyrdur.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tqnzyksj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vphwlouu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhbmrog.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3usyaozbq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pebyhlhl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3sayytrjm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gbltwxwe.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cyizonuz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nchflapk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mutrtwgk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kjrwgzhv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hrypveho.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vnzsixby.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eegrmjyt.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qmudxvtu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3spflrclf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3amrxopzt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3sibihorx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3zzzgywov.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3twwdzeqj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fcvmwpbx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3dpimhilm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3lscwqhhr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mjnheqlk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3qpbjfctx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rxwbtafz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uesaibri.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qygfjbrv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rbpgfcta.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3erqcmasb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3reixsjwa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3fgfzwnfz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xtozqbyu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3iugxuqbo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3zarzwruf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gkutzzrj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3skswdalh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yrappwjw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jerrtwhf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3uobozbng.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cyawlaki.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xkzusoqq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3susujpnc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3xkcixyda.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3hsurvsgf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uhekttne.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3spnedhje.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3neytlfaw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yeconscp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zromnevg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nnbzrrwa.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3uwlziqnm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bvrorxhq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3mshovhep.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vdzplzhy.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3pzrbhixs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfigoj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tkiwijlu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vponyall.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3dpmuyqqe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3edaqwntj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3onabnfrk.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3titjasjj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tvpgjagm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zpevlgdi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dlguvkhn.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nfkubtpu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3wkvfqcpx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3clzulsof.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xoecqbby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xtdimppd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3lnednlzw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqdpexmq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3bgtmrbgs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ykmxfmof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3skxyahqf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hautjrso.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uhomdzpq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltylralr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwrguzyk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ipwwoorn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgdqaoxx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ecxgnoaj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lyhwptjd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ndyqmhmn.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sknrsjtv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3awnbzhgx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yckrundm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkjvupix.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3plixtbcc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3oocqhdkj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3zarsqcwe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3mmygloys.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vlnjypkx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3tcdjppyk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jgltisux.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ebxdsvbp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3yqmqmasd.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3durozqgo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3qzkpgtle.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3arlrbrlo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ssgctvft.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3epajtwaf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3htpjtcls.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qttfpcsx.html


<!-- 参考信息 -->