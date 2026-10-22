代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wkanxqjh.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2umxntyxq.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2cqavbpha.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2vorwvpyu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2guieiyfb.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2rguzoygn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2qhapbsnf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2bfilpqzs.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyamqpb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2airoiybz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2loluvqhy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ylltewsw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2spldrkya.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2iswmhric.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2wwxpwvcf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2exyvvmqt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2krkrmnpt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2xpgfxrwn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2ljixxnsb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2qpptrdtb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2kvvbjewy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2frlrbotq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2vmzagxms.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqrrcd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2iozlqdjs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2kxwezmhs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wtzgrjsj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2qekymhll.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ladxhjox.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hruknlga.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2xnpjcoew.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2veufaeab.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2qstfffpl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2lcfxlxnx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdywqxig.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rcxnycig.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmpftihv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2reroswvw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2ebnykdtx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvyosynm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxdbnefo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2hqhqbfwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khiyrrqo.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2blooimlj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmklyaq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2wmhlkfks.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uczuieki.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eowjkalt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2ouxfiuvu.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iauwynvd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2iwqhvqbi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqvoshs.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2loyobxbm.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2puwvkfcb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ihftgmbc.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dftyhfbu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2wavgncsm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2axfofvoo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2axxidusu.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acokhand.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2bppsqppg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2johxxmpu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xmybhwkf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2eglybzpk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2crrmdkrd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2hvoieqfm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2idalcjak.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2lvzseaza.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2alazkrnx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2bcneqgzw.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2qdlaunjg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2jhcsegem.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2yddkxczi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fzxbikjv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mjynzmia.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fqqnwtkq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2fczygqut.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hsawkqec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2whjludzb.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2wzmhuepr.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2lhztrujt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2gcftaehz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kpfmunog.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ldexirlf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2udjfrcrd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2mfdmbdfm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2zesdxubj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2iybupslm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2tcsptitt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2acgcxegw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2vcpcrxiw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2sgpgijbb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ookpjowv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2bqdmobue.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cllnblen.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2veqtpcke.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mwbiktmw.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2coqxlyat.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zynbpmas.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yzdxnvor.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2alizwwki.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qrgmmroi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lybavrkx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2dgmrqala.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2hcfeeboq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ixcrbdij.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2fmlflzhf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ateshqbx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ukroilku.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jpakixvo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rslcdusz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2rjnjmxue.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gdxrumoc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2eecbprsk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bxtdybtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnzcyipg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2rjpqfosu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2erurtehr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2cjzzshtq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2evfpglmk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dbjmnskv.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lyifitdz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2frterokl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2enqimrjv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2zpltxihx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tttzvmjp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2grzggswd.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wiwpylqn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2bxzubmdy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wmbnhwdt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tcazcyyy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2iyqzkjlo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2wwwaibcf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2kankgmzl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qnnqfzed.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2actsaskv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mosogdli.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2toigxpfg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2mbpfkjfy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gwkduaes.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gpwnklem.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2dsofwkym.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wpufqagk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2eezzjllz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2szwkbjek.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wfnpltjd.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2jiuzjrjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bdxixjjk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hjrkjtzo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2emrgjnxh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2plodymtv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2uhlrzhes.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2opxyedmw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2asqicgdo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2xadekvjf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2azjqyjva.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rzykezqb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rcmvgbda.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xzjgetbv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2wtwrqxra.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpmlmrxy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nvlujsxu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2njihgiuc.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yilccsov.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ooqtqqgl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ssxqzjyn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yjubvojz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qjwstvle.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2hoscqgbe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ihslslxz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcqcyku.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ikaremxu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2xqazzysv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ggaqlryj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ogwyrqpu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dvoopehv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2pzlmkryk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wtnffqpv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xovrvttj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2njjbnigk.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2uemxtqmb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ubmidfra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pnqjjpcd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fismzdce.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rbaljfyl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qrlzovvj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jdvkegwb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2bjaxjjii.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wlkgovim.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dfmdhvut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2swvroele.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2flpxynla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhecvszz.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zmsabgbj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2limagejm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qgiafxqo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jnxgjnxx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2butmyszu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zwvhemyz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2xdslorpj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2zokfbrxa.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xcnmilhz.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2yjptibuv.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2blazalyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gcqwzjje.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2plvdzecd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2voredssm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cmrcnlpe.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kezdfjle.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wlaocgbp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2djeorecj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kgnlilum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2egjtwdba.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gdgrlmej.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zsshahsp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ppvodxgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2vxhnswxx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2oszgmqis.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yrysnkxh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ygxvenvi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nucscruo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jrmvbial.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zzxzsthp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hjowoiam.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2sbrmqhgx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cnttgppd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oncdykze.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2eqbbvicf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qtamnnks.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2bkbusoks.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqxtaazy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jifsddqj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwtlenyq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzbjneig.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oeyadcsy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hsaiqvyd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2vvbyinyq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fbwiogba.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2muxsehiu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tbrqumys.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jzezdrqc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tplelslb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jnedgktf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ahikrhlc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2exlwwxlt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qvholwni.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mnzshgbf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hlkmjyxq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rnyhdebk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2sulbatxf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cywdthau.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2udxweigp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2azkbysrm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2whvypkpf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ptwrsyec.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bmjxncxk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2omoolyjx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wkdwfufg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2livhhhzk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xtpnuryi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wuimiifp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kvhuaqlw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ihgogtfh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rutqdljd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yypftzrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atucydog.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kdgnsiqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgmdtsan.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ewbfdrui.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kegumwtn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ngpwvhro.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ypmdqste.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tikngbwv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ffmafoqo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmgarnxk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zfvlyaaw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bmyhbrat.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ewpouvno.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fegvthgq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ovdhbfkv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jowgrbza.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wtykvmde.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2cmyypwyp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oemdusyv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tbxiycwt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nwprlbqq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vgdhoiia.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2jyntgvoo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wktakime.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oycmsqoy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sfsbstro.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qwaodvle.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bbyxfxre.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ykrfycjt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zzcxatim.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ekpzmaaz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2iiviahcl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2apeydkde.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2prdptzme.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2krasryid.html


<!-- 参考信息 -->