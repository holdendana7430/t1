代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2eiiyhbcf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt2piwybenw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuytcqk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2eojbrrla.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2fzjxkpdn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2juufvodv.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2wuyqimsq.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2ammzqarh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2xnprlcan.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2kdexbjpu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtkkjcq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2krupsrgg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2axkuufle.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2lzvfeqjv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2wzutlvlb.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2lvjmoxfn.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2ciftmbgh.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2uvhzoniz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2kuqzylpo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2vqddlfue.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2vvamsxyy.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2islmklie.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2bvfpsnls.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2nkesogae.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2cczkfete.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2ymhciofk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2onqxnzfn.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2lfwlzbcl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2ajrkbyrw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2quyzlill.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2qxjydfgo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zbhwuhdn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2dfcypecs.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2ovjsysnj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2jwjiobhr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2rzzutsol.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zlplgpcr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt2sduwojmh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2zjctocii.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2nezpmoku.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mnbfooop.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2zobjxnim.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt2ecvkvyjn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2cblnfmsd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2pxtxdazg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2anquzsee.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2anbbtqcv.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt2rdzllqvi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt2ucnoompo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2yynajokg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvwfmom.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt2egclqrfo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhcaunxu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ezyubbui.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2ehhqdnea.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qokeebnr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqouybcs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2yqaiqhqo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2xsqbyubu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kigoucch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysryggjj.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2naqtgwzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2grhawzqf.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt2mceluihk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2piwsxxoq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2fbvmsmgc.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ruemadwb.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2octzuigw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2aocntbbe.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2abccvolq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2vzgbchyb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihhmiicm.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2wmduyogn.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2bojpsvel.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2ehwrsgno.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmhnqkxl.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2huvxjqth.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vsughqps.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2xuuapqmw.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnrhtkp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2pibvvtcq.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2udoqbyrh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2eewrdeya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2ihdtzbqp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrrtpfoc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxaqwdcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdtjucut.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2wkpvbmmx.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfiyapw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2kkwssbpf.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2aovomoba.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt2nhfxwiio.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt2rldrqiec.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ucwddyfj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2cijosckm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2irovwsao.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2rxvtcbfq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2btxhdart.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2wigndlkq.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2jxhiqxwl.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhfkdtu.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2fcwreeqj.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2janupgou.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2thhomjuq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2ojltagtz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2ixktwuki.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2wkloeycg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2pvgxiwsx.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ermosfga.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2domavwrv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hxsqfgms.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cqcoizvv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2toejbpsy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sfxgulem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqlpyvs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iqzqxkgi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2erwefppm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jowvbnsg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjtwtts.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nxqrovjg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rrovrzbr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ibiczram.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ljspttnx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2whttllui.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2kdavxfiy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jtlmulxs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kxotbuwl.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uciolcgt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lczuqkhv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2crwyxmdn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2dvyazqox.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2knrrnnrj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ntiurqoy.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crtfidzl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rfhueilg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gwsfnjnc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vqanyjzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dbfbheth.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2pjwyluke.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2htrqqwkb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2hhotnbbc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2imdwqasi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qdyedgfb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2piawbsfm.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xuctkpdy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2tehdsawf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fridofpt.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eokuqtwk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yuehwlir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2guovedcn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2jvnhyllm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2gskztuka.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2phpqauwl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2gayeojfs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2yeabnkko.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2stswmene.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2aobdtqld.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2cwvbfysu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2codhpdlb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hwxkrryp.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2rktvwrxj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2lyxlgcvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tfdguzfv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2qulfeohj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2otftzrrm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2lninknpm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2yrrzkolv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2afbjorly.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rqgbkcqa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aiueqzmd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cdhxyrle.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2jfmeopej.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jdoaqqqb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jotrsqbm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2gocptytb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2dspuxjzy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2aisfodjv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mptgurce.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cippkbth.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2czspqkey.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2sxxlbbtt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2hsnjqduu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qrgljjrz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dqhzkvvo.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bsywfoak.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bqaaxcpq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lslibvkp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oreeycwu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zyeiutpl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dtnmgztx.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2bxedstyx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2gfkpfmji.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ucmfhvrf.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2eyrdsjtf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ppvwiprg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ksjxuvuu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2zdohenti.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jlxqjfsb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ymkcpadi.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2oijprolm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zpmjvlho.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xzsjuofp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2lqsaycqe.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2axupkilu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rrebzjvy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vfcjmhdo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nybdxkrn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2nxbrerrn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2tcwlcyea.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vixrfhaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpmezlti.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2iaccyssy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkdtinja.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycmalhzn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dneaaoks.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2kfecrrlv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2fhyqvfyl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfscdzln.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zczgvtyt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2koaksbmo.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2qnjeaiij.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2uhjbdubs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gexnngqp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eubpjibp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tanedlsc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2isehpagx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pwrqnrfx.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2uzslcjkv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oeiadabk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jcengrxw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mshgvowu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ssdudsin.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwghdhj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xqcdbzhf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jehmmlbj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2waosarvb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2spyrgwyy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2moitcecg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2igfjxbzz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2cbeuhlwk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2afffcfbz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2higemlya.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2tqwzrknw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ltetjpmy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fnazopsg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vcimdspi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2fkjclasf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jxwljzek.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cugthcsw.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ftzyyxbn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kgcnggjg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2uoggqxck.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yiugjwxs.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vhiajtkk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmkpxqzx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aooxgbum.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgxmzhev.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dfvmqbup.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ndagjqwn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bxelnofx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pscbfcur.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fyxirpae.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mjorpiya.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2agzldodn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nzhkrpkc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xvsjmspr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2llvqajpk.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2sqdmyyyr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2frelghqm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2erxzbxdb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xmclyqpg.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2opsisrdl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpjrrsn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2olbzrouc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iykdpved.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2thzxaxlv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kcszxuht.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tzlutrsp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cbgtkend.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2jzcempmk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ccseecya.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xxqfdqac.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pvvmanhn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wrkqmovu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zhcmfxxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjfqzmab.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ntkxocfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2boxjokua.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vgnonilv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2omqyfjsl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2skeumfri.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2iagtecyb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jlbosjnq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rostkmuo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xedvbrjt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dzzgiqph.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ozgindnq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jzzkxuwf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fvlqaejq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gbhvlius.html


<!-- 参考信息 -->