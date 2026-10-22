代发 wailian999

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2fpwpaclc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2scyrmmja.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2hpnxvtli.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2vxddgrdf.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jooceipf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2cntrfhdt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2zaihzyhk.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2nhdquztm.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2iqecsqyf.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2resuhhcq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2rvnyjizu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2taxlzzvb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2znpctfyx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2omkcvthf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2onkefpfa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2pevewwlw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2venvqagq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2ovhsajho.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2jyhreuwx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2kviabmmq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2ovoxgxpt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2kfjzpyci.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2niphfqti.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2nwnpqojk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2auuhitej.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2bkrqbfoq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ttibjhkn.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2fcmuxyrp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2itfreoyn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2vtnekpzz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2abscfyen.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2soncawzq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2cglyakdi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2iubpyinn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2htophfmk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzgttgpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aevfdosv.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2whpuhxcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkndizjh.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2xmmbuvib.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxvweou.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hbvferln.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vwjtjxli.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnbaaco.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2fmaqyury.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2uhrvmquw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2yrtrclra.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zfxrvugn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2jtjbovae.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndvrfomb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ymfrpizc.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bdnqkkge.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nnbfnrlf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gnmdmbob.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2nxxxqiyx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2yjwydxpx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdpulkrc.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2isjgyvuy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ttyjfebu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xuqifwlf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ecbvjpvy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2rikayazr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2cquodjpy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2bjoiwakt.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2cscxddpp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2zrcbhiph.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gxrcltag.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2lhgkvjuw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hcjuwnud.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2sfwbpcpx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2buhjchyy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bcseszye.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2sesulmas.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2urjerizh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ieditqys.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2siihxlha.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2mpljlree.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2qwxvbfut.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2odovbkox.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zyfoyhty.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2phegejou.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2zvzbmpnd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2brgpyeyh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jfeszgon.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2zmatkvcj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wtnzqdyg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjrjtriu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2norwcabh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pkncqrxx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2idqitoup.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2raopcsgq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ouxlftmx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2crpucgky.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2sdfxuaoc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gcwtlogp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wywqvbhx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2wrcfktgw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ocupsukf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tkafuosw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2sfokjkqu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ttlefmyj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndjsbcby.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2suqixrpj.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2asbswwlv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xczcqdjz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2syxuhsrt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2sntaaluw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zwgcwnpq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2smcyoqvy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzwkgya.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gzjtjtua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hiekioag.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vkegxnkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2munvhygp.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2uyxzekql.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qogywmal.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gshfphec.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2srxzskrf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lyzuwdej.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wnqmfnqo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dolrcwhr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2qvrawbdt.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwnwnxz.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2urxfedoi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2mvirzfjn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wbraqgjk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jkkntcaj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rdypnlmr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ksmmmxqy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qbskaoxh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2bkttgfpp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2axixflyk.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zznudasc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xmzaqwaf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vtjyscro.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2znotrxcv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jdgltszq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cjmotpyi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2lurqtgca.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2nkqixqey.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fldehfpl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qqwwgviy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2otwechjj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2zttbggmp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xebcidlf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2upkujjjl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eyjzdgsb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tdkbzvdr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2gcfuuein.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ajwwhyzu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2sbizekpo.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2exuwivrw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2syianluo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2otlnfhui.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wvmkuzlr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rdvcvlyv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2bnudogky.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bogmuklq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ddtmdsnl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nnhfzpxi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jetbbple.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2aywovtot.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ptliyxpu.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tznpkihh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2cvciwhwk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2kjxlyjam.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2kxjsyxfk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ghmmwwgt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ukmwbdau.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ifmzzuhv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2znaavqqs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gfojmumt.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vifzhofd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hurarzgm.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vugpgcwa.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pwikcere.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mjznqpkv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ylzwgoaz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2pkmhefub.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2iqlnmgcm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jdgnccdh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2dwgzdzca.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hctmowli.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2stxoueeg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jbzevisx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2itntuiql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smaijiex.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2hxkrpdud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2teccxexn.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ssdytbfa.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2gznjlllv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yarzdojk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cyqkcmeg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nastxwhh.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ouayernq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2msalhnjk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ymrunaka.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zzmpwbvz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cfpsslaa.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lruuiyco.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2izucjmpu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2inxocoid.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2skcxvzaw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ohnfnkun.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2scfduxmn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2dqzdzwqc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2drbiguec.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2xgrzymiw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mjyeddok.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bfxmpzbg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dfgsyjol.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2inrwaewq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2igphxlvc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jvlgzujz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2saezkrws.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qxozhnsi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2iiviqcye.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mndbtpqp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ahggvexn.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhtbgi.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2buwueetm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wsizihgv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2xzswuzii.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2irhetqzg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2unzswtum.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2iwzrpbyz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdzgyras.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2wpxxygyf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2scrrkrbj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ezgibfuh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fbtafwxb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qpvibqss.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gijcydbz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wokdsoif.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pnufyahi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2lgovyntp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2jtawvedy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jjeulqrw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yidgadjr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hgktdsds.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hgseplwp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yklhswzw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lrgyvkko.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2xosyqfbj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2jtfhluhv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sqfhvbtk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hunjqjqz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bqqlckgw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2guthcwvy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mqyprbvm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dfkwhxjn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2scrwlfbz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cbgcgmwi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mnualfan.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2heeugtct.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2wflxfogm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jradnedt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mbjlhfsg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2davetgck.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gxwlhubw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hrhnghhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvwprojm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wgbyvykt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szfqcfel.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ykxzkhsp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wdrkiljn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wywnshux.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cbmzncsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wrbvwipw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2slxrxljz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlncjsyb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2utmybfyf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xvvfprfe.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lpootctg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2okeytbvl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2almebuhe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2atsoefsh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdjpgjfi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2vrofyaau.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfgaaknz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rjrwznwc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2auywocox.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mjnaxsft.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2iuiqavhd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qiuaoivf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2drzfwqrf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qvfehdrb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pikyojeq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pugeouey.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2yrccxmdn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2drdpzyto.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2kfcfgfzd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2shmhpdku.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vbnylogq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bzcmvhwi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nmrpeqtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqmhbwl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kselbokq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fsdqytwc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zzclrxjx.html


<!-- 参考信息 -->