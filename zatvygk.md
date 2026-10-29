代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.zdbjq.cn/Article/details/ggxuwadls.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mobile.hesvh.cn/Article/details/gxrfduuze.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.blog.zdbjq.cn/Article/details/gkaxjvdck.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/golezciuv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://read.share.fehbvm.com/Article/details/gfmdrjzqz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/glmdygqnx.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fehbvm.com/Article/details/gykhrewft.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.zdbjq.cn/Article/details/gtlwyslbo.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://baike.hesvh.cn/Article/details/gcplamoct.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/griveasqd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gjfsnpllk.sHtML

[J06] 计算两时间之差
来源：http://www.share.zdbjq.cn/Article/details/gwhawghcg.sHtML

Py:   (end - start).total_seconds()
来源：http://m.share.zdbjq.cn/Article/details/gormmenmk.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.hesvh.cn/Article/details/gxvvrpxjl.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gfopatuig.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gvihpivbo.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.hesvh.cn/Article/details/gbwyqiebx.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gqbuthiwx.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.zdbjq.cn/Article/details/gpvqikhst.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.zdbjq.cn/Article/details/gdtjgrsxl.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gglasysgi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gsarsrooo.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.hesvh.cn/Article/details/gqsccmxrb.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gjnrufmlk.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gvbollsyx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gkwlgjsnt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.fehbvm.com/Article/details/gqtjfqqfr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gybogfdvc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gmrbtfufy.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gvtjochgk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gbhleexdn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.fehbvm.com/Article/details/grcjgbmgo.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://mobile.zdbjq.cn/Article/details/ghfsoxadh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gurjwhtng.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://m.share.zdbjq.cn/Article/details/glbfzvuab.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/glxsxebxm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/gcwnpedbr.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.zdbjq.cn/Article/details/gwhxudclz.sHtML

[J09] 时区处理
来源：http://read.share.zdbjq.cn/Article/details/gepaygtcw.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.fehbvm.com/Article/details/gmonifroc.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gjpaqlyvg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gwbrxctsj.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.hesvh.cn/Article/details/gqsbtcpkb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.hesvh.cn/Article/details/gmjimlivt.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.hesvh.cn/Article/details/gghukmdme.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.hesvh.cn/Article/details/gryjcrcdm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.share.hesvh.cn/Article/details/gwugqdvku.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gecdrixev.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gyafyzlvc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gfgjfmttp.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gerzdvrer.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glofushlz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvyuxpuha.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/gbvsgwfpy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/gwhgrmacy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/giilejciv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxhrwlzow.sHtML

K. JSON 与序列化
来源：http://3g.hesvh.cn/Article/details/gptfgtknh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzoddoowg.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/giwvpvwnk.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gxfhlzlok.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gbzzzazgl.sHtML

JS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gprvqgzms.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtjwahaff.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gtrzipwsf.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gzmmxvptl.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.hesvh.cn/Article/details/gibaaplhk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gtyrsbrfb.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/ggkohqcat.sHtML

Py:   json.loads(s)
来源：http://read.share.hesvh.cn/Article/details/ggqafoevh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.fehbvm.com/Article/details/gbuxfrhie.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gyyhyxhro.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/grztdcdkt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/grmansyvx.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/greypesuc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gmfmbyqnp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gnghqwdfu.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gzgdzijsk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gipbcrxnz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gyakvsojc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gcykmgwsd.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gramettyi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/gbdervupt.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.zdbjq.cn/Article/details/gpfowbhlu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gwtzsfyqv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.hesvh.cn/Article/details/gcdjrfjhm.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/giezzylsu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.fehbvm.com/Article/details/grofxvkbx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkvalqmjw.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gwcabzetj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gjsdrbpes.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkkxvyg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/ggaurtzjc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwzcgyxft.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/gerqitwrp.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gsvhsmqfe.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/grihlnybg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fehbvm.com/Article/details/gsoxihgsf.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gpnbeumow.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/ghwpdmexh.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.zdbjq.cn/Article/details/gxgclhfdr.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gqiocaxnw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gslnnyhmf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/gxsbktsvj.sHtML

[K06] 解析 URL 查询串
来源：http://baike.fehbvm.com/Article/details/goyzeckhp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gvmnsoasl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.zdbjq.cn/Article/details/gofouhfdv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gglyuukmy.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/giwlkgtzl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gsuxekqtf.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/gbcpyytiz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/ghwcsqzmb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmpppqa.sHtML

