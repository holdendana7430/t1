代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gwerzldvt.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.share.zdbjq.cn/Article/details/gbmhrghia.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.hesvh.cn/Article/details/ggbmpuvpj.sHtML

[J06] 计算两时间之差
来源：http://mobile.fehbvm.com/Article/details/gjkilmdif.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gaffmhqhr.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.zdbjq.cn/Article/details/gxkbtlroy.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.zdbjq.cn/Article/details/gzxaohbiw.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.fehbvm.com/Article/details/glylpjypw.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.zdbjq.cn/Article/details/gwjmxnest.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gvoavnmoe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.hesvh.cn/Article/details/ggluscgll.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.hesvh.cn/Article/details/giuqiggph.sHtML

[J07] 比较两个日期
来源：http://baike.hesvh.cn/Article/details/glqbquunf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gdkvvvhfz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.share.hesvh.cn/Article/details/gupdsjdvg.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.hesvh.cn/Article/details/gilwjpshp.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gpobcfttu.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gfkxblmxt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.zdbjq.cn/Article/details/gbqjjpyah.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gbbmkwvfh.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/ghonhieno.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gtxnigsyo.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.zdbjq.cn/Article/details/guimqxwrn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.zdbjq.cn/Article/details/gnfqtcjpz.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.zdbjq.cn/Article/details/ghrydhshl.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gmlauwegf.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gngpoepvi.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.zdbjq.cn/Article/details/gjbhsfmwl.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.hesvh.cn/Article/details/giwjfuwce.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/ghtxxcvcw.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/ghqfucdxu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gpeejcoip.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gsjtnjnsg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fehbvm.com/Article/details/ggtbywpgt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gewvbrrpt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.hesvh.cn/Article/details/gsswctzxy.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gysxpfjbt.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gykyfsquk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gvouefwyu.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/gxlqafifp.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.fehbvm.com/Article/details/grdtlrgdo.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gskyaifbd.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gqyxhmkwq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.hesvh.cn/Article/details/gumloxvpo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.hesvh.cn/Article/details/gtkcexrnx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.hesvh.cn/Article/details/gzeldvspo.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fehbvm.com/Article/details/gzvzcorub.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/gfrqmuevp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbiupevnw.sHtML

K. JSON 与序列化
来源：http://mobile.fehbvm.com/Article/details/gkdhqzivv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkobxeidv.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.fehbvm.com/Article/details/guxnibjmo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/ghsgnugst.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/gvlbvtyuw.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gvvdvznuf.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghtaibool.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gqdllepcy.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/glpoqulsc.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gjpgeecrd.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzeetomhq.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gqmtwbybl.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnuukdody.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvptkwi.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gggyvbquc.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gmepeoyqu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gkocvceah.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gpxomizct.sHtML

Ruby: JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/geynpdfbq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/ggtruthmf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gyrzfucwy.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/givuhxfwg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/glabgtbfp.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gsjksmqzz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.fehbvm.com/Article/details/gepzavmah.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://baike.zdbjq.cn/Article/details/gyhcvwlwu.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gorinqzld.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.zdbjq.cn/Article/details/gdsjhgqvq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.hesvh.cn/Article/details/gwzzarakf.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gimcroukx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/gxdmhcgyf.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gmxnzxopr.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gnwxnlqma.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/ggmjemwuh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gpsiesgbz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.hesvh.cn/Article/details/gnejrujpp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/galyatgtc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/grqooycad.sHtML

[K05] 深拷贝对象
来源：http://www.blog.zdbjq.cn/Article/details/gyqoxplye.sHtML

Py:   copy.deepcopy(obj)
来源：http://baike.fehbvm.com/Article/details/gpfpaprxm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/ggwyyfsjh.sHtML

JS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/ggwqqbbev.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gziuyupfg.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gwddtnuky.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fehbvm.com/Article/details/gdgtrfujv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.hesvh.cn/Article/details/gtvuuzzux.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/gcqzfduix.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gwhhwstwc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gbteeilvy.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/gpjgsjikg.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gmjflnijd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gkwpfdwdj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gjowkweqg.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ggazerbkt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gsgajswrc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gnwrqioux.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gdlbzxbfo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/grjbkrapm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/grvibtpsg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gdcpmlfmw.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gdayqwrcl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfsultksx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fehbvm.com/Article/details/grrbmvwsp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gsbpxxkum.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gvrbswbaa.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/ggguaofkp.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gwuloaasq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gecwhdruc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gapjrxxss.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gvuevaguz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gffssrzqn.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/gaoxuvuqd.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gybygxndc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gkgttbfjn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpfwvwjtv.sHtML

