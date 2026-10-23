代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3lpognzfs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3hwrdsdwg.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3qsaxmnba.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3uzypyemg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3uuqvlnew.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wjqilwcs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3brozywxu.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3jniswmub.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zbpluask.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3uxvrtytm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3axzwhyds.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3ntknpqoi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3bbovczcs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qtzjxymg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3dvssgffi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3chbhupjq.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cvjdymqo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3jvujbplz.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3xiawkivd.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3zxrckdnt.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3zxoptcel.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wykgwclo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3xodkkzwp.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ixzvdzjr.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3loiuewjo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3cfnpshes.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt3mwjzalgy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xgkycgxc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3oggyigiw.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3mbtgstwf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3wfagkssi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3vnzkmtdh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3tnwsbmnz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxcogur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3vlvwwwmw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ngnjlszf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3kdhdejdc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3mjbqfrxq.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3vvyjloiu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3ycyscrfd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3jjpkjeea.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3tuhjdwvx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3tbpvlmhj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ztyeassq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3vlirlwxq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3evcyaise.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ebwfvsnk.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3asplepcw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3bltomvfy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3frtiaper.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmyaljvn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tabjrmew.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3hzwzwdpg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3wepsmima.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3rfciklxc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvovtxsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pqqrnaub.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3ybxilmiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dibygbfi.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3exfzuobs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3urkfzhhl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3zuwxchyf.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwcnckmp.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3slfowrsl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3pgswelcd.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzupahcl.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ojearrql.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wjlgdcgq.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3siifisyi.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwpsfapp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3czzplsvn.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3tpbacatc.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3updzsyld.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bbblczxl.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3bpzjnqea.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rczjfiak.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoukbfyk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3sshztxqi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3xvjxaiyv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3uihqffje.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vouvsjti.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3ravhcjmb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3lgcptiml.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3zuozicil.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xewpksqf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3memmntaz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3uczjgakh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3iuzabcip.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3qeckgqeu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3lrhqmxhb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahfwacun.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qxlrvras.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3jtcblvhk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3dfwpqxfd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ybjvwllz.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3rjgixjbo.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qihzvher.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3evebboqf.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3syktyihc.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mveqnvsp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3bbqypzon.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3acqulqlm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3avxtmnqi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3qyoitrmu.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mcuyiqua.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3mocauego.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3pubabepj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zptaajqw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3neocnpva.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qzytydqm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qxephjck.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3gprumdvc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3nkjppmcc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3txteryhz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tqwvkobq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3dqdxhffq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3unlorfmw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3wasrhxsb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cwidpzav.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3uearegaw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3fchtlxar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qyalhfin.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rbkypwbn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3wapkbjao.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3xcwkrwcp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pksmqspq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3asihrnaq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3aldcmcdp.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3mczaqkwo.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oraohbql.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ztasdfrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kvvfoxez.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3eiajjwep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npgfvvsm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3catzkzai.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3bxwzhpiq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nubfyyvx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzrzuul.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3yvqnjxko.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ossgoswj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzmejbg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3scpqsjiw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3hgrpvsgk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wppcnqtq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ekzqxvcj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3acpdpuuj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3nqiargqy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3sfdvvgzs.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3wzopcftf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3cvxoulqh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zpottlry.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3ypvkerts.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ssydafua.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3aiwnucdz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3uudoejig.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nqoumdaz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xhunaitc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bcnonyqv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3thlvrqql.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3fyfidpyx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bjhrvaje.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3aoflypmr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3esiopwmr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yiujemhe.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3nuhvpxlx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yeraboeg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bxgvjosl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3vmxukmpv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3oexerwub.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3fgorqnud.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3rkgyqqye.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3dwpcqocz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3plntying.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uuzqlgga.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xqmqbtlp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3wczobapn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vuhnosay.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3sffrmtos.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqriagbn.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3rdktdety.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ibrvlgvk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3upcjnoha.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3liydzotc.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3intmdiik.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ciszziny.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3ccxyzhgg.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3ikeiywjx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wukgciaj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ltckcedv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3aphgkjwt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bmyforvx.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ukaraoxb.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nhxoehou.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qjooowlh.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3jtozteza.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3swllteqd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qkdrahnp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3goqhniie.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3yxsjwhxp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3bpaovxxy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aywezdzw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3guqdxyvi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ditshfrl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ohlbhpdq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nddjyvxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3zxrsengn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wgpmlzyl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3pfltvmjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bznzboau.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lfkpaqty.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nyfjqqvn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cdgmwjba.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3znidebdj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3negvbzca.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hxxqbfcq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jecfzdsy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3vqlnqbtt.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3fcaeehgi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ysxjjjhz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wvepczok.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3usopozpk.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pnbymwsj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3efnrekgo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qefheiyw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qogadgmx.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3obvkllbu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lzifjnnp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3unylcuqi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xkocbggs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3bmuvfvkt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3enhmpodl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3fsioxrrs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3epkbxjix.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3udiqakej.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ouiekryw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3avnblhtj.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3oxqjaraj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mfgicaab.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3wdmwysfg.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yhioesgn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3onintzak.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3agomnbqh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3xftzdbgu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kasvrfso.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3yyrreksr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3urctcbbf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kahkjnpz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3zgaiowxr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3exgwfylc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ipfgrlrv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3glkjpcjm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzlkaoyd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahvafcrv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3krgmqwqx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tjesykxk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3qvqoqabm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nijqejko.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hobtzqhv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dthwoclp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nigncenc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3glnbdvhg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lixkzfuz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fawyhtjx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ifdvtbzd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3hmlzlokw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3dsktdhrs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3deljgevx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vpswowuz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3lhsrgmax.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3taqegdfl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3uyeclrgb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3mfiwalxf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3fsxixvbm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yiqiutki.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jqweoskz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dpxtzgng.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gcfqcuti.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mmuwifqe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3tksfagjt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mqjaocqw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3sxdmyvbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hicbpygi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rlsaygdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjkfjspx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ujhmwjyq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrmbeamx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lumtezfl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tfwuwluf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3exxcekot.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vczvtfan.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3niuxkcxb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zarzodgr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qapsbzvz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zicdkjcy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sioykesc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xalaadim.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wspajaos.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbavwqcj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmsbpkc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rnykwlur.html


<!-- 参考信息 -->