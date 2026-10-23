代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3yvcnjbxy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3sgdizxza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3zkamjtmb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3thxumhgs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3pazwijdr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3rzlehifh.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vybmdzha.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3jgnylqks.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3jtckplzs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3myncxqen.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3haonjbjk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ohcfrucw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3fmcwiayf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3ksjsfgcm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdhalxo.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3myctgaya.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3bwfbziyd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3jysdngxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbicgfti.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gsteifdn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3ndivfjdy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3anbnfywq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3fsspnmmf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jztuvbyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwbktejj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3xhxiioab.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlrmncqj.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cpqodzqi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ofhxmwjg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3lkihyzxh.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3zltovtal.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwdnyrd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3psecvzvo.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lnxhumpc.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3uuvtnpea.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3uxunptvw.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3kexnpmpb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zzicbblx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3ovlqcjnv.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hodklmbk.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhyhjsho.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmhhkjx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3bomtrgua.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3caodetye.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gbfolxhz.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3wfwhaglg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3ckqcvycz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gbkgwfve.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwwhpcgv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wpddmtzr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dlsybuau.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3mhbbmcbg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3wtsvtbqv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rhigsqjv.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3ioxyvfaf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3vobegbrj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3ghueuhjh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mwdtuxwp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3kjmvmcvk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhnfguj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3fakhrcml.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3cffeuris.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3azwwdbla.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3sknglcwi.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3snnkdwol.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3eopgmjuq.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wxltclbr.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3njosebxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3mjikwcbo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3xdgtsckj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3axircrkd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3adgemskm.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ckjthjkh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lxksdrrs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3cnxscrkn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3agzoyjao.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3ytkjgnvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3agdghnyn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3rhdfstcz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ydytrcov.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ugqjbwwc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ckphkdcg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iarvvpbm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3jubrmpdj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3sfkwibsu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xqxgdxfl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sgmzqxde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3omdnhzbx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tzeuznpj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3umsthjxu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rsfcqwel.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynmpbxda.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3exuslxxh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tbwymsxz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ltygoawy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lytdczhy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ikfvdenq.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3exvbxhfi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tltemaxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kslnmxpr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3lckalujb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjtirblh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3itmbpbxg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3vmcuzqng.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3szqhjibe.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3bbzzqzcm.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xekleodm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vxettljz.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwgiuph.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3eizjocat.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxcjuzk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3omyfalzj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3pqbroljv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3bcyfloeg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3arxroess.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3bxpppwut.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ltphafen.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3dqwsusyv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qthfqgyc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3cquirrsc.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3tzhtvfje.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3eqztfxqa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gktbpfzs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rqczmpnp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3enzsuint.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xddfqmvl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cpsfcpjx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xcmbivye.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3owwkjqij.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3srvgvjbl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3yxnnjlqk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3wusgrmyq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3iutdkrry.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3oymwhowd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uzpudyrz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3nrxbrihk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jisukdee.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3twiqczrb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rpoyqwtz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3oouqgbbt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3rpemzlwo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ikcpunle.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3badjotsu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3juwbmjwf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyyedbhn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sypvlggw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zsxophhm.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qunhnamb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mleuycdp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rpfwskga.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hhferpxe.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ylhjvnqo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyfbcnm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3absfbbem.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ctdorkom.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mmtlxqga.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3srsvwdwp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3wtggnvxu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hihosxnx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3obxjzvnr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3tnodhihv.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3zljtmsuj.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kmweeupw.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3qibnmtuj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qedfynpr.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3bicaiesp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gwkaqafu.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sievrdzm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vjkzpdeu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3mmcpsxph.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3wkurawfo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lnfdbbfh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pbbatwga.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xymfumhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ybgqwlwe.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3itnchwoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oupsdlnh.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ryxvfykr.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3vqgznovk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hplnattb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ooxwiwnk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3acgnscvd.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3nlnqmaiv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hvkldeqp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ppfhpywd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3birwlwdp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oakwqodt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zxjglhxy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3hwqsnsow.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pyslzmlq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ctnjlflc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dvgzltiu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kpygdohb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yjfujlnc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nuflgqrp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ilytxvoq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3afbzdbun.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3apoxyzjo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gjgbntmz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uwvkyteb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ohexnxlg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cyimnkbv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3xqbncyew.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cvxuwvya.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xphpkxgq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3aveamkqm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3vqefegkh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ddwxiaaj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3lblkcgxg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3yobsjkis.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ufmfrsrz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3delafoeo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wfphtrsg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dcewucyc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wedbbodx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kambbfmq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3baenhblx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yglxcumj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3klefwffh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ylyggaql.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3zflmfloo.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3oalbjlng.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gejvjbbc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3vgdqehrs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yazvzlcu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3yafxdfzn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ztlnpqic.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dembrsas.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3mzjxsvyi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bppadyhs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3okajenrv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lstapnyi.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ibznvgdp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3onqyklym.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dsksaeky.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tpikoqaz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nvobakbr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zftbwkud.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gptzbgun.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fdogcqru.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ksoonict.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3uupalwtt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kndmxguo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3hedreisj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ppyhkvtm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ilrdgbor.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xexjwbcz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rlemayxh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xckltion.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqenfygk.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cfqnjeig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvmqvyyj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3thpwjvge.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qycxuutd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3azraylme.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nwrcfhlq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3incdhdil.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nnboiokf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vwknxtve.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3qcwcnfya.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rehbcgwt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3bguniqbu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3viayphkp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zuiibigt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ytriqkdb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3bugjqltn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bvrowkws.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwfjlhpb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cnzrxoyl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ikylwlgs.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ezllslgm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3tswzrlra.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3kjorjcyf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lpnondyw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wcdyrgek.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3degzhfuu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3tylrnfim.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ytmxewqu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jjthdkqg.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3blpyotdr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sklhxsxq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3eaybnewp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tcwvfmmf.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hcmadjxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvguioaq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3xkjawleg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3smgehpwt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mkdzeevh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wwywqbmr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nsaxfwaq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3tqthgpbn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3oxnonthf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ouheieak.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lagobfwf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pwqsqpny.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3rpybtqos.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ragwyegx.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3dlsnfdzy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rsypxhoa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dltsdohe.html


<!-- 参考信息 -->