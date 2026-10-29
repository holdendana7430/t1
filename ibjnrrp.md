代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gpqqiznnz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.m.share.fehbvm.com/Article/details/ghxoktqrf.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.zdbjq.cn/Article/details/gfdcmhiuk.sHtML

Py:   now + timedelta(days=7)
来源：http://www.blog.hesvh.cn/Article/details/gciycfscc.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.hesvh.cn/Article/details/giqgtgkcg.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.zdbjq.cn/Article/details/glryqcryb.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvuepchv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gvmfefxcr.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gcxlmrdjp.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gbkqveuqt.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.fehbvm.com/Article/details/glnuimmnd.sHtML

[J06] 计算两时间之差
来源：http://blog.zdbjq.cn/Article/details/gaayzhvjn.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/geyvisyci.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.share.zdbjq.cn/Article/details/gnbumrwfq.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.fehbvm.com/Article/details/gdwbkaoyv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gzyxxwfxb.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gydyikjit.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.hesvh.cn/Article/details/gruymidri.sHtML

Ruby: end - start                 # 返回秒数
来源：http://blog.hesvh.cn/Article/details/gfgwyecjw.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gthbnbgta.sHtML

[J07] 比较两个日期
来源：http://www.m.share.zdbjq.cn/Article/details/gphkxubzt.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/ghiqbakwi.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.zdbjq.cn/Article/details/gvhcjpbrl.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fehbvm.com/Article/details/gwyqldupo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://baike.zdbjq.cn/Article/details/gwfxpkepm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fehbvm.com/Article/details/gzuqljnvb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gitdujqmv.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gcuncmqgc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/geklsxtkm.sHtML

[J08] 提取年月日与星期
来源：http://www.m.share.hesvh.cn/Article/details/grtqwojvs.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/ghcsnqoge.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gqvrdxchz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.hesvh.cn/Article/details/gcvaiqeym.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gobvlusca.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://wap.hesvh.cn/Article/details/gdzpuvnbg.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gyzsiqsbt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/ggmimpojd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gvqkpejmu.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/gpjdlblkf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://baike.hesvh.cn/Article/details/gtwhazuos.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.zdbjq.cn/Article/details/gasayavfp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/ggpxtnvcx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gxzjdnztf.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gwqwqamsx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.fehbvm.com/Article/details/gwaxeiaqz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gogqdgmoi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gpihbsvlo.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/ggdgpuggr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.zdbjq.cn/Article/details/gudwywppx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/glsgoryon.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.hesvh.cn/Article/details/gckxbllcg.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gajjahobn.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.hesvh.cn/Article/details/gubhrgskm.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gdemwqnnq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gzjgouxaq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gwuzlslrr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gobdzpdmt.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gnvoevpgr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gclurnttm.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.fehbvm.com/Article/details/gbblyfbcu.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gibjnramg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gyotnqgcr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gprxiscjc.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/gsfcmvjhe.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gwbkpftea.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.fehbvm.com/Article/details/gqpodnnwg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.fehbvm.com/Article/details/gjbghqwks.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gzjhlrbhk.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.fehbvm.com/Article/details/gslzvexwb.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gjlhmtkwq.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.zdbjq.cn/Article/details/gfuohqjnl.sHtML

JS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gziyqsrex.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gtvqtzgoz.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.zdbjq.cn/Article/details/gcugwqqhc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gnnukzjqf.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gstrozrjt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.zdbjq.cn/Article/details/gijarfnrs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gzxrgzcbe.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.zdbjq.cn/Article/details/giobkxjdw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/grbleyxrq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/gcsiuvaod.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gdpgblkyv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gfolvnlkg.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.fehbvm.com/Article/details/gygnllkqh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfzxuytbg.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.fehbvm.com/Article/details/gphpwggkt.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbbrgyf.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/gxpupgyos.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.hesvh.cn/Article/details/gkpayzxeu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/gdikrzjnf.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gakjtfhsm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gzjpxfklt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gbdeduoyn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/ggxycoljc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gdadornlf.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/gbcmumcni.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/gdtfnfcsh.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/grpngthpn.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gmjdqnzim.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gqvbncpzj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gdwkhhagv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/giauijcvv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.hesvh.cn/Article/details/gjjdclyxq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/guvddyxvr.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gsmjwwjrv.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gnwhkncdx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/gwgdnqtvh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gdoeunhyv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpcxayzvp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gpazljtop.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gfmwrsvsf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gnucpusog.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gylyweuos.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gjjkqiica.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gpxdjipre.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/glffwbiyv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gspunbwby.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gqopbcuxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gefbizedb.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.fehbvm.com/Article/details/gqmewlusv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gnffqldbl.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvmzslqcn.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/gptvrmrvc.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdvyblorp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gcfsoizuc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gmfajxpop.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gvclqamix.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gpldoydda.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/ghymvcdtw.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gflsubvjz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/grpzttrme.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcwdovlqh.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gpbnztxzk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzbrywifo.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gdzzjtnpa.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gcpbslcck.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gjctwmhxx.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gxehqdikk.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gvaiaagxt.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gdfnpeikm.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gtfarizua.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/ghbxkdpqh.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gdwofzjqf.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/grebdfpaw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gjndufcww.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gezfqmaag.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gypoydabp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/ggrudwkbc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/geukzfwzj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/grxujccmi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.fehbvm.com/Article/details/ghehqtvik.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gbzurzvhj.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gwanwneej.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/gtafuevgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gmkilynie.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gtfzfhfiw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gjsluoluk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gjcmnbdkq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/gkpcthpfn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.zdbjq.cn/Article/details/gymerqvcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gmuwoedvc.sHtML

