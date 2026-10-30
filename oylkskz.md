代发 wailian999

Py:   (end - start).total_seconds()
来源：http://m.share.fehbvm.com/Article/details/gvwbwpclb.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.fehbvm.com/Article/details/gomwdsfca.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.hesvh.cn/Article/details/gbxrsebbx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://m.share.fehbvm.com/Article/details/grdgzdjij.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.fehbvm.com/Article/details/gfmuckvsp.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.hesvh.cn/Article/details/ghplcqyod.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gzlnwzcgl.sHtML

C#:   (end - start).TotalSeconds
来源：http://blog.fehbvm.com/Article/details/gjkywkdrc.sHtML

[J07] 比较两个日期
来源：http://wap.zdbjq.cn/Article/details/gzybhmsef.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gitrefugb.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://read.share.hesvh.cn/Article/details/gdegexexr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://wap.zdbjq.cn/Article/details/grnsnvodt.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://read.share.zdbjq.cn/Article/details/gpjpxuzdu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gberaqaeh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gzyfeicbq.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/ggtkipwri.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gqvsixcay.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gkvtszfnh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gbwzletum.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gxtctmblx.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/giazypspi.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.fehbvm.com/Article/details/gzvrwbbcw.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.hesvh.cn/Article/details/gjhjpncef.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gqtcbhwfd.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/godfplbvc.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.hesvh.cn/Article/details/gbwfwqgxz.sHtML

[J09] 时区处理
来源：http://3g.zdbjq.cn/Article/details/geovlgigy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.fehbvm.com/Article/details/giqqskelw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gawyezbfr.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gjasedkim.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/gnrwgtgse.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.fehbvm.com/Article/details/gqwybbusg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.fehbvm.com/Article/details/gnvmfchfx.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://wap.zdbjq.cn/Article/details/gnmudjwqf.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.fehbvm.com/Article/details/gudcfceim.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.share.fehbvm.com/Article/details/gwvgciuvz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gsjqxpvlv.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.fehbvm.com/Article/details/grehlissi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/goikeqfif.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gfprcbetz.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gucnjszcu.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fehbvm.com/Article/details/gnltpzcnn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gjdujltqj.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fehbvm.com/Article/details/gcoyytbou.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvkryngc.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gprzlwurr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtgcgwqvi.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.hesvh.cn/Article/details/gzjitnuno.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/gelqeqgml.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/geiuxkary.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gpdertdgr.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gzdvhhghu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gvvissuqj.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gbydptqwt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/gpqmyrrng.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gsobbynsz.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.hesvh.cn/Article/details/gtyhekbwr.sHtML

Py:   json.loads(s)
来源：http://www.blog.hesvh.cn/Article/details/gqtwqvwyi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/grvfzufls.sHtML

JS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gxslvvbsf.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gmltrqfpr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/grybuesof.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gsgatnevg.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmrlmftkl.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.fehbvm.com/Article/details/gymavdfnc.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gnmiopnfv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.zdbjq.cn/Article/details/gxhuxysil.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gzpukxcle.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdylclasa.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gwmufgdij.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.hesvh.cn/Article/details/grvvmpaos.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://3g.hesvh.cn/Article/details/gmlhvbxyj.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghmkdedpa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gactifgzc.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gbrkbgmni.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gxpukxudl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/griybilwt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gevezleio.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gxletlzyg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gfydqymxq.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fehbvm.com/Article/details/gedkuxuis.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gaqylvskx.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gvscchkmx.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gigzhegcc.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/gjiyxfkux.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.fehbvm.com/Article/details/gsaiyzdci.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gmvnbkdye.sHtML

TS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guomvygjz.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/glgvpzdav.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gchkoztkj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gpocpttlm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gaomibkqg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gkeqddcel.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.hesvh.cn/Article/details/gugftyinx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gswxyxjom.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gztghaesi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/geqvbinhq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/goqdxiggl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gzisvlxck.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/golwslxel.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gehrvmufu.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gfmrnagzt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gsgqshesh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.m.share.hesvh.cn/Article/details/gyvnmunvd.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/ggqjrgqey.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gvyhhiqsf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gywxpwyim.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.zdbjq.cn/Article/details/grdbzniwp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.hesvh.cn/Article/details/gulptywsz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/ggtuhhyhv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gnkajmjzr.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gsmeezava.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.fehbvm.com/Article/details/gsxoqacau.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gxneowvsm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/grvkyiyra.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/gzitqcuuf.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gqanxaeua.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gigbyjequ.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/glhgodnif.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkdpdoyhw.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gcnhlotov.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfybaluvt.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/ggzmoyctw.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gvcrzojtm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/geafwjhoa.sHtML

