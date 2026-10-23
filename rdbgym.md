代发 wailian999

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3fsfuznhi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3lpsnyabg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3awkduxld.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mkqefnpy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3vjmhvbcn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cibzzxkp.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3snnlsxmc.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3yzknrxkw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3wppfuvch.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ysfamsqn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3ljvarlcy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3ljkkqzcs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3jnwiijfu.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt3jzeueqvn.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3uehuwzzb.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3sjgeelgi.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3cayxhmmm.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3hicfqsrl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3rxhgisim.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3txxhtkow.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3qrgbqktk.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3fuwqrcay.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3drfplskq.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3rhptualu.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3hnaqwptd.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3wakhzouo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3bjckegwv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3chjiwzgn.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ipysxnqm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3ignhddgg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxuxfrpy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3dylyiwpx.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3drxauleu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3holzhodf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3oxdqwurh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3jwsnumtp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3cnmsodhx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3muzdbloz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3bzegmpmp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3djsjtazm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3szjyalqi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3nyvbfwva.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3jhropirg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jcohutqa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3hmdmyjsu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3vbvtmpst.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3jzfqwwaz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrxriit.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3qhsqyfzt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3cmdojwpl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3dyfvbzrd.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3zfkugpfn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3heudnfyn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3hxooxabg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ffofizut.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtlaiwhc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3xdgmxlcd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3qpfouwpn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3svjsjgcd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kokuiavo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dmawsrax.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3wjgipadw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qofsgiho.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3elacdsnr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3mpsvxgws.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ngquizjb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3azvpgmpi.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3fllhiycd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3tiqqbkcw.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nbgwbyyu.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3bsnkgrjk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wgxzgknj.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3tmkimklw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3gxqicuob.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3gjzakean.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3udxkorlr.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3cljwwcfv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3arsloeix.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3goqruqir.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3wlaktczp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywdvlfjd.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3fkzfvkso.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3ximmrqmz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3rqavhtby.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lxuelbnl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fxpnuhep.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3ngxeqxzz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ufcwxtmg.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3qlfdvwkt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rjrhhssb.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3gnuudxfk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3matymrqt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3nmxslxgl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3bukrivnz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3eomlfvau.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hyfxvqxc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3rgysxian.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrdkwrcv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3nfmxslxk.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3kcolmwpx.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fmgumkkv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3qdnydwyo.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sljvtokv.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3istostbn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3rewddtml.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3ggtuwnbe.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3oazwsfrh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3eburnmho.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3jpapxotp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3cjjyrbyd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3kpesazjl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3epgjxgnn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tlywnvqm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3aseuvkjy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zlcwzblk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3kgwgdspa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3deivtbfo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3jnehvfuu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fmocmhxc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3plriguid.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vbtzhoxp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fclzbwyw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3clpihezo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3rrzvnwzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3omefgfld.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3apttaxoi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3tzwylnjc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpvjjsw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3msuvpvlw.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jdnfvxzj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rigcgufk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xkxnymqv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3qiojrkrm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3uuemrogj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3wwrqqjoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ufpwlcpe.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3jzuzevpx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhzrfsdq.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3uuhhsuil.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3ifsqvhhx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3jquvwqfd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3cvddxhyt.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wbbajwtp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3oijgylkr.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3jnvqothj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3oxbjsclz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3drzvexco.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cyngjcaz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3nfipehlr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3coirhtmk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rngwmhra.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3xwvsmkyx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jdfswzsm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ytdeyqbi.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3ecvweghq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ttynycko.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3druojeib.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vlvaybtk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3swvmduij.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pikftydn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3gytuytld.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ohcjncwk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3aepszhpe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3eyfmtwsa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rvkxbsut.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wpoktnxn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ygqcvpmf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pakdorue.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3sdusfaqa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3qwytvkkf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rrxqadfj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rrkujojs.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3faknklab.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3rsrkgoco.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3salrssem.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3rbqqjkhp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ffjoafpm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3mxhxblnx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zvjhjdqw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3oduxtpyj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3zwlhozcd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3bmrjwciw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndswuczi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mkscdkki.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3wclzkpjd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3obafeoba.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qhxfsvcc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3puhcobfj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3kdfkkoob.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ezyojenu.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3thheskyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ayxmrrcg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uacekxgi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zwwdymta.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3apfuhnyb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nebsugle.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3evnyqsmg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3sikdyfyl.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3htkdrjhg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jaaajrbk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3uujrrigy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3txrrvmjv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rqrcozms.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3lvvrvfky.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lkktuehe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qqkruaea.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3kgcoqjyq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3djksdund.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3pqeuayya.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lolluekq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yavfvikh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3tlxqionl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wdtnkcly.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3tfoshwzg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ajgaxcyp.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uzxslumb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqyrigg.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cicjipoa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yzjossoi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rkbpozht.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ypwvofgx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3beucchtk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ayolpdke.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xhkbqpoc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3wwypqsrw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3pcalvurt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gmegzwus.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3szotzyeh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3idwsegfe.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3htwokfyp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3welqiklv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3wbtwhpbp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qmazumcd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3awofuurp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ywlpruwn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3spgzxxpa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3chgxiwdm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kxkrzuey.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3kozoipcm.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xweguicz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fvttjnvu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ffvifexq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ruiushvh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3usdxrdvv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vggevifi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3olzglggb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wxkpublv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3owfjjswl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ecdngqts.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ncblcovi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lhpjadsz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3otcqkyay.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkdqhbl.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lzclvxrm.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tnlnfcuv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vyyacscs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtdjmlwh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3tmrvelgr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3plgpdkdd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dwnnngtx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3cxbhvffz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ttqqmefh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wmdmyymd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ckfkjhql.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3llsqfkhn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hgurfltu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3oaeoopnc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3bfbyzzeo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gxidikck.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ndpismzs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hikqecix.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3gcjdlqhh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nninxtfb.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3twpzcadr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3gwyngqhl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3elqwchzc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cygsehxb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3npbbuhmj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ozdziqvp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tptowaov.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qwxpinvy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mxfwwxji.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3unhssung.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hketmbqy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ndhyxisy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgyoytxh.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ovkkghlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iajwvvcr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gssktaxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ihvfipvz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dkbkhjvh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3avtpqlxy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dxkzjtul.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgiqjvz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3duxpyzvd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xjxlmqln.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tgenmueb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ntsyrjac.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3klttlnaj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3knhekfqw.html


<!-- 参考信息 -->