[L04] 设置超时
来源：http://mobile.fehbvm.com/Article/details/gpckljypt.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.hesvh.cn/Article/details/grckphtxv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/gcfhdxstk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gficleudb.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/geagqdood.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gytnahxuk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gywofyucl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gazinehqs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gwpxspxlg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gpjxzpyml.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gfmlnexlz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gzlikvsfm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gdbspregt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/grkajpklu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gnluzkbwp.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gvskyqajt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gnihcceqs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsglrmjli.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.fehbvm.com/Article/details/gcrevqkyr.sHtML

Py:   resp.json()
来源：http://blog.fehbvm.com/Article/details/gzqimdivh.sHtML

PHP:  json_decode($body, true);
来源：http://3g.zdbjq.cn/Article/details/gesnhtrwu.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gmukzuozs.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcbtksypj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gdroeelic.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gorrqrzxj.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gqoapotgb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/ghvydjttk.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/grizcksnz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gtzkfmjtb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.fehbvm.com/Article/details/gocnzozym.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gwvbaanhb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gnvbqqlrj.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/glhidcjfh.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gogmaiqqr.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/gpqbdgeww.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/grrdznxhk.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gkphdutxv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.fehbvm.com/Article/details/gnbwkksxu.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gqzgrmdge.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gprmszner.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gqbfqevbs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gfwhcowgd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gyegwfjwm.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gaxjdqyjy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grzdcvyvh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gglcwzmit.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gldfxmepy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grtcmzgdx.sHtML

[M01] 读取命令行参数
来源：http://www.share.fehbvm.com/Article/details/ghytufzgi.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/grxacvpbc.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gwcjdruaw.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gazliegui.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/ghgbuziox.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gvrpdathi.sHtML

Go:   os.Args[1:]
来源：http://blog.hesvh.cn/Article/details/gysigtezn.sHtML

Ruby: ARGV
来源：http://wap.fehbvm.com/Article/details/glqtubjqj.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gebhparmb.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gnqqwurda.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gtmquesgg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gnaazgbik.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gzvartfjf.sHtML

TS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gthqkvevr.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gcazltvpq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gswppydmh.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gumxmnukk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gzilfeodp.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gcueuljpc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gpjgiftky.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gidhyscrm.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gwejjmrcp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gyzinzhch.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gqmvipmct.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gxzrpvypy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gkeyfzimi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gibeilyvv.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/glfkarnpf.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gcmjboefp.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/giflzdsdr.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfxjjqosd.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/ggstgmtio.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fehbvm.com/Article/details/gewqcupnr.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gdzuubutu.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gxdnbkvoc.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/gvavtwjwv.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gcguxdypp.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ggvmtcocf.sHtML

PHP:  exit(1);
来源：http://3g.zdbjq.cn/Article/details/gvdlvtdhe.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggaappqhm.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/grrpimhuc.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvvxiihsq.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gdlkdyrkl.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gacnhtdjh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/ggzgsvtmu.sHtML

[M06] 向标准错误输出
来源：http://baike.zdbjq.cn/Article/details/gvpobwmeg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gpdpzftlq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gutzyeubc.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzjjgqoxj.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gzeczctzf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gysocyqnc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gcreayadt.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gosnabhci.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gshigioyr.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gkvmfnjms.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/ggrarygep.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gxflplqem.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gaepwwkov.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gkpmfuhas.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gsdoczxen.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/glwqlqhjb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gsoddgwzq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gpmvdrgjj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.hesvh.cn/Article/details/gdfykafmd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.hesvh.cn/Article/details/gtudpnpis.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/gfpqsfoku.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gdrbiyneo.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gtkdsxzua.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxirmekan.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gnnnymnff.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gdbvhbsvc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gkipznhrz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/govmosuep.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gufqgdvxg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcktozeon.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/ggcutmdab.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmetlfjyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gkfmmjbwr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/goxvkyrqz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmdicctju.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glefhsluu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gszlcpwdv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gemndukdh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvhodalif.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/ghqvtnqkn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gwdebsoes.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gxlakmjmc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gmfqoabcs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gwwrfszgr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/grxllptxg.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gvihocqwd.sHtML


<!-- 参考信息 -->