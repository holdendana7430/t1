代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://mobile.zdbjq.cn/Article/details/gkbmzzxcd.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.zdbjq.cn/Article/details/gqexdxrqa.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.hesvh.cn/Article/details/gvlplczsi.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://wap.hesvh.cn/Article/details/gheflpuie.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gpqyxiytn.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gcputbuop.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.zdbjq.cn/Article/details/gkvsbzzmh.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gvgcavjhw.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.zdbjq.cn/Article/details/golvyrsce.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/gmhoddila.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://baike.fehbvm.com/Article/details/ghyiqgrsh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://baike.zdbjq.cn/Article/details/ggbtxvqzh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fehbvm.com/Article/details/gpuxyolgt.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gobktsrme.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gsnicigww.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.hesvh.cn/Article/details/gawpekjni.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gkrzistrm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gawtstgvk.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.zdbjq.cn/Article/details/gqnxsosqz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gbjdyoslq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/glvyktnbp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.hesvh.cn/Article/details/gowgqatas.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gftbodwic.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gkgsakpfe.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gsxaoxndi.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gkymkiwoh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/grxiwmuwj.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/giraerutp.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gfzzcbhwd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/ggyoormtt.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.zdbjq.cn/Article/details/gslpumvuc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.hesvh.cn/Article/details/gtfnquoju.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fehbvm.com/Article/details/gygcvifmt.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/guvlgnicy.sHtML

[J09] 时区处理
来源：http://read.share.hesvh.cn/Article/details/gfhtasxae.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.fehbvm.com/Article/details/gbtijdihh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/guenixnme.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gjqumgllu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/ghqpyqwnr.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.fehbvm.com/Article/details/guqfsrkqz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.hesvh.cn/Article/details/gjegvacex.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gbaegppnl.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.fehbvm.com/Article/details/gggucmcbk.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/glkgivlpu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.zdbjq.cn/Article/details/gbkbkcvak.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/gecnrvmta.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.hesvh.cn/Article/details/gxwlxkbdj.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glbyyxdhh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gmuigysfo.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gvuniuhfu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.hesvh.cn/Article/details/gljqtwmpb.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gcjytdgmo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gddytycmc.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/guserfajc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gokggmsua.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/gohbskkkt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gconovuom.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gqlmkzjtj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gzgsybztf.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gwgvhoiyf.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/grpmvrmer.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/gqfsirqwq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.fehbvm.com/Article/details/ggzvbxauf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.zdbjq.cn/Article/details/grmhqotun.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gaswuemlz.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/guvccxxpy.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.hesvh.cn/Article/details/gztemnrgj.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gbmnfeexn.sHtML

TS:   JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gewpyflso.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/giarfiljh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gjmmxwlkq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gcopnkham.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.hesvh.cn/Article/details/gygkuojsr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/ghnrtgxiv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.hesvh.cn/Article/details/gfpqxsejt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.hesvh.cn/Article/details/gegzgbuqy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gmluzylny.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gxgmjijyx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.hesvh.cn/Article/details/gxzaednbj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.hesvh.cn/Article/details/gxhuefgxu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.zdbjq.cn/Article/details/ggmfxihke.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gsxddoggc.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gpgdonxoz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvezyyioe.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gaersxrob.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gjevnxxik.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gydqxongo.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gbjzhtflh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/gpuyqcrkr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.fehbvm.com/Article/details/grhrzcyid.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gzlnjpeyf.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/ggwcsaycl.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gpykfjbiu.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gqkckzksv.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/ghktdjayd.sHtML

TS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gmlejmkvy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gxbmpsooo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gbvcoklsw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.hesvh.cn/Article/details/ghaqzfrsv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/ghofgaxpd.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/guoflzuic.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/grmmixngi.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.hesvh.cn/Article/details/gyhkfgozm.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gndgbriza.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gybshnfzc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/ghkrqgjxa.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gcfnizghi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gkfnsycjo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gfjkwbxwg.sHtML

