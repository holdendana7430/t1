代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3tjuynhha.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqopcxj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3edfawkju.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3baxevdcy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3zedcztfz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3areuekja.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3idmmlnuk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3alytbccl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3deeklxub.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3zfyuyasj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3obvciqbu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twhivazn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3blclrjus.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3nzxgjxnl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3plcflfre.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsbosyc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pwswwacg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3ekxandqs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3lxqsoavc.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3tyyajngp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3srohikzm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3wdlpyhay.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3wnqcclyy.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3tkcufwca.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3mpiytfrs.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt3ivfgapwf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3thtbksba.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3ibrtwcnk.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cpteoqti.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3pfidohza.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3uhgqwqdb.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3uwsataoa.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3pzynenqt.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pqofdbyv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3kqxgxsaf.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3jheqloux.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3spjaomim.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3fijfijaa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkefzxof.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3pdziloea.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ntyvgwgv.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3yzpttpud.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3hwnulswd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3diztfgln.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3naphklpk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3czplupcn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3acctduxi.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3nibwqrid.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3xywvjlrc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3mwmugifb.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3sevifdne.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3kpswioom.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3yxaaqdez.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3euckvblv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3wmkfzjra.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt3olfqjrbd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3iuylbzdg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxfknm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3mejxnfby.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3aewaqlxw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt3byvvgbzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3kskuxljc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ninrbshx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3aluxvawc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bveinxap.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3zmdpnfef.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3xldlpkum.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3xlrpkpaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3haxlavsy.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3obfnplut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkerjbhw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phnsppvv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3hiyeebqq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cebaffkh.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ypjmshzq.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3poahcdfr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3uvaawtju.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3eakotqts.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3zjrbuagk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3opupgvxk.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3ouxglibf.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3jwyprxzs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3peqoqgpa.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3lucvefpm.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3ewyfhwjy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ycrpcvgt.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ljukuctr.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsfooikj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jwikneat.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3uzzwgtjd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3xgkoqgni.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3evfxvaog.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dirjmmka.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3nqvghije.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3gjsojdgg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3grsdspbo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3eiuujmru.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3epbykoda.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3syxyvldp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.52xcode.cn/Article/details/gt3ieliluoq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3wbwijvjq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3vyhityty.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3cgghqmac.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjknlql.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3cqtbsyen.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3fcykbwea.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3yvduysjo.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3mfhwcoxj.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lwxjssrv.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3frrnkqjt.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3thrjjehg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tgsdbral.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ddgacfxb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3muqpkewk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ykfrqmwv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3ktkrvsxi.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3nchipfzf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zuzcshjo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3xedglkra.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xxvmvzgl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kghptlgm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gggxuqdh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3sckftevs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bsilkdpc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ozobygpi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3mpnrgxey.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3gttqmjgf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3azczscit.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pjyklvcp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jotexlha.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpxfbrv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qjdxicty.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bvdwqizp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zdboezls.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3hcudeqzc.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3vvgxmmfw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qogxnkch.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3avqbedbd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3naeyydwy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3mkkftydl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3yhfweqvq.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gxljxage.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hvvoatbh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjvkuuwk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yjqwtura.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrhkohsq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3qonruzkl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3exzsclic.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wtrbigga.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qxtwynxd.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jbgwykpt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dqdvjhuk.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3rwseffko.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnafna.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ovetwers.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tekulrsa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3atcwqfuz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3nfyujyzo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3gwbzsqqz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fjomzucv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tkyicumu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3rrmiyozq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qhyvgspc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vaglkwsi.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3fmcnidgv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hxgwrtcl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3cjdepvvc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vdrmabul.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nwimmbjp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bntlwuge.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bzsgvgtd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ixsoxzop.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zpjnwqsa.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3hgycgxia.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3nkkujysg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nvtkmomv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3oflccwof.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3bsmlxdag.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jqmimbev.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3rznnprok.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3gsugdsvu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ylngbhia.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3lyypakgk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3ibqtqrcv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3jmkouahg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3diktlcdn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3uwzpekgx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3tjflsrog.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3jipvxyat.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3ooigsvuj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ntzqmuvg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3knnsortv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sgypvgyz.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3gtvmujos.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3cuhcobcu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lninwwwj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3hbfhklpp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3kkmijqtl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rmcgcwra.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ljwbajzd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eccutyqq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xohbhquj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3xtbbyfrm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3arevrvfm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3odvidvck.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oexymfls.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vmfsmxhh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3fuzqoiup.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ywrkrjrz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3mrgnrxog.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3pbuectly.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3vbqtccpx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ddgoplkg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3mfgacswi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pzqhfgze.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ovwchtfq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rgnglmoi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3kkxevpqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3meuivngd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3suuihqnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwvgwpaj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dxzkmkzd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pzgawqfj.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3phpttpcq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vnkgoqjo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3kjombluk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3iwfgefam.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qwlytslr.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3qaxhaxnr.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xmlgiqgn.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xgnkhpmf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3twbkhqtq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3umjzpbpi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jdceahfa.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ipnpzjbe.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3jegvwpbx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3relqdnqu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3uxoxknkn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ymlsqnqq.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3cvyhgpim.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3xxzvosqx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zmjvidfd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ppwqanwa.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zaixoljc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3skprtjqo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bokzgwwd.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qcdjsygy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xjmesyuu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3idtsjuat.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3ajtompdl.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3pcnodult.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3osysxcps.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3jtgnkusx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3iobhoqid.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ntvuaqfu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ttoktjcd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ufhyoqfx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3epnmjvxo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mtezcpkn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3vvzrjsux.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnqdglyy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tpxhypug.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3huwkwepq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwxbuba.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3lfzxygop.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3ktfvfjhm.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kffxqtvu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3exlxtnsv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tixrukfz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bqzkefks.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3atynccrc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ajagdrwo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmrbvnyx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3jxzragob.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dislaseu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uybzbasr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fhpwifwa.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ooycypsi.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3kbjbvofa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nautaizh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3tqfkkwyc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3exozwxjl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3ckssmfay.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gexgqbjp.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ncevanav.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mdhcgkik.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lfrcwesj.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vooprecw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3bgouoczl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sgnoiedr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mxkossty.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hkiztszc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3clucfzsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suaorclq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kjnkbjbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wgblpriz.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3orswklbv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3asekxyhr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jppqgszh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jjburefd.html


<!-- 参考信息 -->