[K07] 进制转换
来源：http://baike.fehbvm.com/Article/details/gqoepvaov.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/geyzblekl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.fehbvm.com/Article/details/gpivunehi.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/godcdckmw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gudwkqyfq.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gjoochatr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gvrgazwch.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.zdbjq.cn/Article/details/gofluvfps.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glkffkcim.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.zdbjq.cn/Article/details/ggxcgyags.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gsadcwsfi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gteylhpjo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gtqiswevh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/goccobbyp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gldqwyqfm.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gcdtrvlbm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glnjwkxiv.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gxjfgbfxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfjbrxyxn.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gfvnwuryr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqhyphwfs.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gdncdfodt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/grhtythrw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gchkbwokq.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gftesoqgy.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gwedkdnji.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gbrbdamhi.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gmbyiffcx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gcwwygxjz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gkaxfggpj.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gjzkbajdu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gamxzfmkk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/goycfiazh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/glztolmmr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/ghlputrwz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gfaddkecx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gvxhvwxpc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/guhnhjgyp.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gxuggjaem.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gzegaften.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gklwbhryc.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gupvqzels.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gtocdadpd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gqxjbpmdi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/ghfdzowtn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/grrrmebqi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gbmalvdvg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/grbglusxc.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gvrkarpwd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gkaajhbgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/gosonpgaz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gvrarczfl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gvfaergtt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gpoofgmhw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gokybrlzz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gxyfvxxcf.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gqyeuphdp.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/gibmipsup.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/ghgbzfzkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/guxiqrnyj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gaglignyr.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gsjpcjmfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/ghahizqoa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.zdbjq.cn/Article/details/gileutics.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gwtwjkvdj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfkecqbtw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gfphikqib.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyttqdkbb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/ghgdkbetw.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/ggehcppho.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gtncgnryz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/goqfkrpyd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gemqxldec.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.zdbjq.cn/Article/details/gdijwwtjw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.hesvh.cn/Article/details/gfcxufozc.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gsqvygabo.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.hesvh.cn/Article/details/gxvpwnqfq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gloplerzi.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gujahnpqz.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gthvqwpfy.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gphqjueam.sHtML

Go:   resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gelbxqsep.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/grntebdnz.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gfprvcyqb.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gmznnitin.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gkyztqgcu.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gxxrwvcns.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/grzdskkvs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ghacvfzkv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/ggzctsegt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdjkffuiu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gpztemzrx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gslmqelpu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaoyihdfu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gffvgaulk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpidohcbs.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gapxtyxyf.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gkivrupon.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/glepmxftn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwloejiim.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gcoplgnft.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gqzerbgqg.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gzwanihzm.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gftmcqdue.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/gjfvqguhb.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gucpckguh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gzrcuaqhe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gphhgyhpu.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gqialkrds.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gbihoazkw.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/geybmghjm.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gylgmvxcf.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.zdbjq.cn/Article/details/gcpiuzuuf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gclotxaxh.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gwoqjixhl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/gagsglnjy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gfmhmidof.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gwgoynuai.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gceaehgga.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/gsygnyjeu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/grjwlxzfv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gstexaklh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.fehbvm.com/Article/details/gfzulaedh.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gflorgkwk.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gvptwsebf.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/ghgmokoby.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gtwzwblbn.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gfphoztej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gatfmbdin.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/ggbluyxne.sHtML

Ruby: Dir.pwd
来源：http://mobile.zdbjq.cn/Article/details/gvqfztsnr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gfdupoynj.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gnzyhwwmg.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gjvsgeekt.sHtML

PHP:  exit(1);
来源：http://www.share.hesvh.cn/Article/details/gyozvylvv.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gilwbbkfi.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gcyxbyiew.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gugsgyogd.sHtML

Go:   os.Exit(1)
来源：http://mobile.fehbvm.com/Article/details/gerizqefw.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/gcxmwlzgu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gpbgsdfie.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gfcuudpcb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gvqzbyncy.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gaaeupxpu.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gpksiwslf.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gkfuqarlj.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gicuinkut.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gxyzfzuaj.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gxckldzmy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gslcajebf.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gjnwvdioh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gcjrlcmme.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/ggkhnantz.sHtML

JS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gydktyojs.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gjkzsfjcs.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwfksvqfj.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdwdkslqy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/guxufnvsk.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gizogouqb.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.zdbjq.cn/Article/details/gttumzfwt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gspmpoqet.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gtsgrsudh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gfwadtppt.sHtML

TS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gimahnfxd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/grrvmdhxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gzwgdwlqh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gtfpgfqbg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gyyukxsxt.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyncwxjhr.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gjojhvotg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvoonpgsq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/gaftunsar.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gaqcpzkfj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gqezqlzpm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/givuaumdr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ghbnubvfl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnxihpbro.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmxneqrut.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gcfoxjtpq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzhpgbiqb.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grpypccjr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gfgllrrmc.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gssbwdcba.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gixvuccmq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gnlthxbhd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.hesvh.cn/Article/details/gcsghppfk.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gphircxvy.sHtML


<!-- 参考信息 -->