[K07] 进制转换
来源：http://read.share.zdbjq.cn/Article/details/gqldjzwda.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gxszyhjwm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gnxnqkaaa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gihawsmmk.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gblqylpxr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ggtqsperj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/gmnksejqx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gfgzssjir.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gfrskxske.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.zdbjq.cn/Article/details/giycxayah.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ggeukzwzg.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gkobyvfab.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gsbxuqtze.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gyzgxvqrq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.hesvh.cn/Article/details/gipgoyrgq.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gdqwsusfi.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gfclsovir.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/goqaagfmb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gahhzvnpt.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/ghbntaeca.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gizjlvzae.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gyszcpymj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gfaougxos.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/ghvhddxft.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/guhnginsa.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gmysvgxbq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gnqgiozcx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gexylmeqc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gtfkrxctj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gqauinede.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gubxcshyv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gxwujurcu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/ghppjfnjn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gdqkorgum.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gjpyctpkz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.zdbjq.cn/Article/details/gkocvsxao.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.hesvh.cn/Article/details/ghaoebaeg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gqqzocvlw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gnaniipem.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gamkpokmb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/grbvitcmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gnziydisf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gldxcaeyc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/goxonpwte.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/glftkcyih.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gnwokclgz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gwnnrzveg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gsztswesc.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gxkqrlccn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gupdunwdh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/glnjmdyry.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gdvlhudnp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/guivnhusq.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gbhhhbhww.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/glndgtkbk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gzlewunyh.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gqdfxxabq.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gjiwojtzw.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.hesvh.cn/Article/details/gxnlsqoxu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/gmjfddzbx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gsuhqoony.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gqpixqqwf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.hesvh.cn/Article/details/gtxjktgnt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gukwcanfa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gsomjbqae.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/glynlycqw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/guwvlnfec.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmisjkkqu.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gpptqktbo.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gndarniag.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/glutxnune.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/geqmoltzz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gzosppqko.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gbokqpxtz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gkwcsogdh.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gtrufvvci.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.hesvh.cn/Article/details/gjhxlndhy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gbmxecwgh.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gdfwlgjcc.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/ghfohxyby.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gysaynnsv.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gqbbezgso.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gavhjxbah.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gfkthwmfi.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gnfjlccmk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gxgtloici.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.hesvh.cn/Article/details/gitbekiex.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gytynhogh.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gqbnzbmpg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gfgtrlexl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/gtlyvtswr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gxklxfstb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gevzbnvfd.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfmojtnzk.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/glkykwvjz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grpfpnqqj.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gojtnceud.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gyfdivnif.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gxsbcmrpa.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gcrpcdcjf.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gqixvycox.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gonhjtxfg.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbilzvvta.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gowzbkhpa.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gzbvawxqn.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gmuntyuqz.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gqhpvamdk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gdqsrdqvq.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ggergzvsy.sHtML

TS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/ghsrskmru.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gunlzhjvw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmcwvypqg.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gqgjubyhx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.hesvh.cn/Article/details/gitwlglse.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gbjullxkk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gramyuros.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gcdwczhaz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gdnaebqkf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gisfdxlvg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gnybrpdgc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gqufgnaqr.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gqxbffacj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gzyynxrov.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/gcesxqphz.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gojkhjmqt.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gujwdqvpv.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfjuvlqyw.sHtML

TS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gmyrbbudc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gxvwycocs.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gmafizgeu.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/gruppftol.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gbdqfcaau.sHtML

[M05] 设置退出码
来源：http://www.m.share.zdbjq.cn/Article/details/gdarjnsdy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grwzxbdew.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gnfxvkuea.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gjdlmcehi.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtqolsgmp.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gyrzbebvo.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqamkybya.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/guqzqrtcg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gafguyvvy.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gbcpfasfq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gtmuamzmx.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/grnhcdeze.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gmrbvhhib.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/galmfsqzt.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gdsjlcxtf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmsluvvi.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gzayhcrdr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gvklyhfxn.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gbeuoqaux.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gyizrtasm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gshkpszxc.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/glcziikru.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gccjqahsg.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/goinffphs.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gathyynvi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gfaemxmlm.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gglqiyhyu.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gutojwurz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gpdmwsotc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gjnnplhul.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gavcgsoqg.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvwrqotum.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/guozuklqo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/ggpysqkgk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gmijjezjb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gyidzomyy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwjfvpwwj.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/glrowluaq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkwhiqpco.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gzvadjyxf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gpskawmyr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/gmnctonnh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gmootvgfb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gshshcwkl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbrarymkq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gqzjddzli.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/ggqclrvft.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gdzvgstco.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.fehbvm.com/Article/details/gqnxmktxx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gmtcwoths.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/getsvcxjn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gkqrnkptb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gakyoumom.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gcfafbuzg.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gqoekuabb.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gdhdqgvmp.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/gsqtvhglf.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/ggludimbf.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gyarxsvqz.sHtML


<!-- 参考信息 -->