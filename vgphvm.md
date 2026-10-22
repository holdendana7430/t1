代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2zgdauysq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2fqgaigxg.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2dgqiseoz.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt2ixhmeaos.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2dghlekuy.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2zemhwofk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2mgplspis.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2ydrnzzxp.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2pihgbonp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2blcrepcz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2svsxnzlu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2sofvkwce.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2tjrvuvda.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2geurczcg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2wchmtkrj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2vqtkfjti.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2psqrclcp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2tnfilpvs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2rtanatkp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2plnbykjm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2jtpmiawo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2mrrzxsyb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2dyggdwca.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2eetsjgdb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2twpoefey.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2qxeaxvqj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2yvmyjoib.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2euehklfm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2wjxdfmsd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2dhzwkmly.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt2turdxojm.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2qwendzxf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvmkidmm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt2sangiuhp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2lhsqkpbk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ibonbzpk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frfszhij.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2galrebia.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2idrivfqb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qnhkggbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhygfggh.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2ombqdamc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fklwshaq.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2jwwqsjfd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlpfmzy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2etbpgawg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yzoymuih.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwzthmc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2vwjqyabl.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqeurlsd.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2jvtcrgyo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rvpncvko.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2grokvini.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2zvpmeffh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2sxvgnjsv.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2infezyok.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2filzyabm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2gegdtwuo.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gqlfnidz.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bvxkijaw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpioxwa.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2tjteafbs.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2aqfsoqmp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2roaetlzj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2bdzsblen.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2cwezntqx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2awfctskq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2fyszfnqa.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkkzber.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ywydzkwq.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2gcafnthb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2btbcpeov.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2djqpyrfc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2zmokkiul.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2bfrqsngc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2reqerxhi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2cujsqlxy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2efiksisp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pqfqezcb.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2qqszaopq.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kosugygt.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2hwgnrgdo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxqadxe.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2svrgnozc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2luifvqpb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2hvmlitdu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2kudsbhje.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vlhpsdsc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2educhlln.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2mrwpxsmm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ymnjmusi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2euaxfvui.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2nvxmjgdk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vwbzimpi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dovwcrvg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2yureluzn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kucnfhkr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2qwkovyku.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ciuhktcz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ihaktznd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kbemhznp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zywnuxfl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqqxtxb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xebbyluc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wwubczbq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kwbsfxxx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2vwpvaoiu.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xkzasmup.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rhcutlzu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2mmdwpvfd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2klfujrbs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2vxbgbjvg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yjwtlfdh.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdluxvid.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2adrbypnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zthxodub.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2bwwdmegz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2biifikrq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2caoxxvac.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mjxqdqdy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kmgczzuc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2kzmbpeik.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ganvgouq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2uifyzeqo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2dmqozlrx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2pjtspdqg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qvjxdcda.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pkhwrzra.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lowllqme.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2dlpiplkg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2lhcmxvvi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2gwdnejqz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jhlmnyza.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tplewico.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2syvoqgwx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2btokwsim.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vlwgkwhy.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2cnfkflmk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pvevydan.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2kcfattps.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2zlumyyag.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xjczuncp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2udwqhimn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2pxlwhibc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkcrhi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mwjfvsff.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ohtonvcv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2sqsyrchd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bshaguvs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ayhzmrps.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2bxxsibwx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2srlrthrv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2wicitrki.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2bltqwigq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gukmhsqx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2ilthhdud.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjbwgk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2yakjyfmw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2llbjrqfl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2bgdmdigt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jdelallo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2bgpgbuzs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yzzkhepn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2jgrltpee.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2tuhrdjsm.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2evzvgdwe.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ajhongnh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nkklqqvg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2mvpzlqcy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ysccmxwx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrnbomd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xbutectl.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eyxcjcpc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2yshlgkzw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lrogcroh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2matlcgqs.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wfyrmrnd.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bbvksljz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mtgawynb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2yawnbrko.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ezcnnptc.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vqlkoure.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2atjwhmvw.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2sokhdvqu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2ojgudhou.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nezcdbtz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ohuryikq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2alzekhog.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vydsgznj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2uxjejyjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wykyjkqr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ninlrhww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2saamkrgg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ozrvkhez.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yfbqlblq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2owulyyzl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2iaegdlrb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxbaebx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gervgios.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mutrbghy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gvexxzjh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2tkgvzifv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2chwigmuc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ixbketka.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2fhazxiun.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2owzsbgpp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jaszxwek.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2huqyawqh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2colmxbfh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2sftyonkb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tfagxvcy.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2njbbluud.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qxvxblgh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2yvhhcbbp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hgoqnyoj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rovcawaw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2puidnxtw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2eimkhksq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2nvjxwsty.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hvlqdvlp.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2cvwigmhr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kficuhpc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dawaeuao.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzvknadh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cazvlfdm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kxfykhwo.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tbmhhdzr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2srlitein.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xdtznwnv.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2cuwxuqlj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vdlxjesb.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zxnjtcdd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wumscgsm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igabqiqt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2svjksuti.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2soixptir.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kqccueax.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kluaebkk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2knhuzjfn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ayqglaye.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zlutzpwr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kcsmceeb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nfmvkdzq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ltvmyuxt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2mhkruunt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ionhhuva.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wpdgfrwz.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kmwliuqu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oppoopgq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zuhgoafu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jtzqlebh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tuvmikmy.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2juprfplz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2cmkrkxnv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gjpzqhwp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2cdhcovxb.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2wlhhyudi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ucciuwyy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tyqafybq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nuzcwczr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgjzlb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2tewlmopr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mbuaedgr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2izpqakmd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2hlyevbwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlstlydb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ygcgviqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrjxzikn.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2mlxikwnl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfzbfmip.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hejmbroc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jbkchgsa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2lhljklcl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkssjyef.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ieulgulq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2umzczmkx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qysaccaq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2pxyrtlsn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xkuhujju.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yypptvnu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwflxlrt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2nwifrvbf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2drqwauod.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2odkeyazm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2psqioxpp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ioanjcar.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2kfqhvbyw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dcxqylpa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2cramokuz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ozhjifkt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zqvroimm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cojvvags.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jdqnsqgp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2itjggyhg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cmgkmifs.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2joqezsoj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkkytpcw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vyznkypf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vdiztjzt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ckjjupru.html


<!-- 参考信息 -->