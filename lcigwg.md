代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2sgxkvbvf.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2djpsxbvm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2hdzornhn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rbcfwdyr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2mkstwewt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2gbqirjnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2smvlvukt.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2epwxpmrm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2nmyosymx.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2xtseskor.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hboubypk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nwqhqibu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2hvefazsr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2avursqoh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2pyjnkooy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2xgtjhmyl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt2ddkiizlm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2pcfiexrd.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2byfovmjv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2uufyepkx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2urxaqzjt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2bzsouwvm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2iaapcsob.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtzppkz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2stancujc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjdzvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2amfqkwij.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2dnicfldi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2yklioujp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2osfxhlor.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lntxgyui.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2izfcjrua.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jmtrtrfi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2hdolqnnd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2jzswrriy.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qqbekqop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxqnbhzl.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2bfabhagi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ybvzpjfv.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qpnadsql.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2vclfpeow.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2pqvwmbgx.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2axzscvrp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kvjxpxwb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2hqafwlen.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hcoaaise.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2tadmdmso.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2wskxoekj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2hysksbde.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvjwkeb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2kymrqhag.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2isnnzrrn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpsjhxuu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2klvmfoky.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ekutdyqk.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2phbedtju.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohldhxyb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2izqqvthg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jrrepcld.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fdlgujgb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqfeogu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqrcwhkc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2opiwdlwy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2prgttwpe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqqdmkrj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2pewnfhwt.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2desrwkdh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2tpomtprr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2sayaelwd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ijzkfzfx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2nckredil.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rbvykyiw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nhysrcxl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ypsyxtjz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2ouhauccg.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2mpmdbhwu.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2shwsrhkv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2vypazwrb.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bentxxrf.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kljqvfle.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zrjezsif.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2ngbxbqwk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2phevsrld.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2tnhilfff.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2vbnaxhhy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xlezyzbr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2pjgktaxq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fclfrver.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2eueoooja.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2vyctrwjo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ciryoxba.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2iavazssi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vkjwlemu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2jpyjykqx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mlxugsev.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2figbwzoq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2nfxizjwr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hswdagyh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2flutmcme.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fcqfxebn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xqzzgheu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lhkddoyf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2dmfiprus.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gtoaqdbx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dnvpaara.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pvaduogl.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2nbubdods.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2egpgfttc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iehrknvk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxtwujwi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yfwrxras.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzbnjcpf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2cjsubuod.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uimrgift.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2cepgjhdu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2adxyorim.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yuqyuzug.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kysoqrbo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ljsaizat.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2odexrugv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jroamjkq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hphmtlmu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nftpgtlq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vesbfrbh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wpzwwadc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2nbrusahp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zxsbrada.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2hxbhsgew.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rqfmkbxb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ukffensm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2fylkopcs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ravdsqvv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ztvaovng.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bawcfipq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksudhgjb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2edebonby.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zcuqroje.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ujfrfluo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2tubwrwby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2eghzoauj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zunxgdsp.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2krufqrws.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rxmxplxp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2aridovmr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2crtgllkp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2rjlnxlib.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wsuywrfz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2dopfedig.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2krodokrn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wvfxomln.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jdgpmrax.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2lzwggapy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hhvvmsqo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ejfbrvvn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qrnlhxjy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2vrapyblf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtplcrzx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2duvbsqlo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrrdehwu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2zvvrdgol.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tzpvqzcu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kheckpxu.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kslalvwc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rcxhznau.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2buoeomxh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ainyrjqt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2eguyzuuv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tdksfvty.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xyxkzgnx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2cwgktevu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fekebcng.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zktyiaxr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2xhrqstqc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nunbewuy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jwhrjhzo.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hnyjpmov.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2twcewdlt.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fqstvldb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hzopbqcf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jmuubfpp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lkybufel.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fbrcyynn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2qajwkagj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2zandngpr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kfcepwco.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ouopbipe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sekjwcql.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2kznmmfbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfuuenoa.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zwfufpuy.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zemnypbo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2utmvjtsy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yjeepstf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfzrjyfd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ysicyasw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kpommljc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2jzeakzxd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uitgcuzk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fhfkoarc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hfgjcuuy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tknuiemj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uiccqoqv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ksesfowz.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2aulfggst.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yvpglzkq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dbunvusd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bzwtbvmp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2kpwejgsy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fzjtjrgl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dukixgqo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2bviwsqlu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cleozggp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ovgifipr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2qsuvihpd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2osmbhsgy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2hocusdaa.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fzvbjwik.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2sswoblss.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2xyfxgvxs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gtlseqcj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2boiwcqgv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2idykbskc.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2kimezuyb.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bpvvhmsv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ewztrcds.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zlxrprus.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbesimbr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bimedpgh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ivxehkbc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhohaoih.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fanonldm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2spyridff.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cqsiqctv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ietotqhy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bqtbwuru.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbnqxec.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wmxezsla.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eeljkmip.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zepqcptr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sendymld.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2waflqwxp.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2flcazfmj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvfakfb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uyidrlql.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hwprwucw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2rfehihwa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2olajkomk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qxphozxe.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2syncbhlp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2xpicvsya.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2nrnjnqav.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvdeqsn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2tfuvxazt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2cnrazuwp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2woaxvjdz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qetzskui.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2olbqndkz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2pogizbpg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2acfhsiul.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dssrzgju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2awexgirn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eeapcycx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gdsokxlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmvrzejk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nyyjrsfe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hjglpfjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzofoohn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2egruiyod.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mmxfruxl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cmiciatw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rgynebak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zrytskqb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mosgetqm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hftnpuqe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2twxvilvz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2yqsbqxcs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2imaoddol.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxjvqwl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qwudukfb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyedwulz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ymrzvosn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dlitfyvq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2vaptcdii.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2inhtqzgx.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2uilffcav.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rafqojiy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2khvswrjn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vbfngdgo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2sbxovwvb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oiodtmic.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wacjnuei.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ydwwjski.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oxhqhuag.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2aifiwpdm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fporxujx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tvcystil.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ympdvvqr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nqbjhdhc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nbviyyab.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vxmskxey.html


<!-- 参考信息 -->