代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3qetaslzk.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vewdtkcl.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ktfdwfqr.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3aarvdhtf.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3qmiiwjfj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3xoskzmsc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3eybvopwa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3dtlewwqn.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3uyjjegfq.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3gsrjwzrf.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ffpoufil.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3kfolkpbt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3mavsczee.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dcvechxm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3tqlqhimc.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3dmyroyzg.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bvhprsbo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3zxvwwpyc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3ceteywap.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3ylphsvop.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3hloxxtsx.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3tmnaqdcz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3avclyiuj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rqifhuji.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3bjeeydlp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3eunviunw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3izpninkj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3zvpavhmh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3nskytpca.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3ywpmirmy.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3seuzddvp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3zctotjmo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3ftwtnrrg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3abritpxn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3ksniczkp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3rygljcxy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3gaguqhoy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3widbwhwf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3zvzspvwr.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3eydtraym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3pldlklzp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kwejmjso.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eouoacic.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bmzeeohh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3osdalmqs.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3bvopedye.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3zmzfwhlq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3hzotzihh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3klxxdgkj.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3jeymbwvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jfammdgr.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xthrhwrf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3nrscznqb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3gclqdeeg.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nberfrok.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vvgevlbu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3ljaozrjq.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqgmjdo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3melnkges.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmmjxlj.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3oddnoyei.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3bbhvyiof.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3slvgbwlo.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcoyvfly.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vghtpcxk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jbsouftj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3sklrhofj.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzpzvfz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3gufnpjqb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3tumujidr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlkrrqb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3vxffirze.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntuhypmw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vabzjwat.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3fshkjace.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3vpoghqqe.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3udvvejak.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3hvxedzqo.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3twseamvd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lqitlepc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3lpijlakx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lluruziz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3viasqbzu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ahonzklz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3idifiznm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3ezatcanl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3fwjtpewe.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3bnquhtdd.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3acgnadur.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3lkwgyjqh.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mbovjngm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3ckdlayda.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3qkwvmvnz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ynrljdfb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ajihavae.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3bcmxniaa.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3pxchgbav.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3upqenyeq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zxizwpoo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tpjywslf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jphkgjjl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3rlwpsjpk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ezhzpomy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nqhdkych.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tsrnwexn.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ichigfme.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hejutmxu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3gwdtgjrg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xbkmgjsk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hxpfyxxr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kekumnle.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3phsmwyvf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fqrwytip.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mztzondg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oxracwco.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jnnedasg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3npddgwcw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3moqkotko.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3iypccrdr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3niuywqff.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nvhfchvb.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwjdxmq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yxvjljab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovtpughz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yaavwvxt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nnnqburr.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3chcfxhsg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3zuhpzvef.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3bomwnlof.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xjrbtndw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ektnwnsr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3cfdtaadm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3lwpexaun.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ulhiuxau.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jphhaurd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rrmptdlj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hytdipqw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3gbolvgwj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3wqxaxbht.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3shjcksnt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3joxhbjsp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3gchgtnsv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ytbhooia.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qfqkwiiu.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ebzywoik.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3psblposc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nuueomzh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rostsiuu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3odofpwnc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ocoogqpn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xossndaj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ticjjans.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kkhlryvm.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nrgasliz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3zzmgqbyz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3idovkkcv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3hgithkkv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3lcpedgvo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ztpgnvns.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3fjixbxmk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3kaoydrmo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3qdzeufyj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lhufzpnt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3notuifvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3wyjqivol.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rcpfzjjh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xmvlpisq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3itnsvkjz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3pvdelrvj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xenosxif.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3muaoecwd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rvlsofph.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3mkgwsavp.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3yoecxbco.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nxmjpvge.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zfkfmywm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uzgxmprm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fmngugty.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ppderpan.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3jhjhcmjy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3dtufuixl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vuovmtau.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3fqkiagfw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vwfmmwps.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mhmhnbdz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3bqefftnh.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qyovlgvz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3pimtoakh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3zakosktz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hdkvuwxp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3mvenjpgr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fzkoxchd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wgezbxjk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3pqfzggdg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3csitlotq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hyiwafqb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zffckvto.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3kugpsyvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nslshcwy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hahotart.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzcgheba.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iylwkpmj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3syaidovu.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pzskucll.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmivluui.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdyavja.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3rxubfcvh.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dksmskns.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hvbsfjfd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bzixhoba.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nrunidle.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qssbhdnk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3shupgjbq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wwzbrtnl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ywgutezc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3btkfppmx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ebojojtg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hlgsfhjk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qbarkzya.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3saoebpwg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zuvltgcn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wjxhumpf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rufvtrpi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dnjytqdn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ofxyrwhz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3fajocwvv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3mvcudijo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3njyelcpn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3wsiafwlq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3najhbcpc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3veerypcw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wmluasqk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fmveuqma.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3bnzfdwds.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gtvnruah.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fqeavtxv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3tdwwdtna.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkpcmy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kwxuwbal.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dveizdkn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tadlmysc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3esduivpq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhxgdpkm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3icgqugvy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3puazhquk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3qhsrqwiw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3bifnuzjb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvpzotu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uywnubuw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3intptqhu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3oncbomgg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oviepiai.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bsadrwsp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3dxoetztz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sioeocyy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ofsbgfrm.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ecthyyrb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ztsdcyhp.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xklqhozv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3msfwzgmn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pmwoizgp.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ssxodbcy.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3lxxuoizp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3zfgunxag.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3knmlnxof.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3znzolxlp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3kjjatakz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ucfqqozg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yxybbpvz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3cslvgbjc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wlikqnzu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3isrlqxsp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jvqdudnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwswkrvx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3noflmbqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynyuvwfl.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jloztiwd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3edxsqkwg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zpddnhmm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xbrddakz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bnonfcpb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wpgioeyu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3enmcfxct.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3hwkxlmzz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3waqyoase.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3mwyfsoug.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3urnbnslm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hqlrnavz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ysdkvbee.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3cpzpdzgz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ipfgrewj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avfetlgk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3boouhjnu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3zpxogeuo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3scqwxrfw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ujjmspzh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3ibxmltnf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3krtocejv.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mavlflvt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3lhuaidea.html


<!-- 参考信息 -->