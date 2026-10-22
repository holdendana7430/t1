代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2qgpqqmcl.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2acmsarej.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2zhgnvlyu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2avxjckjn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2riyofisx.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2jleexaal.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2hdpjfszy.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2uycutmnb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2rxnhviuc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ezlauqee.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2dvocusqi.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ybrbcczn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2kdvekjdn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2rmaxehyn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2idofwmhy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2hhsnrwyn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2kcuyrddd.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wxeakizi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2zlkxfjsx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2nxavrghs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2ugnwyows.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2rparoqhh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2wmdqhjka.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2bpoypuga.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2xbuemdat.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2iumlreyc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2jrxrhzwb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkdtggt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2esahjlzk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2vxpvdlka.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2irvgtpsb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2dhsyzvto.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2icwzqikp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2vjjyuakj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2hfutkmkh.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2vvqlqjtb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2empkclbq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2byccmvmk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2wrbngfxb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ufzwzgje.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jnbnrqhl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2wxggqlmf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2kolzuuxk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qecmwnwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epjutxch.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2oraxvhtb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xluxquga.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vchivdwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2inemcnck.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bgxtqllx.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrngxhxy.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2thkoghzx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vchzinxa.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxfervz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vergpucs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnfixtwj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2lvhcckzo.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2jpcdfuez.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2fdloktpe.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otfnnsmn.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2coexcqvb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lnldzdqq.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2whakwmaq.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpddqgi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egbaoxzj.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2ptntlmoa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2obhbacnf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2fbdrexwb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwvysqf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2stvaeafo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gaiezsyx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2phlvowmu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsjndacr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2scunnero.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ikuniefb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2threatct.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2xbtepzhe.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2fjbmolqh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2avjxjaca.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2rzymbeza.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmucdbw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xwhwnfzf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkjspipi.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2bmaqitkx.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2oleqvtuo.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2iakrbjwt.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2apefdfdx.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmpgzwrr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2tbwlvbtg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2jmamjqcu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2ndsjnnpo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2dkwahbsc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ocfpyjjl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rgapkzvm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2zmxhzbbp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2igagjpzw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2puazhmeq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xpadqosv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2bsjaynwd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2unxcbzgn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pwlulvwv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2mijljeir.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2puogppoo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2efxsaqek.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpioekpt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mhqzcwhk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dfemjkiv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2iszidpts.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kxngijzv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pfwizqtc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2litkrgjh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjhksjh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zecninvx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cwrcusor.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vodhrewe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xngqfbyd.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2gkzqlkep.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vxkpiofw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mkfzaeeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onxjavyy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cmqxptuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uujtxezk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2styvwdgz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2rssrmegw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2paheubux.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjejwrj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qpiavfyi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2kupbkhub.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gamxvcfv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2tceigxmg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ybcwlkxo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2fiywiwhu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vnnpuqyc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jpwonchv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qtuarhbh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gpqkveil.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2unlfpzsk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2hvmcrrtg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtftpbs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzpwvgis.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vpqbvlfw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eexirfgn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wjunaxev.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oqlzmshq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zaotfgft.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yjcglhnn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2debzetlv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lbquymeo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2aaewckwe.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2ytlpekvb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ftdjqjpf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2hctxupfw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kttnckuf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rkqrxzsf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2gagdfept.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2bvwcqvzh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2rdidaomc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nwqesxtt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rmhwsvtz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2scksgaux.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lneapbja.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rztffjst.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2lzypopng.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ksmcvgpr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vomtbzst.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iyvxlmtk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zpgqxkeg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2olekrmim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ijsnxdbj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2gdbzxidr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wnjkqlue.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rqdsodnn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nglbiaog.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2szeufdyv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2redzqrrk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jayjfdub.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tvazszsk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2gidqxttj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fnisqzbq.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kkhxcgxs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fsgkilby.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wvaabbop.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xqldxucj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnqett.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lrgpfmdv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2dmxgglal.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2zdemiiqy.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2hqtmbrkk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ujhvylwj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2caogsapj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2immpcfgf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2aambzmnm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vtuilzgx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2awtpmfak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhnddzgc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2nzoteidf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vowfdgha.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2scxoerch.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2malmpjeu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2wdzgkpsn.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tsycgull.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2sgqhtkfu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ywnftyeo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gclmhmfa.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hmyxzoaf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oqbbmlqk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2cmcqicfu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hpewjmab.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2reyfebvn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zjfzxcrf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2abbfwlzd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ethullyi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jxvgjoxe.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dyyujwsj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2udtrsfqf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2rwspuhzo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qwdcvepn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2okbytglz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2blqpswjn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ivizomrg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2pmidrgzi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kbsllowx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pfgudlpi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2fktrigbc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2dibxtxhy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2wbdceqhl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2gbirongc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mzxyrswd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2feaabijs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qrsdhzcd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2lbhxablo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fkxuwaxu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ztuscgan.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2frcppyre.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjmvwtfz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2mnpptuxr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yvmylyhu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pumbmxsd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hwulshnn.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fwvrrfqt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2twaatunc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kxcsjhtj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zomexbhd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2apspdhem.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mzqpsiux.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bfvczcoc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfurazs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xmtktdrv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bxpzbpvw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2eqdqbddz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2eosmxuur.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2qvquxqye.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2vgmdpvnb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ctszmtnz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2npssehmz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2inqgqgzp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2acinyzpu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qnxfdaqh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2daolygwo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2rvitazfz.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2zonprcyx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ugskltja.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tptklkgf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2iovfgues.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rxofcutf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmdvcsk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cbfoldte.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2vahahmfq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vqridkbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxtgfweh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ttxckduz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avxsgwdv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2sxbzhdba.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttfkugjq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bcdlnnxl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wzhvidwd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qgjfddze.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uhdqxazg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqnwkaxy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hziwzmyb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ztylttxx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mwbrychl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2soqrbluk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2sopefzps.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfyfwmmy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gchfcgfo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fzglvxql.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2amhgdizx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hojfxwtq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gcmzoabb.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ykribzod.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2hbaqquvo.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2xpdwaliu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eqmrnkdy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wfchvazl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2auiuxlfw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jrexxlcl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vntlawrt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dohzfxkb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2gjayklyl.html


<!-- 参考信息 -->