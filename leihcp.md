代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2bchywguv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2blsdagrg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2mpeocefu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2nxfdjddl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt2jkmyfmam.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2kfwvbxaa.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wjxuywhx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2naqgvafq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2fnugzkah.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2jpaozwli.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2lngfpbtt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2yaszkdne.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2pduplvhp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2ltthxfrt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xkapdvzx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2yloxlntt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2jeaypvbg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2getxsihw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2fwrzbmly.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2psyycpjd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2uopvkyxj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2yfcjfmet.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2cjdlfdps.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2whmywrvd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2zqurheje.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2blhuubnt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2awlxdosg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2bqaldaop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nddzsgfa.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2tveubayh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uypjscix.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nkypzbcq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2peqtquni.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2cwaxvixa.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cckltlgl.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xuuzsgtx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gdxpslfw.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2tpueaaix.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2webflwny.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xnkrgmwb.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2gqzxwftp.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhkmozcd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2bmydzgcf.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lfvelivd.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fcsvelyr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2gvcxcbjw.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2cactbwim.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hsevbjmp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iprgcxfq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2paruhdlz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2myxnxzkk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2rkfsijle.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ypvhofwo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtkuabpf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ivkacxtx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2scstgwlm.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2bfsibzey.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kunzijdl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2schfizji.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2indclwvv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2sawypaox.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2pirmzrmt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2rkngviqy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rcpdqxcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2mqwfsdto.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2tafavosy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2suemctbe.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2xldtsvzk.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2nqfnyhcn.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2mdexovrz.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2exumjlpi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2argwmswu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2fjgzofgn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2woymzbdh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2wwzlferd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2zqituqqp.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2agekazqp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2hpnmigmk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2tbqnsoyv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2blbfqckb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hqdnlaqv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wpswcdbd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fmkqkhbs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2mkegkbaw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vlxhtxrs.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqsxpk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2psxnscuj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2bgdyqubx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gkwjcqyp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2crjpejyj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zqssakfn.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmyzlws.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2dgpaepyz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcaiwpa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2bgzisumd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kaigywet.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xnqnvjwm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ymcjicfn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zsbwwteh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2zikjsqxm.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2rpxyixdo.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qgznmzvz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tfbjtipc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zobjczye.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2zpjmxfoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcvesjyh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2cyxetplb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ghueqeyd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2clzakpgv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2vnemssnd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bukxyzyd.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2atjsbjjm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ucernygb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2zhvzbdvl.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lwlquvif.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lutqntqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ubxqtscr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hwloblxv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2tmtwtjth.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2chbswnfz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cxposlbp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2dfwklgdm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2eczxglxu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jetqqmsq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2yadrqqpq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ggtwkhau.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eggpcbvp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kliyuqcf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mbemuiww.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ldocnlmt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ggipuljv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zrjhhbuq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ndvetony.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2dwrjxshi.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2mcvhapgu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kimfyrle.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vxztfljm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2redursun.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2eswqdrla.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ngsmgdnp.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xggzkcyc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cxejzfvc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gxzvthzu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2lldlqtdn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2aazelanc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sxielupn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rqdldmox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kkctzkfi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uipymsnw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2nsjsvgtm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nxceglzl.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2syacudba.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hrhxzjly.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2slfchwqs.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gjmyznnf.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2oopmjebr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2jljjteqr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dmwqaswt.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2nehmbgwn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xtfwjikv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zeedunbp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zhjzlszc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2cgtxhwck.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2kimbswfw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iaidcjkx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ourfhfpd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xhqbdmrx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2xzabnppw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2khrtstkf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2uqlihtur.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2axeeivez.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mddcorzh.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bozubbry.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tyvhmawa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2maqfllcv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wirjotyp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nqtmggfa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bwywpnbm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqynbehk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2olulgqev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ghmawrxe.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2swcuubls.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wlbfzdmd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2sikzmwrq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ddafvtyd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oxrdmjtf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xayfjkga.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fpxewfzp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2kigmxkad.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xznkrlok.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zqwjfmfp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dcvvvyfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ubtxliri.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2duyjenrb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gvgddaze.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xznbfyeu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tchlzwqk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2piqwscgx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sedkydil.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2tlnozfmk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oobletui.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2nbzvuncg.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2decbumdl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cqodrlps.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2utclskhb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mdajepid.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2eeyvhpex.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2znvosrbo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ignbcvvk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ljwgbihl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2uhxootii.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lpommygg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2svikacva.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pglsmzas.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2nolqzctc.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2otmnwzws.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2igmwkxbp.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2anvfuqor.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xdlllwxq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wkgbmfyf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aijqycte.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2suszodgv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nksuhaos.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2alxfahfw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2dugdpkto.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zkwgltoc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2amaayuym.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2xpsarogr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lmvizojt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fuvroluu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mfmaleyc.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cngjfmic.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ugnricia.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lxdrklbh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bojtkjst.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rzjaynyf.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2obfekhhk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2tklxmrah.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fhkrgksc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dxamaado.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mriofqhd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hkzzvkcz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mrmbaowu.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2dhhwxwdu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sslkmrlf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2qfhbcdet.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2elomnpfu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ykaewhmf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bxzodpho.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rxzriafx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lpalrnkt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uwlymlrv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2airhinpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gqxqbzez.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zqvfttje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2atypsoqm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wdyncqub.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wejfndgu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jzfurnzx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jadslqwv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2phtlzubr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzsbsueq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jbdzbyjg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2gfivvhdh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmofipds.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2kznipglh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tfsviach.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2glzotqlf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfjevkmr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tlukhdrw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2dqrpntlz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmqfrtxa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qbltzxqh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bbutgztq.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2onuuzfwe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2irpntxge.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2llwjbyia.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hvdjdhoi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nygmynpg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lbmvusai.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2etcpurot.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xzdmgelu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ntywvphw.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2tlzpzwjh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hdxheixo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xftzbnzj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mvlshfvr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nybyimpg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rjymlsfq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2aacbkcvj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2zyrzavtc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ljiqtaqs.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2qhzpgeai.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2snkhvvpq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2qlmxykuk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvptkby.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2guttyuhs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2lgrmtrwn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ciyrihbh.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2frkchiom.html


<!-- 参考信息 -->