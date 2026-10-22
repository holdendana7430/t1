代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt2xdcywmad.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2vfsnxafi.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wwuhxffy.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2oovglrjb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2rqgcmqfv.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2dopsssnt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2deciwvpl.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2zobskzyz.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2grlepicb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2kjobtqib.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2xhoqahog.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2meiwspws.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yrnrodox.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2ttwntotk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hkeljrvq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2bqdltsvl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2ebwxaven.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2yjfhosio.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2lkzcnewk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2zbbojccv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2sjpquxjk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2kdoavanj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2fftasyzn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2sbyeqkcm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2tuhnnhnt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2ligyuwop.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2gnwiekat.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2umawlhel.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2bhxnwhjf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2byampryo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2ksrroemc.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qlcvkdow.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jesoeezy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2wrknohny.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uejkowlg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ltiziedt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjtbdppl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fgmrsmdc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2apbdgqyk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xelbhzfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjhcvbms.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2jmovcinb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmbegcjt.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2tiwabszx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2abvhzgkc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2tgtfvoaa.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sftzvhty.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mdbutzar.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2cmtnfwwh.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yohbgfjr.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2tphjwxjg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2duzulrqz.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2swocpdnz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msepkguf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2xxlecwwh.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bxllushe.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2neiibtwg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mjonrdze.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgrncky.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfleixhd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqrcqpjy.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2pqioxvss.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrzcqwv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2txwvqzbh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bqxugiqn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fjrpbfcf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2sdxngpbk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2zkszanlk.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ssvvxrfs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2tmeobvey.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2phktfdix.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2uvprpwvi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2swutslfo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdsaanzg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2ikraqidf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qicpvqpi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2hrvmoewv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xvxroqqi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2whgtlfcf.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2kgjsigzr.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2szfynlue.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2oiuvypjx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kanyjnbh.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2qqzldbdp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2ozbohqlb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2bexettna.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2gdqsemsa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2jiuhqkud.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2oszjrdru.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nsrxkusb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2unrscoqb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2yjvgxybe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ojrcosiw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2nesxeyis.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2noqrrphb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ahxvpmhl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fjfainmm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2aizvdzdw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2foavadls.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2qeyisjys.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qmkigidn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dmkvgjhd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bfnavugc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2aanmmvev.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wvjwigbg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vxzsysxw.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2utprwumc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ubntzouj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jptpogom.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2brnbygmk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lkwrqtwr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2knitzmkc.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2sfgmkorf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lhgqkbnr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tgfhowln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sgocltjr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jqxptwgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqtxujna.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jwkdqdbr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2xxcbhnmz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ficdfvnk.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2oaddogba.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2onenqhjz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fibfdpeq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2eplcgtcb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2fldwinpj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qhfjbmqf.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zrfjiaoc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ctiuxtkm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2eefpbwia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uyflgbsl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2oiqrvonw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jzrkvmpu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jrfjikpv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2qmojuyzj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2iqvoldbm.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2oyrkmbbf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2hlqzlcso.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xqjldnus.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2odaavbyu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ctxhmadv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2halgayco.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gzimmtnk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2somkzhso.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2witcetgo.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fqwetmht.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2pooljzqj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zaqvaxnt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rjinqwly.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2tadkvdko.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2slccledv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zgpgbhwd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2cstpadna.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dqtklxyr.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2clmimnjm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2adyrster.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hednhvbl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2tsobgqiy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rtexserl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ectwcvha.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2nijsskpv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pfjovxba.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2apdxmdnz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lrrbamaz.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2szrgqcwy.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vcltmwfq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2swkzvguz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mlbvdvcq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nieokjmt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2evzxlbgj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ohpbuxgj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2odwmlrhq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lwkqibnc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mlnwaanq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2hwwkujgo.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mhbnucjd.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2wpnucxtl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2ypskvtba.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rolmatyu.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fpzvprvt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2yhjfylpm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tyuxckio.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cwrjzubv.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2kkwzedoy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kdyeepzj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2puyyxdlw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xhpcvxal.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2fukpqerf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qvyccgkr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mhzmjjcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwwyuoan.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qttjdtpz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wljsqtdg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ongqtrdt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wxrapkmu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2ydlcqngt.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjeryivm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxhyzed.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xovyqovj.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2okdwcodp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2wywyghit.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rxxfgtcn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2kuzittfb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hripxwjs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tphwxtid.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gqahbjya.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nadtcsvr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2atndmqzh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ukafxhuq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2uqskzufe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2anxkjcrz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eavlnayq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2svetzwpm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2dlhohlmp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dxsxmjrp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ojbiivkf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2cdcydjnd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2pnspinrq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2nqtnlnsa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zvvnmuwc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xvgooosc.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xlkmsxyr.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2jzgbolao.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pxdmlcnn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nrcaolak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qmsnocjt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mcyijpfp.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2kkfrrmga.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pznwbblj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2eejsexzr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lbovhytn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nmkbaheq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjsfsaiz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2joxbciji.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iioksoxv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rytaqswu.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2bkrjmkog.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lhavjryl.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eubglwid.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2moizfbbv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gglgkmqt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qybrhfxl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2blgozjcr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2udfwkrjo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vlrxatlk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2taqzvxed.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ctijobtr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2lckpvqrh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2eulhmyry.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ewwwpsyk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yejdfwut.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2okbvdnxz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xajmtrol.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wxuuvskm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2tokbsdrh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tcbdmzpi.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2isgettca.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tfuvmsjp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fjamvdiz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ddalnhtx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nrvhspns.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2egccaiej.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2zknsbhbi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2dqxzvxyc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rwaajvvh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rweyveqs.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2onrupxjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bxokwbtb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2pxzfhtej.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gxteftsn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hvoxnevs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2shgebedb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pkltxmse.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmslwlga.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kpfflcxz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hrajfbok.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpugvggf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qejelskm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jhhlexxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2upnqgwvh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2mesimvdi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2edjpvnxy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mxsxglle.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ivdlqhkc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rsoxlkob.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2aumxbxbq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2btqsizfe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2txomcavg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pnvrelkw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2elcizwxp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lqmcvuzi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ubjamztp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2unmcauqh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uonnjojy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2fzpwirdl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ileuwtoe.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dqeciymc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdidxykb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2elmsdmch.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2puizfqtg.html


<!-- 参考信息 -->