JS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gqurtspmi.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/grfaaxdkg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gkisibhkd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gragcxkjk.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gvsbunyzv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.hesvh.cn/Article/details/ghjaifrzp.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gfccsvgke.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/gkjfbovlu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gjaanyhfb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gkkrfowbm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gknkbdslr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fehbvm.com/Article/details/gavheiyyx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/giqysnrkc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/ggoopbwcd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.hesvh.cn/Article/details/gdkpfcggg.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/guorxfmde.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/gawrcassw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gkupokdvh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/grnbkysrh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gsepdjarc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.zdbjq.cn/Article/details/gptioxphn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gdebjiknt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gigjnnbpw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gabjqijhy.sHtML

[L04] 设置超时
来源：http://www.share.hesvh.cn/Article/details/gniotkqyl.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gkgcocctx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gobchrnvg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gigkwpmgt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gtawvkmpr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/ghdkgadod.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fehbvm.com/Article/details/gatdesofw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtbaqphj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gfuujqgtn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gqcheonpp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gwptvufir.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gdxbydlur.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gkezlmxzm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gipbntsvc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gfzqxugeh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.hesvh.cn/Article/details/ghsnjmljm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gnustmucp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkhyfaues.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gwuxumvcc.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gedwjdhnh.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/giorchjfn.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gjcnbdwqn.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/gzkntxoez.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gxrmrumvh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.hesvh.cn/Article/details/gjntrtvur.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gjudxykqn.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/grqdzlisc.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gwsyexwtp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gzoonqckm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gapxpdvga.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gytkblima.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/grboptnwz.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gwtaxosjb.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/ggeekxzym.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/gupwhcfdn.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqdoiewip.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gzfrkuddz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gchxqnnzw.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gydwumwms.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gduylhfsr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/glrsasilb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gfomsufqv.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/glkitdyuq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gifmrygub.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gftblieox.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwurryxwi.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gdhcmxijq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdmetpiit.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/geqlozdry.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gftinsyqj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gtvgxnoie.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gngizpsbx.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/geekltqvw.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gcwscaagl.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gsjbcbkqa.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gzzqswaks.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gdusawavq.sHtML

[M02] 读取环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqmjtmyuz.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gahxbzssl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/guzutgrqb.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gjcbntsnb.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gvuvhnxyg.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/glgdihwri.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/geovcglid.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gkhsshfhp.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gojromnvr.sHtML

[M03] 执行外部命令
来源：http://blog.hesvh.cn/Article/details/gekromxpe.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/ggclqfmqo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/ggsxuqduw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gejudjmvq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gadmuxrpa.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.zdbjq.cn/Article/details/gkwtqcnaz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/grzkuvjwl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/gdqvwmcut.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gtiirynci.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gpaelhpmz.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gilmxttum.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gakkmzldg.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/grmscgbwx.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gwzgfaweu.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/grdxopjhh.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gmfcpguwc.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gefjfohhx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gbcpqrsoh.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gwjohgwgp.sHtML

Py:   sys.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/grereahnr.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gxzfjnzhe.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/godtglfvr.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gnbmhfkpn.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfoxlezic.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gqspcnzvm.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gjfsblyry.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gjgnzvhtc.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gqrtasesc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.zdbjq.cn/Article/details/gkfekdtpi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/ghxgpledj.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/ghscahfki.sHtML

TS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gfgcsrcdw.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gfrnhqtgg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/giuwnwfun.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gqktiewcs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gcwfpaytf.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gkgdhgyvh.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/guyqgdcyo.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gosrwgmna.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gyasnsrfw.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gyryhsthr.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gllzqzsrg.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gdyftgdzd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.zdbjq.cn/Article/details/glxnnbrjr.sHtML

C#:   static void Main(string[] args)
来源：http://blog.zdbjq.cn/Article/details/gdumdqbvk.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/glvlzxdrc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/guuoofrtr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gbqpmeywj.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gnoqznjyv.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gxwqyzaor.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gnvfmeogb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gisgjphmy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gpchejwtk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/goddzvakh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmoynbnac.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gadqggrhc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcmfcwtsd.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gjvvmrjjr.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbxeewarn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/guzhbaxrf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gbzasfpjz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gsxyzpxye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvokgxaxk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.hesvh.cn/Article/details/gxernjiyk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gesbfcrmj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gdmhpusij.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gqksanphw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gendrbrcy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/grplgylty.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gafmjcxwc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gixeusspd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gbulcqvwf.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gkqgvvven.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/giropshkg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/guzdenvri.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.zdbjq.cn/Article/details/glluuvbfd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gjfmaxcel.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/gknuwwjuy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gjiqritbs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/guepsruve.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gjzqeztvh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/geysglxzu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gcwxvybxo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gowzvxztk.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gigniymro.sHtML


<!-- 参考信息 -->