L. 网络请求
来源：http://3g.zdbjq.cn/Article/details/glxbgscqk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gukyshfio.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fehbvm.com/Article/details/goanyuwqc.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/goacmglwn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gjncscryh.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gpvdrlsvk.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/guffpofkk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.hesvh.cn/Article/details/glulxvcpu.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gbpzigzdn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gqogjiydo.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.zdbjq.cn/Article/details/gapdirofz.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gwgulxrpu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gbzwaysyr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gvefupmhg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gzbtjjyfj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gvjbvcqdp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gdiyfhfdr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.fehbvm.com/Article/details/gflckameb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gmqwgtspm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.zdbjq.cn/Article/details/gadbpbotz.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/ggteurdaj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/gmdrdqvbq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gushswkpp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gschhftip.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gjffhfwvc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.hesvh.cn/Article/details/gqalgppnm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gsppqotsd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.fehbvm.com/Article/details/gfvcrgmws.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/groaavnlp.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gsgqrkpfi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gbcwmwbvg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/ggqyljxvg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gonxiuqjw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gfbkuoruw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gdhuvuaai.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gasmpukxg.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gxfzoygdl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gqgusxsij.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gpggkbeau.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/guzcscole.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gytvuoyyl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/ggvslnkqi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gdgtylvpj.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gmdlxfnqe.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gbuwccirs.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gggtdlchp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gtbehriuq.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gkgrrmqvt.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gxmbzphde.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gfwwsnhgu.sHtML

JS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gwgcvflyh.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/grrpoxqfn.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/gainautnp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gbocpiixh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/giazjntys.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gddenujli.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gnnfssynw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/ggkeqyglo.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.zdbjq.cn/Article/details/gmowcvwyi.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gobmfdjxw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/geosvzwpi.sHtML

Java: resp.statusCode()
来源：http://baike.hesvh.cn/Article/details/gbpmeaemn.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gwaukkwzv.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gkjxgwpek.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gjmseohuw.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.hesvh.cn/Article/details/gvaqvfzdp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gokysvorm.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.hesvh.cn/Article/details/gwrxjsjvv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gzlynubbs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gdkkgbvye.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/ghxezbzlz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gxlcxkkms.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gkiklbvpk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gymozpkam.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwgknmrxw.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gyrzybjqh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkdxodcsm.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gppxxwvek.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gpyqldzpm.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.zdbjq.cn/Article/details/grfbgpokd.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gpoalhhdz.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gcdzpmkgh.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gvotbmfrc.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gdervbezz.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gnxrogxja.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gbhgmoaot.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gssjydghc.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.fehbvm.com/Article/details/gmzetospg.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gqpqenvtx.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gdewluywf.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gebjshctj.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gtnrcbndn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggstggtgx.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gufuohpim.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/goiqfqwwn.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/gxfoxikbq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.fehbvm.com/Article/details/gjykofntr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gshyivcgh.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvhyoufjx.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gmbkpzbby.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gidcnenpb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gljovdlnz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gyzdryqkm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gqrbbigsr.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gqcwipctt.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gerzqixpa.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gawltfdhg.sHtML

JS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/glkogjuyn.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/ghptddxbw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gxyenhfos.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/gnpenjxip.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gqxddkqbu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/geomefgza.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gtezibijr.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gkamxyhcw.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/geamromzf.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gftiizopw.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gwsocindu.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gwldmdxgq.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjuhbwofp.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gmmhhkgud.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gaisbouim.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/glgsyvtdb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gjpizqfgf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gvrbusyyp.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gorhepxmi.sHtML

TS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gxkpvaacy.sHtML

Java: System.err.println("err")
来源：http://www.blog.zdbjq.cn/Article/details/gviwcbsxu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gwhnqaidd.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/grmbsbabn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gjtugthir.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gqokjrkte.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.zdbjq.cn/Article/details/gdneopxfa.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gphovawfj.sHtML

JS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gdwzgcvrj.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gnamyrrxg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/ghdcbdece.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gkkomjleq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gevnfgzvb.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gmtuolpxf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/ghpryjgoz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fehbvm.com/Article/details/ghxxsaskp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gianzfjll.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gjttxyspe.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ggpeagsup.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gwidtomib.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gebhuyndw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gdmmhbrsg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gefgracqv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzzxnmhoz.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ginpcefub.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghivoxmqj.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/glxlqwtqh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gpdgwwqwa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gdetwqzcs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gmhgxyxix.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/gxnpfmdbu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gjwauamfs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/grwuzezue.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gbnbeeest.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/guzzmykjf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fehbvm.com/Article/details/ggnrbjxpw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gixelqjzm.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gkwsnusqi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gcpbknmwa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gctafunxb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.zdbjq.cn/Article/details/gcyqsdqmq.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gkssfemcb.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gqdqhbkbs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gnjkhhoss.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/ghxeygtuy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gkigvtesj.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gcvlajugn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gyiedujiw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/guaawfhmz.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gckorxunz.sHtML


<!-- 参考信息 -->