代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2jgzsiahm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2auxxjypp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmspsgb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2tlqgcmdn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2mkkpunuy.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ofxhvtvq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2tjzahbbj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2dvroyqmk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2miuldacj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2vvdrrano.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2ininztbs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2olzhjnad.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2byhedfmw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2giobizqt.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ijtgkwqz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2jetpfhqt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2gujslauj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2cmsemwso.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2twzugken.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2oumadybu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2wguslbev.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2hwxnyylk.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2sdqngnwt.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qqavbney.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2srhfvvep.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2qtcnydne.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hekrwteo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpevkrpm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjslcdtf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2snkwiszj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2rsbjmqdw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsrmgqts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iitisyyj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2dvyramtv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuoubkko.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zoksitwg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2teziapmt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fjjzbyxn.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2trldbgvb.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2scfqprzm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2selkmyzj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2drmkkcyo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2frjtwlfp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ynvkjyie.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2dqtmaojy.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zijqedbw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vjxidkgj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vnopfuad.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2tnngcunt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uasuyiox.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2ksgtmhrj.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2txsbeqtm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2rdxekyjl.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2yfgkmmtc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lsimscay.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zgqzepsk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bdlvvhmy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2stczqckt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bcsrnjgs.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2twwptgel.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2amysotzq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2kjvugnxe.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2hdbfulea.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2bgsxjmna.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2semaypoc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2mmngydif.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2andqftnh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rudurtkf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2psyudrqq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rmvfvump.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lsjtcfaf.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2drfnjjzy.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2tfvhyuid.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ujciihqn.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2vwkpnxgs.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqwodggb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2smkjjmdf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fbvufqzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qpynahoo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2nwphxsdo.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ldfksdlt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uathmcod.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2gvuomnwb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rdixldba.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2urexxfgs.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2qxydbzld.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2tnkbcfyi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wdgxlsuu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jbuivnbh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2bqlkltwh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bljroohr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2izwllsqy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zorrbujs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzrandu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2redljtfj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qimappfg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ueyxtejz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ezrkkwol.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kqvudkaw.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2madxhznx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2nysniktm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eryzmceb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iylbfhca.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2iwlrvyzm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wlgzcpqx.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nzjnxnxo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nhnnbdig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hombtsnz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rlchntct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjotacij.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2rtgsnzsq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2qkiliyuq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2owgjmplp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wpcuovvp.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cnkogdju.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2tlzlijmk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dlerytfd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dlxzjgsr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2pggumceo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2nsmeipcx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ngeewvih.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2clxkgzpj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cojozami.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bfatzymd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ojiglzkr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wpeekjjk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2rddbfwli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ocaxqyak.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2tucdxyxg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2iumhajsk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hvrcqcnh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nqczgszf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zxhmxeeb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2tvlbnelx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uuhqdzga.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ixeekooc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iclzyipu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nhqgoppy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hbyyteto.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lqnwsjkh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yxrdmzla.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2frpqdwdh.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2tevfspkm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rdrihdds.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2mnmjysbt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lttxdcsb.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2hhxjpfdj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2yptxslkt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2whdkmizb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2mqubbyvh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wikeeupe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2cwbbjasg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2etpktgrm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bzhtmtjw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vdozamro.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vwebdzzj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2cqgtdanu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pjczhmrl.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ycotnnqe.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2svfibikr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xfbjucbx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2gynqwtvn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zdnmyzul.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xwajgaef.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rmylcidq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2nnikdsdh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2hhisvxtz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aqkowkfi.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2imggvlqz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2chkgcsxn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2fphjhfxw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wlscfmhf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ivejvzqb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2gjipdhbz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ykedtblo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2mbmycrkh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yfqfiadb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dryhfgib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2pspfpuwn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lrbukovz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2crqnmhqx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2qqncxtjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkeejarp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2vfexrowx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqiwohuy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2usdssfkw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uuhatejn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2woicsxeh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bqmiwimt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ksowukjg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mmgbwtmf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xpcopmrg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cpxvqrkc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sppvytaz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2maqnywas.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ebxchtye.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bbbuvxwm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ffjmtrac.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2syzyygok.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2gurrswbh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2chsoscyj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2zmjmliee.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2elisrevb.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ycpyqgsf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2abndyukj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2kiisenxo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uasqcbqa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2kwbzsirk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rqysqdea.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gclkcyof.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2aelrlifm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2jbyzkmks.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2awckhoky.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kcscumpm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dhlblxyh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2enpufglg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hfotpxqt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ietfekdj.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ahagbxwm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2szcovhdf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ubnljvyw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2reihvxus.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cwwyuwvl.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bxtaomof.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nnadhxdi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qdhnfbnu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ligynagx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trnormuw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nkgyafde.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2unbmmczg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2dinfzktb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qhjnykpl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qbqabecj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2okpuwdvj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pywfrulg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xyxgwzmb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ftxpsvic.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nrkncmsr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jhgqqprs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2twbydoro.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2rxsywhkc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2raotgqzk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lpcadsux.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ltqjjrdb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2axjzlzii.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2slglbkxh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rljgffma.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpsvob.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2amphsdiz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yrkrlckv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tzuaonvg.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zofpgsoc.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kttovimx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vjvgsurp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wmqsgysc.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dqekjtwe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2aeciurxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smedjkwl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2mtlnbwlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyzrgxsz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tgjkemfk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tnntlnws.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2odosnnzt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ackvnevj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vrzttwsi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ylddmbgu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wjvkyagn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2boxzwitx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vsliqtwk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ddnbptnl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2chrtjagf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kbnmdotx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jqifbyaq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2aoctnbvm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwsoect.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2qijhtzml.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ooxiprvs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jaxbvsbe.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vwwdvcfz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tvbubpaj.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yoblliof.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vdurjpkv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2pcizkjdq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2iljtmzrd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2btxoytdw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wcmkztmh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2mcmcjcpw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2egbnxawt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ahbwtuqd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahqmyfqj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lbazweam.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2iqyzfftg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhxohrzn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2tleqyldw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zmfngmzd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xkygecbt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tsmcwvhi.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yzymxadf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbdcqlfa.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvwyaen.html


<!-- 参考信息 -->