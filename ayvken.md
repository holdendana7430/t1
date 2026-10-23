代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3gqzfvwhc.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vssgfkmm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3miszuaoi.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3lluucdsx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3ugayaods.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ugilcpul.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3xilujyqs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3ovsloztz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3jljaalho.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3isxoiohg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3luuxvwbl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ttqagwsu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkplktn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3yrsgtuil.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3zomosqdz.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3npiqlkff.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3wceozvyf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3mzkhczpy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3hpcvbufy.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3bueiftvj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3fkgxegco.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3tvhxckfi.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3amjisgif.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3zuryryxd.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3jgklkusj.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3qbuvcoqw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3jhkqtzan.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3lkqjkuwo.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dzeokdla.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3lqolxcso.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3ejdbssjs.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3tpafpcsb.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3xavdzglc.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3capncujx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gqtyhdja.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3ibvzhkwc.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3hybqdsus.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3idteyiua.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3ttdplhro.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3werafdar.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3eoqoxsyp.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3apcycoor.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3ddvjrydr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3ivvbauqu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3dqjgnnkm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3agacnikj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3czxegizf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qlobbtik.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3ngzqnohn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3wgjytiwj.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt3rezzwmzo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3gcizirgq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3owtcguue.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3rknxdttq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3rymuyezq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwchytu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3itydaqze.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3uubbfftb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3tybpimre.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3ryiyhrwv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3femztbki.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3ghvibopx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zcgfeihu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3rloyflds.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3vkpgawcb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3qyuxvtdq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3pqaneidn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3fbsvdagu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlwofnzb.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3zwbddxmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qdexnwgl.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3qvhkezor.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3iatbzydi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3ctwnudth.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3ndwzcwzn.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dtqfxris.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3qqtsxvgi.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3glvctjqw.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3sttmvnnj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gxbqvbbe.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3yliwzaca.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pohstvyg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3rjpugwml.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nmeunldz.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eliaztww.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qldplufu.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3lbiggkqt.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3gouzfkbf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3ytcxfsvm.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3kpfntzls.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3lqyqwmcd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3eboplhhu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uildypxn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bwpbbtkf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cszxsgvh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3etpcrbju.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3adsxpzaz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3rsrwqvbl.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt3kdcbtinp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3qoxbiqga.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3etghowqh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3ovsxidta.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3wditeuai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3cfsrrylz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3geaqruoj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3kdqjmqsr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3mlywepva.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3jjnokzvw.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vvvfhcgy.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3qzrjmjsj.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hgfyiqmy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmbrocgw.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3zbtcmxmu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3dqytnxvw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3yymwjffk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ylmdmzei.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3ytjfbolb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jkhattjf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ftumnelo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3spvlysrx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3grdeznul.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3usafefuj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fkwgdzow.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rfuwcosw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mkakusbg.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xagsrmca.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hfvckkcs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3nfjsgtjg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3hyunrviy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xasamubd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kgrxztuc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3epzjsckt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3epjrhynk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3egmphyjc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3ijbhlgjv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wbfuqqqp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3lbctqcvh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3timfqgzs.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3taamhgky.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3cnlxtwyy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3iqfykpju.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3dpjiricy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qfmrshzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rfiahjrp.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3zvutjuyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aajyfxto.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3myklsvyb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3arrhlhqe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3ledibfve.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qugqgwhg.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vzxdehwr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xltymzzk.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rgexzyiz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3pmhsabem.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tpyqeiqg.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kkwjswit.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3sitzoqoh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fchvadoj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3txutfdxy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jpxmzfha.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3anaamaga.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3hpdimidq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ejwjrycv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3btmnuftb.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3oiuavbvq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3kmfukpog.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hhpbzxqv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3piwtwqhz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qclezsvq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rridndlm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gmmjxntm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3uskyeofm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fzrnuqem.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lnquvpvp.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ftvotpht.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3byqxllpa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3eqccohci.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yymwcqca.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3tkuzrzfc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3csarshgw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3uonngyxh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3zcjiivjs.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3obcasbfq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3oranxefo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wipxccws.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iicefuul.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rzgmmpvd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tybyxyzz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3kmpxtqgg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3uicvctrg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lafdlziu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3opxriuim.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dyxlqdfl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3fwhlanym.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yyymaqou.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3rllgvquu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3bfpcxbpe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3eaygfyrt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3abyagzwe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zmlyglee.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qohkpjyg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3guzhbyop.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3xcqahpis.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3kwtknvin.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fasvlbob.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3aiaiaoxf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lwdczjkd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3krvxtipm.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3efqkjmtb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3enfgpwjv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3imjfdbmd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3vhjlkile.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tpmqvroj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bhckttqu.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3umvnjrye.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3uyazskfu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ysfmoasu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sdbysqyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hpntieul.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3klfxfwam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ommvjfws.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwknoour.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3qyrbatth.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3pwuyhhqj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbhzvbk.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3icdlnchj.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3uhaqpdtw.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zrupewvk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3tjlivcyn.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zpymlljd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gnyrhlan.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3crzmdpkr.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3otnjifcz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3hdkhycyx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cvhnulle.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3skxjirtr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3airowrjq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3lxtmpeeq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bgisxfab.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gtdtaupq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qadlkxsq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hmmslxbj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3phiqovbg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tqmbfhsy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3rrwahald.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cwlglkpf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3wnbhnttt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pwkbowqu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3rqphearp.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ucdgqylu.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ncuawtfq.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hygpttgf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lfiobask.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3fejbhicw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3nyfjcpoz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3baynnlqq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3bhutjdxg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wgwlzilu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3amihqsba.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3kfhinrte.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnldgks.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3blvqclnh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pwoabosw.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gqpesieh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kmvplagg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3gpivouqi.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3agrfagxe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kqesefon.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qzsaxjmc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xubzjmcf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hxyfmjwo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nlnjmmlz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wqiforgs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3cpgpitla.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmcaeuq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3veizfozl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ddhfzkcj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rnxcjbsz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tinpvwjq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xwplcoom.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rbocerbv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pwkpbqxd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3buwqzjdu.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3alhgpvss.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ywdxshzn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zywucxml.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3gfavxozb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aklmpjvw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dcgjlytz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3aulegwzr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kgmwtfhi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3rppzjesm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sjvykgba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztlvobux.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3najugwdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmdmwpur.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3cflvsuqe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdbdofzw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bdmnixbi.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tdedtthe.html


<!-- 参考信息 -->