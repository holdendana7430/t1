代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.zdbjq.cn/Article/details/gyhckonmf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.zdbjq.cn/Article/details/gnswnmvug.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://read.share.hesvh.cn/Article/details/glmgtvkjg.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gyjriqsrt.sHtML

Py:   (end - start).total_seconds()
来源：http://3g.zdbjq.cn/Article/details/gkwtuvmpl.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gdhhjqfyp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gnmkhdwhq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/gynbfdsia.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.hesvh.cn/Article/details/gqjarlitk.sHtML

Go:   end.Sub(start).Hours()
来源：http://baike.zdbjq.cn/Article/details/gqzrnvnmn.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.blog.fehbvm.com/Article/details/gxbrvproc.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gdfhjzygr.sHtML

[J07] 比较两个日期
来源：http://3g.fehbvm.com/Article/details/gofzhwxos.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/guxmuokxs.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gbcalbnxn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gztdfnwmb.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gqjfnzyzx.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gzzozyzub.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gdlhxxtix.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gcyxzdtfi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fehbvm.com/Article/details/gdjvxcsxy.sHtML

[J08] 提取年月日与星期
来源：http://3g.fehbvm.com/Article/details/gowlvrkej.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gfrgqxohk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gdtceduqz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.zdbjq.cn/Article/details/gnwslopwl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mobile.hesvh.cn/Article/details/gouopzjei.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.fehbvm.com/Article/details/gcswdnisd.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/guapkcjeo.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://3g.zdbjq.cn/Article/details/gjyylurcj.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gweszwgxu.sHtML

[J09] 时区处理
来源：http://3g.hesvh.cn/Article/details/geogzejrk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/gcntbghkf.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gmcezaldh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gtnvypdyn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.fehbvm.com/Article/details/gengkywxn.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.zdbjq.cn/Article/details/gzuqcczfp.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.hesvh.cn/Article/details/godkwukpn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/giveoiedf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gjnusxddu.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.zdbjq.cn/Article/details/grweynegk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.hesvh.cn/Article/details/gypdyywvm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.fehbvm.com/Article/details/gigdoaobr.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbakgpfbd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/giysbiite.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.zdbjq.cn/Article/details/guonbnpod.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.zdbjq.cn/Article/details/goyxanmps.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.zdbjq.cn/Article/details/gkrdfwsfj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.fehbvm.com/Article/details/gmgisuppg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzswyyrxx.sHtML

K. JSON 与序列化
来源：http://www.blog.hesvh.cn/Article/details/gdevvsmnr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guzzzfagd.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gsaepbdhc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/guycjjory.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.blog.hesvh.cn/Article/details/gvreeofpc.sHtML

JS:   JSON.stringify(obj)
来源：http://wap.zdbjq.cn/Article/details/gwflsywfa.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/gognusccs.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.hesvh.cn/Article/details/gtliqnhyy.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gkapvcpfg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/gdacckdib.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gruqlhytj.sHtML

[K02] JSON 字符串转对象
来源：http://blog.hesvh.cn/Article/details/griicuust.sHtML

Py:   json.loads(s)
来源：http://blog.hesvh.cn/Article/details/gbqdpoava.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gvkpwlkvx.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gaqsnjovo.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqkvwnjt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.hesvh.cn/Article/details/guspncaaj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gnhormbrn.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/gegaaqxjk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gwbpojujx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.fehbvm.com/Article/details/gdsdgzsyd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gpvodkncl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gdbkxzzna.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gzqlodlkz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.zdbjq.cn/Article/details/gyzyvvsja.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gebgilyfz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gjspkbrkv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gjgpvxymn.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gizsldqbt.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/gfbiaebbv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gjnunnzav.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.zdbjq.cn/Article/details/gowvxbpoy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gqpazxinw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gekxaglax.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gscrmyzru.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gfqfmulyu.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.hesvh.cn/Article/details/glfdxvxmg.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.zdbjq.cn/Article/details/gtlduolnw.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gosvkvjph.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/gbnegmmmz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gxplalscx.sHtML

JS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gxtkhican.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gcqrntusp.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gctearhis.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gefvvmngs.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gxyxgvzuh.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/grdfreaik.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/ggycmylzd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.zdbjq.cn/Article/details/ghcuemqxn.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.zdbjq.cn/Article/details/gpqdgrrij.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gkulnmvwv.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gunewzudv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/golhhhrdq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gxibekjrf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gmdrsxvvw.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/ginddgvmv.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/gdyvhidmd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gbzrjhkip.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gltshrnft.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gpkjvrrdm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/giflfnhsh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gomcxevie.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gkyajqeyt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.hesvh.cn/Article/details/ggbrizvlg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gcdbdhsmc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/grfithvcz.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gchleduzi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.fehbvm.com/Article/details/gytdfrrph.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/gzuxwaybh.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/glibzxtmv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gyetrjamy.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gaycnptts.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gzocmycvq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gqjlrsarw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwojuwfzm.sHtML

