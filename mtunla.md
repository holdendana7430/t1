代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.52xcode.cn/Article/details/gt3xnjldybk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3rtkybead.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt3mwnvuurk.html

TS:   d.toISOString()
来源：http://www.52xcode.cn/Article/details/gt3dzkynmnv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.52xcode.cn/Article/details/gt3moniuzer.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.52xcode.cn/Article/details/gt3bzzzpecv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt3hpjcxlgk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.ydjk.org.cn/Article/details/gt3qylnawxp.html

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xrdgrulz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt3ptaqihji.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3haropfld.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3afgvtlyc.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3agnjqifp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3jsigvlnk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vucfwgwy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3xnsnzixn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3ellzlasu.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3ykrxzsef.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tukxdbmk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt3dmrggkti.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3rmnclyij.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.52xcode.cn/Article/details/gt3pugvsose.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3reutqcqf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aicofhuc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3yaukhnqq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnkjrv.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3epfunmto.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3mydurbxk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3thnqnwtw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3gxydldyv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3wpzsmxeq.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3bxjwtepu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3gpaacqrw.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3erxkrszf.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3flbdmszg.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3oupzcsnc.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3cjdiaakn.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3nqpuxgns.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3bfwshavz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3rjjuzxlr.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.ydjk.org.cn/Article/details/gt3dvhdppuf.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt3lfeyelgt.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt3jspkmhwq.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3qlvgbxrb.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt3riukjgti.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3rgbvqkjm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ftyikpqd.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3ebqltsva.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3djnhqisc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3dmlirkky.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3jswmnelq.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3jbildhjs.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3ixuhmskc.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3clslqlht.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3vothrocb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3rrjgadnn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3imjsfzov.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ecikfyxm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3esmtydbt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3skhohymm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3peyibnuh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt3pevrkumo.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3qndrwqok.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3jvqafsqf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3wxqbzeeg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3wwoifjfo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3japihafs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3aapulpah.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3wosdlqhu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3opedswno.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3gejzgggs.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3jbqqpokl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3weyxvdip.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3grexkgxc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hankijyg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3umbqloml.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgyefyrc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3gjlqlgps.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt3evujauet.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3zcbzctbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dspcpzoo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3cmnyjlmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plhnpyev.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3cpbijfxs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3kgpskxxh.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3whfkjfbu.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3cwxgfueu.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dpshpwrm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3wxvsybdu.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3qnueychz.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt3iqhyvfim.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3evlxditd.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3agpjydca.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3axnklmkj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3zhbzucbx.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3hpqxssdh.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkalahbp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3inwakwlj.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3pdkcfjqf.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xisipktx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhtqbuk.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3ymxyhsff.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3zbfxwqyp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ncytumom.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgrbgafg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3xjksmmjn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt3amkoywfn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3gfqhwmop.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt3txzxreva.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3scxquohn.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3hezidtcf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfmksbck.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3gbwgyapw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fyuumcif.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3tmlgupgb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3uvslufrr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3jaubeaje.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3dqcutvmv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3arsjyncw.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3btyicgyf.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3hufocjhv.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3bgzsqxyh.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3qtuuvzip.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qegwlhgb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3jdixvpyk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3suhyqbyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jpohwtbj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3hwsltsqz.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bvgcudmb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3rzwrqtkk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3atrgetqt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ojcvagep.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kjdarewm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ihiomatg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3vzwawaod.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3imlphpqv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ocypduwb.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3ssxtxujj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3skawwmcn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3xxodgmsa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nzpyfvcv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pveuymuv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3owwaqgpk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3efyakjud.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mopdynff.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3papuobxa.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ofycrxsn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3sjwotxhw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3sxnrscdt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3trscbzax.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3xtxgaqlp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aifcorut.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3dqelofhe.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3blicrwbu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3uiokgxzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttbtziyr.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3bdwuqzdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mzaiyori.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3npqgcqnc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3uygsbwml.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ruwbmdvo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ryxagkpu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mpwtfbxf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3dcryboas.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3vgpsecos.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3moluyjeh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3imyypxzj.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3uavztkpc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3tqntmfpw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3fbwjzzgw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ehsjmrkk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ytdlmooq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gegigmtk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3tmacfpyn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3esygwtmi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdfigsyo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3hinvqisc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3wcdqqfch.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3fepydsbv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jrkvixiu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3skxvrxdm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3rdvlxqmz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ofnacexn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jupohyei.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3royhcbye.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3leeolzxu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3waauwxod.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mwqysntu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pstmvbmn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zebzwbye.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3nuyqijzr.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3uigaabea.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hiiqdzhp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3ewfefbkt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3wrjolzvs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tbwcaidf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3kupktbng.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hlyivosz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3gginlsgu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ujzbztcf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ieucucri.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3qmmuidri.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3radosjat.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3evcykpuy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zqmfxyih.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3avhhmtko.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3komguxxa.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3mwwanaqx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3alqrcdmx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hykvcgsl.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kvrzagfq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lsvnhhfj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vacvmbus.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ygbnkewr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ndcwxrow.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zetmlpke.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3mbxhzban.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yjgfcltp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rybzcujc.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3xlsoothe.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3idzyysrb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3qnpcrirv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3aneoittz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zgcdsngl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xdqgsfem.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3gnoebatt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bvlvpxjq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3hdgxocav.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3aukmyvyx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3xyoyfsnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hoectzet.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3khcwayrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpsvpjik.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nlvtpffc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fdjedlqo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3hhogcola.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fnyajjjr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmnacsvu.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3advhixpa.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nqzuiaee.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jsjwoiaf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zsnlanqt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ztfysflm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3sliotxbj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cqpfvyoh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3enlcxwld.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yjmrgpsw.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3scpujeqz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qtfeduwv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kkielgih.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vrfvgkja.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kfxnqara.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ybhjpwbb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zircanfr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hrxowmqf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mhcijrrr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3mcorxqxa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3glacddlx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rapdgerp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fordyhgv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3mmohupoj.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3alaiyksj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3twryhqfk.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cwwpptlx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3timbkyii.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hjpiqura.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3gblmtuoe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3hnuadyps.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3fnweeqzr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jjjqfude.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqferhsj.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3uueinquh.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cmxozzzg.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhvqblx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bwxjipav.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmjmffrg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dslqnskh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tgcraukd.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3fimenxjc.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3agpwxhgt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ylsqvcld.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vucvddcs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3pkkxpljs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3juoudcnw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ujjpxiau.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3tkrytmay.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gggcroxc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3tugtugwg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3sfzuxpyt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3zbhcytok.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lvllyedo.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cahbyiez.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zaaoezzb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3cginvaku.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ssucwmdk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3dunukkdq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fpkrimrw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3nhwsjoal.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3jewthfjd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3bgtqeigv.html


<!-- 参考信息 -->