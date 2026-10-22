代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lzjsxkaj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2tdocpxxi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksjuwlmq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2arkiuaqj.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2jfxoooou.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2qzpuewfx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2uyurdyib.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2rxaatbgb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ijrjieae.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2frkdrjbs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2npfpohbt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2pvikeuui.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ojhsevhl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ebhqucvq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2tnfcqhnk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wsfesvbw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2diwwldcc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2qhlygtun.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vaknpwfu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2argzgtno.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2hfgpdsdf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2ycswhdvc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2uttvdhsh.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2blkyamdx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2blbzorzt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2orenxnoa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2okzmfclc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2dolhdisj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jricztpz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2qanvlnkh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2tigcdhwo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2sdxdgtvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opvpiiki.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2wejhsmzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhiyxl.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qrdvjatc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2fqequfur.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2xrzgutmt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2pieitgaa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydqvlrvo.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2efzprjvg.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2qvqnxxfr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2zxopwznq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fkuehzsf.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2yoyqafti.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cbmqcdyb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2ssualodz.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spnextgh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ofmhcvkr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2yblgllgl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ilhreore.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2ihixugpt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2anzcsqdn.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2sbmzjgsc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ztgipops.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2iwcvvcam.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iufqpnbn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sodkaeol.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgpndobd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bdrcavgu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2iiohpvhp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ygrefvah.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2lcrcpjce.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2scghrhux.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2bubhcdji.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vyqapdqo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hlxcefaz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2sbbkyfvh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2zltsvwvn.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxuaixks.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wpvoquel.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2daygolgd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xjmhbrru.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2tezfcwle.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nhidefej.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihgubcll.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ebvurjli.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ktpsbdma.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2uxnmlhmf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2zngnxcdx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2dokyaitn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2sbkdtuxd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2euqtvhob.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mlakkhqn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ayukhhrp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2emkocxdm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uyvlmpot.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uuofsamc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nhsviptb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2sykvthef.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2useiquig.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rskurewv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rmewwqqz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kniatglo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wwbgzjsj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ypdkcrkc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2zdnbfztn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rggnakkb.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cxnxfxxb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2olbdjlvq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2epddbahg.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2koxstckw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lksjzrtl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2cgbbhwdb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2jlnwvufc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2krnigfhw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rovmxaqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqywcqez.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ygpcrybs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eqfiegpo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2cybnjebj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gozbsxpd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gsorhedw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jgpnxfqu.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2klxpwfae.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2svqgpzxm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2grvjpvyz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ssveczja.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gxnjeejq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fnzqsszr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2oobagszd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ebrcsrrk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2glcweuqn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2mmpwguqf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2fmlmnkrl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2phfbbkfl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gnresely.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qswiqhsg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2liecgjqm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ollippzx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2inlhcrdw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zgubgtey.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hdpfgqdy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2iaymdfsb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2poobxyur.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2majvimoe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wmgbmnwn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xhmfshwe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fpaixwrz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2aszwduuc.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2lxytjglk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2pbrklkqs.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sdhypzct.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2hgatsjwt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gxotjufo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2iszpyekv.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2bkcmcfsu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2jhehepem.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ngzbcwbk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yhulfxok.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qcefbezh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gylwttmg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2xzmvtdia.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tsmjrfmq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbfkfjdq.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2mfhkuluz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lzwqtnxn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hrtiwukk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vtvkoqfv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lhmagqwy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qlyjnund.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ysrxvqvq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vlpahskd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2uduuxdpf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kpolifvv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2pgjoxcez.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ysirfjsl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wphkzlid.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dltbvhyx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pjgwgovn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mwwuyjwa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2elarubed.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tvymrlon.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ekrmcgsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bzqnozpy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2byhyyoyf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2knmqkhps.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2irqvqhgn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2edcedqpc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2cnuxzsbj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mfjmxnkt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fdlpphtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pftbujcc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xwrnxzbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjvmwphg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fqcscjic.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uxmcwlce.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qwebtman.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejspqsjy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2gpmpojam.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lihowteq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ssrxqrcx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2rqecojlu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2srdszrnp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gouwuozq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cngzesjr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qkbigtnu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rcsfqgzd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vrgtfldr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2omjlsyqn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aapbwtsz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2pennogyb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xcprqyno.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2arwcvois.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fipddzqq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aknwmajx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dxwhieat.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lduwdfku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2cgcrjjyd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2nqecyigi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ktdpmgif.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2qzarcrss.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qmndtuvw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zqnczihh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ymxgkkul.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2acmvaxwh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xuajngev.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pspbrpyz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tewfwfgy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zvsuvzed.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rcslifih.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qvevatfy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fvzamjfl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vjmbylkr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjztfvtb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tjnlkdqc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eloqrlpl.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lganttly.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tjvqdlko.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2fnilmlqp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2miswtfjf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2enxquvvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2gvkpfzvz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nlcoswzh.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zznzydyn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2znakvuxn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2joltkvlq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qmvdkkos.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ptmfotlx.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cixlhwxd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2adjfhpzh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qbmzzoir.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2btycjzmi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2woxyfuds.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjwhdom.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2uqorhaks.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2amngdokd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xibzrsmn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uddeuwae.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wugcuryv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dwoolkew.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ejmpzxch.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ehgswjvx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ruqumgxr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qtvqsord.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wnbyyaef.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2flifrlqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2whqgpjzx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2vslkqoia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoryhfsq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gqaenphx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgiqncal.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ezbyfzid.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sxfoyxaw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mxiagiiq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2irlcmozs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvntuois.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qcvfwqnu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2woohozgc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ndljzybw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dcdbwvxw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkybkzi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xjkshzan.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2elkstmlg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2usemyqok.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aftaenbr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fkbioglp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2olsllfaa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2swtmsnds.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2vpuffylu.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ylfywdvk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2xfisitgt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cuoleveq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2phxgvles.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2iukhkcle.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lyngzgha.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fnufpequ.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tnynmkmq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2heieijpc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjvobrhc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hivfoirs.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ixjlkcsp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gujoiavt.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2atgkozyt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kjpxnevp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lnfmgmke.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nytshkiw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hskzndgl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnjimxo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pbjwzjua.html


<!-- 参考信息 -->