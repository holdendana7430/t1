代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3fawefcju.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ztfmkdjw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3idicwysb.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3lqjqieaa.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ddfnyztm.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3wggtdmwx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3eaajjwst.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3utklepbg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3gveqkdvw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3mceclvqi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3otwmcpfw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3xamrbrht.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3yjgvmufn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3gmhvavob.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3crztmrhc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3nlayqzew.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3zpckbdgq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3lleelsgq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3efqheusx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3thgcxtrh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3klhnrmam.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3qphgoagd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3iittkett.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3qjteuuij.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqeemrve.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3xjodogko.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fttublbe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xnyrhvqb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xcegzpfc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3xjfgkmhb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3eqlkyqqw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3itdaxfyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciypgmbs.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3mcyxrpkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dynzbbqi.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nwqxkhhu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gaqenxim.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gwstjbrz.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ptvuvalg.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3urhqhuyp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3aldgpyon.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3nztyovxm.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3rgjpasth.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pzyjlspz.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3djshpaex.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3fdncefhr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3dzmkqhuo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwuayqw.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uykwynur.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3wrumxpul.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3juovltsx.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lmfrwezt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3tdjjyiev.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3dotddbor.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3brcpfeyf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zfgpmgcg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qlhtkqzc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qaitmeky.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acbxnhsq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqvkhl.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3cumcqiqf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3zguenvoj.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3irtcfkbg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3aofktwua.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3zwvpfdmv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3zowjynrk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kmfbmyxg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ecaxmpyw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uibpxlan.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cmxbmtyt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ilzbkhsm.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3axsyqujt.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmghnfn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qkzcerem.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgaufqj.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pgcasdls.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3urzibbix.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3vdfaxzhf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3psjxukgi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bqcfziwy.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3uhaxnqvj.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3anrjbuhd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3rqhzfypy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3stdwiytr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pbsmvvkf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3vfswqnwj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gogfcnlf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vfgdbaur.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3owxnjmcd.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ltksjecm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3brdpcozc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3nnejwcxz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bpdfbzfy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fchwkysv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3stnfvgsz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qiyypuwg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3qsrgexzn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kaxasbiu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ajihqown.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sdtoottt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3kdgbjvan.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3srmtoykk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3xyyqkvsw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xmbdryhq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3mfnisqsf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3udiyfmuf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3pistkthj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tboptyqt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3yzejtlia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gferwgpq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3huzfjxoq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3gcsxpphu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3zxfusgcs.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pcskxzsf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ovsiqgpp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oclttoak.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jpyivjnr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3mtycmpxx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3dfaoyntp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fyfxpnih.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yuidrfhe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kgagfqey.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3mapvdasw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3zkvqevdf.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3frzjsplw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bngefeyr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ewakpoxl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3kfjaydai.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3uhaeibxu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3eiyyivhz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3axyeykfm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3kukqiuag.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nwbljsvm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3qglxmnhi.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wiaxjbsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ramdnwea.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ymskvqre.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3rutvbmza.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3rgsnlrez.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3bfyyvgnp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kreisfqq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3tuwcranj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3gagldxeb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3mahgiyrt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hygyyoag.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3cvxvkpzd.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3lnezgfsv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dlgzjnxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nazagncj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3vzzrkvuc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3nacoswdh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3emycibcl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dlqezezh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ikjoxtcy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yrmhiimk.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3couggkdt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vdrfotyg.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3bmdodrxy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hxsnovpv.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kjejghlb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cyufowil.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3bbtttifh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3kdvuxlns.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jprnnezn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3alxfrifn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3maoixgpc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3buabwxgs.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cwklxvlz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ijetossf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xyryxlug.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dwvwrfjz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3moebeohu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bjaeepcl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ujolumlr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ucfzntmu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3bughasrv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ncyvkmbd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3jksuwlga.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ftznavln.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3aifcwdrj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3sbkooabj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xmsprzjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jeosnzbu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xegvecfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxxzmvcf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ivpyocei.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jcliubcv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hujvxdrv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ejtfzfwc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvhaqwxq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3knosxoke.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3fxqopbuo.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ifkbtpte.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3svzcozui.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yyifwkyo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mdcpagfp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xaftpthu.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3iiupozqm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3eyoscntu.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sqfvwmem.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3esfzzgye.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vajumohv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fjuynyac.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3acznnrpy.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xqzwzggo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zmtlczvw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kuomkrvb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hhjjfecl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3rpoxdqlt.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rjxfyxrb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qkblgbwr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ryfzetql.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lwcyhgfe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zlbppnmq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3jaqdvudy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kqyylgaj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3drsjvkfd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3fhjoocqc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ebruzxhi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3xrqpqict.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ibanncls.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ctyzokvf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hvajonwj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3upbszknj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tduyrlxi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eeoulity.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3orgnimqz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3upyhchbg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ukdliiev.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3abzrqlnm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3gfqodqib.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3zuquqqgg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hjdxnkzr.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfauind.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ivmvqqbw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eptamyqm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3naptlsld.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3nyrjwzaj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3jwqxhvkt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rvugiptl.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3pfvlymax.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vimoaztr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hqcutilw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dljkzwgz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hjlrbeua.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3dypishap.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rnbfcyry.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vybmdvlo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3olfrxanz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3artjvuhy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3noiknczp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mgywbpff.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3uvblesso.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3etfruqnf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wqadtula.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hrqejzfw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3exfcsckh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsxisxrg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rsejsmrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfafmfwq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hdsyoawn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ofrvcudo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uxtrsnjv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fmqapihl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xnfyccjg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3forphftw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fpcozson.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3uxyuqemf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ftplpxrc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3oydwquyd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ccuzojwl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ibtoobqp.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgytenl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xsjhbewl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3jjipmkzy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgtxzris.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3zzvydxuo.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vnpvkjkl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ocoqsnva.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3iztbnwon.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3svigiyie.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ipkscint.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jmthassq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jmdcvvej.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cngdejht.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3bpgoraaw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wfbimfij.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ykqtfvky.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3aqfcoqvx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3crdtlofv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fzldrdjb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wsmjmkkj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3cckrqsfo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3sliacdjh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3tdezkcuv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qwfhkpmk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3bayzgzon.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vrduhjda.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3hrqidvex.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zlepjhsm.html


<!-- 参考信息 -->