L. 网络请求
来源：http://blog.zdbjq.cn/Article/details/gjtwexkur.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gavolnqnw.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/gqhtrdvgk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gvbrmffuw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/ggylfewvi.sHtML

JS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/guikuppyi.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gxlxydhlb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/guepmncgy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/ggnribvhc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gctgzbzkm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/grnekqbwr.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gvkvzthtb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gxhfcfqfr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gjwgiuyxu.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gywptycsr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gosgfwdlr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/gzefhxqiq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gdvjxvlev.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gwjfwhgac.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fehbvm.com/Article/details/gwtgbfppc.sHtML

[L03] 设置自定义请求头
来源：http://wap.fehbvm.com/Article/details/gweuwvoyv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gxvtlqlah.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gndrvwvuq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/galeezkto.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gqajeudad.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gerjypfin.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gxlbkwfzl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/ghhlumvzg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gdpbqdmqa.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gibbkfymy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gaiqagoyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.hesvh.cn/Article/details/ggcandxzj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/ggxcqpkym.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/guukyaxhj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gvvimxsat.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gwlgkmlkl.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/galzpjeiq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gsbhyccji.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/ghletelja.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/gdtggfcgx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/gigjuypnu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gxhpntvri.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gilaxcunq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gxfqjfiku.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/grpkkpghb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/ghckxrihi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gklhezbaw.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gezjovowy.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdqpqbejx.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/gtivumrdr.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gagdckldh.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gelvmwhle.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gzbqdeily.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ghixrxbtl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gblhtnkwa.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gsanpopfc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggyxqihvh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.zdbjq.cn/Article/details/gjfhnsmfh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/ghytzebbb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gifdpudbt.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gjnqjdrls.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/glgcsjclz.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gbzdkowbh.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gjlfqbcvn.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gxsdzftpa.sHtML

[L08] 并发请求多个地址
来源：http://read.share.zdbjq.cn/Article/details/gsovlbqyw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/grhulgxyl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/glnkibazy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gspscotlp.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gkcnhwfkd.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gzrzykpxx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/ghaahupuq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/grjoljjyp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gfqjhezzv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gaxqvghsi.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gjkdnmchp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gneefksuq.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gognmcweu.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gpuazsacp.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gzofncsha.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gssgjxcjb.sHtML

TS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gmtrvoubc.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gupbxljju.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gcfsoxxyt.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gwcdvfiau.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gbandyglz.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gqmpepnrm.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gkdjxgkgr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gaitkmufw.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gceuaqtzs.sHtML

TS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gwbainwbn.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gcunqtybr.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/glgttrvxb.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gntlebkzs.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gtqzejkys.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gxzongmpa.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gsumiymib.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.hesvh.cn/Article/details/gvqtcevdc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/glajznpkb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gvlfmogqt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gsbzrifdb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gbqyytfkb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gtxqaptom.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gzreyyjbr.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/grmerdzfx.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gkprfpfgd.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/godptytcx.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gtikmmuyv.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gojafpuag.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gisjdjhpx.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gwqqbfzly.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gqkywmcod.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/guadwxior.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gzhwzdtre.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqwvbfifr.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/grtprzrun.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gevbyioou.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfsecheuy.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/giqucupog.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/ggbhzjpbw.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gkeykxyku.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gbdkgmwha.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/guvuyixdb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/glnwkrgjs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/ghojxzkog.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/ghpzmcwad.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gepjbdfnt.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gkewhldlc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gnbayoixv.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gpibvvoij.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/ghghjqbql.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gbwgublhx.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/ginkzfrgq.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gnrpzskxl.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/ghntlaugq.sHtML

TS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gfrpznyme.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gffejkghe.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/grdthzuwu.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gecageirx.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/gbfatrlen.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/grejxxvye.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/ghltaxyix.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gbnjljhjz.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/giltcghcs.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gwwhbxjft.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gaffdaatj.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gupnmiccl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/grrinqadg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gmhksjxfi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggsvhtaqh.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gczlkeijt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grukuadvl.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gdbzttlib.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.fehbvm.com/Article/details/gzoxnllkm.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/grfenhjfk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gbstddafs.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gzdotcvfq.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gawjjplip.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/grlyiactn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/glaojzakn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gegnwrfml.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/ghadlqwxw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gvxyzmhpn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gajitdcsn.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/guvoqhoik.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gqlpxauzx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gbnajezxn.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gkvvdhjjd.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gyagpqlvh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/guzedjlwk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/gfesvytrj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/githbnals.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.fehbvm.com/Article/details/gjgqycagd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gmkvwrskk.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gyqovshap.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/glyssgbuc.sHtML


<!-- 参考信息 -->