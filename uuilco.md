代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3atfbbiwd.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3drbcggso.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3qxcckswp.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3yxewdqob.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dyoivayb.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3rfnsnfyi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3metstbov.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3kzhczeze.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3admoaopz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3kwrbyfcb.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3giowqnak.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3bqeimcjs.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3bislialc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rclljtty.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3eaxweofs.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3rtkeutfx.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yioiztqe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydedljny.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxigbvrp.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3hagiwbwc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3rsaulmod.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3juyasddw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3lnndwsyu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3txdmneui.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3vpvjqtkj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3svwxirfw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3suwnihkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3bpqflzlh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3evvoggyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3mzokblsa.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3ocgvumju.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3knaohrof.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3qkgpfffa.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ezaxdjso.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3bibrrjqy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3resskgci.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3frqxfppv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3kccuohxf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3nbhkebuu.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3joojhljt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3ksdmsqwc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qosdflxh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3fggswzno.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gvcgmikq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clpbwamm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3gfqaynmx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3josyaxlj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfmivwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aapoahjc.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3vsoihtxo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhavhfgv.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3slmmhunv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3piosmahj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xdjmtagm.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uffxqvnt.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3byukscmp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3nvfknejs.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3yruqztlt.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3quogcnyc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dpmgsgjc.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xbxywpvs.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mxasqapd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rifkzrnp.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3thzsecij.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3xeoqvjgr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ivqlxifv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zjbqhdbv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fwadfstz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkfurpav.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3qaspelxt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xusccnst.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3oikygbvr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3zihdjhyo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3vjenogqi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcnqeokm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3bshoezos.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3ynvgsntc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3aovcyyqk.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpzsissw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3pmhfxnzc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3upvybncv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3kdctqstx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3gygvwuxz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3huejshsy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3zyiucleq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mnrhzczs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3wqdafppn.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3pbqldnws.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3ozgesofh.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3dzckloqc.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dqkbaxwi.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acqcxxbm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3axmyhtcs.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3woztmima.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3yabuoxly.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3yuejbaks.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ripnkcar.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bomajluz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zsajsbtr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qumumiat.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zqvezwoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3jfrtkgxe.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3riexpxsf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3xwlumjrb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fvowafyp.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kaznxvvb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xtwqrfoc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3inezgvsl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnckmfr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3exnpnetw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nlsjbves.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3idhcrvoc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rolbprzz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvngjke.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3xhjmegbj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yzgmwehi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zolakofw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3piwrrxhx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zlotgzbl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3kwtpevxe.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3jvjqdpic.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbngsvsf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3skqqhpxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsdshgcc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3rpdkmnej.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vwkhyrqh.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3rrsyytmg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3rkwicdpe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3auujkbat.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxxvrxb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqrpuip.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lbcaauxb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3uwjolwrv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3kyvwjunm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3sdhmkuhc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tfosfdwo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3puudwupa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3elycjxqo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ithhrmxw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3puidrgsm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3yggufqwu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3pyxicclu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3bbtyixuz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vlkgdtpz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3mhizimfh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3zigdisra.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3evpkzkuq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3yxwdonha.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3fkvnctsh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3jplazaur.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bienwpeb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3hsmuorbu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vdpmfsng.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3rpopatxe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3skxvorew.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3rysfqjyz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3xltaboni.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mmulmxbl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3hgncizew.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ppnllwfb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3loplhtei.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ekiwnvei.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3caigomql.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3gxuauuyx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3bwjefkei.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3wkyhypod.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3erfdzxbd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wfbgubow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yxeeqvjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3osrqueks.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwjrwawi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ewgeukkw.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3oapanaet.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bpsxqame.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jtwmmpft.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pddteled.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nbmnpegf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3pfessunz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3tnyfsaiq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3oymaqxzo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3izvndlmn.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3crmzgesh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jngrigll.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3vjndjuov.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3gcjjtjyn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3wiocwpra.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qorewlwc.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cucajtct.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nkejhitp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3zgsdpbub.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3xaqtrmqi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wgekttbk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mijwpmxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3njzinsib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3thdpyeek.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nxakzzyx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xleozhxm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3whpsjxus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjdqruuh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ehknclct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3woxajurq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3eoozfmrr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uhqvfkjz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ecpljsfs.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hspyqyka.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3szsrlmxk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3orjqzumk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ztsexcmh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nxdmiowi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fcvlvrfb.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3zbriagdx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fqugdaww.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3vtuvegcm.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zqcgdcsh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vdodzeab.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cpexmaxp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ibpngbiz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3vlovjxjk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xdnspdai.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3mrpipezx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3diyujrta.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3korcrhnr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ffbppvnx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ywhsyipb.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3lyqsheyv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3btqzvlqq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hxmsgbti.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vanxvibc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3zbvsmtjn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3qkldnljn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xrytziow.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3fwpnexua.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3mkqjcjso.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3srjmbrwr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3djkmmbzd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3eduwwtiy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vheozlmg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3etxpmrbh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mqypuqog.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3azxoexoe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gewcxgax.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kazvunnn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkurnrg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhpafx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3wyjctiku.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3eadmigfc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pnwyuood.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xodevbwy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gxotophc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3umrbrlfk.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dutfbiob.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kknnvzcl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3kphzwigc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pjisxdfz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3plfksdnb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bwvgdrry.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3binvdvfj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3pkmckjep.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ypjrlbdy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gnzfnljv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3yokifhpm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3fzezekbn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zfefbocx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kbvvsuuf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jmqzbfym.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xgndyjge.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3nsqopsrg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3xdoathko.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3egbdoiro.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3fgmdzyoh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3zaeradey.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3suezcnvm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3clpygtap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgwayanp.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3kbadqeri.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3efyfnovg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3chuvlbqo.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ntnnlcpb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3vnicfkof.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cyrljwsw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iwpxhkju.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xjoplmdp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3iygozojt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ajpuhvah.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3luihmpvv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3imihtwww.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fiavksxe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3hjaqxhxo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nednduxg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3duletnsw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ycalskxy.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwfegbnz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wvojkpqj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3gwnwboyh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3belcmnwj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3etlbzfft.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ifixpgex.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3oehfzctn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ozpiccfk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jetbowqh.html


<!-- 参考信息 -->