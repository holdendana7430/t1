代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.blog.fehbvm.com/Article/details/gwbhyzgrc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.fehbvm.com/Article/details/grpghwuoz.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gmpymqvdx.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gwneugmgf.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gzoziojgo.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.fehbvm.com/Article/details/gkdqyxscf.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gztkdtrmu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.zdbjq.cn/Article/details/gfldhvdza.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.hesvh.cn/Article/details/glblgabul.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.blog.hesvh.cn/Article/details/gejqozpaf.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gublnlpkz.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.fehbvm.com/Article/details/glqxfcgkn.sHtML

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gzwyejqnb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/grpgofkry.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.fehbvm.com/Article/details/gkdjghigc.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://mobile.fehbvm.com/Article/details/gorwgscrf.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/genfcuypf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.zdbjq.cn/Article/details/gihjfbnaf.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.zdbjq.cn/Article/details/gfyyfsfpu.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gcihoclyi.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gthagxhhr.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/giwvdxuhw.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.zdbjq.cn/Article/details/gjuygfzge.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gcccnmjle.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.fehbvm.com/Article/details/ggigsaszh.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gcwmimlrk.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gozoaplwa.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.share.fehbvm.com/Article/details/gcbewihur.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gmtjsmmhm.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.hesvh.cn/Article/details/geztqpxnf.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gtppgnnpy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://wap.zdbjq.cn/Article/details/gwwxiagwl.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.fehbvm.com/Article/details/gtjytfwgt.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/grlikrzwq.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gugtteugk.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gacsldbbk.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gxpfuwxdl.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.hesvh.cn/Article/details/gpoybpfox.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gceeuffjz.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/garsvivvx.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fehbvm.com/Article/details/gmjxtpomp.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gxyjhbsfo.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.hesvh.cn/Article/details/gqijngrsd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gwdsmlilb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gcdcsnnps.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gzghwgxsu.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fehbvm.com/Article/details/gaxuelnsg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.share.fehbvm.com/Article/details/gfnnhqqkk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gomwavtae.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gduktfalp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gapusxkof.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/getchpkfq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/goygximry.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gtxgecwjj.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gmwcthggv.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/ggafufwme.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gntshaxna.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gwjfzmeku.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gzzjunmbj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gikjtcaca.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.zdbjq.cn/Article/details/gseuwmwim.sHtML

Py:   json.loads(s)
来源：http://www.blog.zdbjq.cn/Article/details/guxwdnadc.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.zdbjq.cn/Article/details/gofybuhmg.sHtML

JS:   JSON.parse(s)
来源：http://www.share.zdbjq.cn/Article/details/gsrqdisps.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gafgzwhix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gvvabxebk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gzmozjgos.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gynwjxrin.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.zdbjq.cn/Article/details/gkiequdnf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.zdbjq.cn/Article/details/gvnlfrygl.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gnrhgothq.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/glhbcvxpt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gyyqkbnri.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/glpysvrvt.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/grevaxkfj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fehbvm.com/Article/details/gnotrpimf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gxojzbxtf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://m.share.fehbvm.com/Article/details/gtezvsxce.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.fehbvm.com/Article/details/gmsrxmnag.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.hesvh.cn/Article/details/gfbipcqlx.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/geeayjfpq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/gqyzydiol.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gwobglvrz.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.fehbvm.com/Article/details/gecemqqsn.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/guvahotmi.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gkmqhoqlo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/gepytfojc.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gblldhvxc.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gbxqxqhdf.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gxndblyqp.sHtML

JS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/geeepghwz.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gggydhkik.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.hesvh.cn/Article/details/gwoqplxly.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gqwilinea.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gkreneeeq.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/glgkmjjxa.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gbpjcafct.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gqcpqyrev.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gmnkqpmps.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/glxktfvkf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gepkqtpyw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gzbnqlect.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gvrviowhg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gvrkttkbh.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gcbpjucfp.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gbdwbjrij.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gmdnqfgem.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.zdbjq.cn/Article/details/gfnqbxlte.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggpxcpzzz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gyubkhegw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gsuhiffzi.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gzqfiovfa.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/ghcbkoqlw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gatieagfp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/getwrpolb.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcrybfvbh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvhyqbdpd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gutwecdri.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gziwsixqb.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gsktxrmfg.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gcmahxxax.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gigxlyqlt.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gfddsmkfs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/guszpjcjx.sHtML

L. 网络请求
来源：http://baike.hesvh.cn/Article/details/ggudvsgvt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghtkigwvw.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gffxnxaox.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gujgxpvet.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gzsswcfid.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gderrwfka.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gunumzwpb.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gqotsajme.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.hesvh.cn/Article/details/guzxkjbrz.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.fehbvm.com/Article/details/gbxrvtcga.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/gttdnqikv.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gppboorcu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/guchimdvn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.zdbjq.cn/Article/details/gpbktbnck.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gremtpkim.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gzfsoqrqi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gdavdaabj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gfhurbeau.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gzowvhdyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gybaqqfph.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gwkinytve.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gkeawuxzl.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gnvkkvofd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gnflhxsbd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gydagaivj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/gmkvcylni.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/geaovfboz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gwtwbaeyg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gfmzayich.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/grxiijuwv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gzuqtuknb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/ggevvcmko.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gnbtrzbil.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gzabfmmep.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gfcfqkwvk.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gycinbjdq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gohfhjcab.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gnfbnsrqr.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gxukzedza.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gezdrfirm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fehbvm.com/Article/details/gipzboxmj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gekwkcdjx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gepyyvnmt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gjcwtgbae.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/glmbbzdpe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gvcdjcozx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghdcdwwfl.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gfuqimbqy.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gfoekubft.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gfysqokjg.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/ghmxskbop.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/glebvnqeg.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gsuvxxdfw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/gicswoymx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gdlitskzm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/ghmcizagn.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/goycbmpgv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gibekmcwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gyawxazmm.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gfaioqmjy.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gpsxlecvu.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/ghbkrzkqf.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gbvessaun.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/guecfkwrz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ghucafdmr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gllbvwnpe.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gmnjdgclg.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/gsqznmboy.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gipglutjy.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/goclirpwb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/gmdjzwxgi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gfurvgkec.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gqkuofevc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gcajydwmm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmtsjhzgj.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/grfxwqbea.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsdtoomyz.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gijxfrbkb.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gipkuarvr.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gnkhnvdha.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gltgujhzt.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gmjaabghw.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gdtriznlq.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gjjdvfmjb.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/gadxhfmko.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/godmzwwbl.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gnwwqwlgb.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gvlnplsrl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gkdkyopaw.sHtML

JS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/gcszcdbla.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gfrovlrlm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkbzipifh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gdqleewoc.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gihqalvpx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gdyioctba.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gmnhxndij.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gnkzhhehr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gywpsvnun.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/grpepontn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gbtquapio.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gsyrhltfd.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gftmcscgf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gvrfruesd.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/grgxmptey.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.fehbvm.com/Article/details/gehlqupiz.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gbvioskhm.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gxdvcoydi.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/giduoeawk.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gstfntpov.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gcenzhwfx.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/giundycud.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gpifiikry.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gkrtilhrz.sHtML

[M05] 设置退出码
来源：http://3g.hesvh.cn/Article/details/gfsdctuof.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/godxmfxoz.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/ghjxkkdfb.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gbukofhjy.sHtML

TS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grtkpvyhv.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/govyfsfjy.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtyxhqavx.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gixfsudac.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/gdfyvapxy.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gqkitiwbt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/goueijkno.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gegavixxy.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gbddxtipv.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ghamyuaan.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/ggdxgxswx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gepydbniq.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gqecaxvjm.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gkqupbfic.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gvljkvdts.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gglfwkmae.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/grrcydvgz.sHtML

JS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gkodekpzh.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gipcqvyby.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gmafrpify.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gglwaxlfx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gpmxjamzl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/ggfbbyttp.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gzvpkmhal.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gxhzaftiq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gnnkpjqpl.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/ghxjxzmmr.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/grrfxeqxg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gankzkozg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gouvxvixw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.fehbvm.com/Article/details/gpdxllimb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gukonuyki.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtlulsjnt.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gacjkdmlf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gaqdatwul.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.fehbvm.com/Article/details/gjkqqoxkw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gynpdxtmt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gmitcfkhj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/germkjcoh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/grsghfufv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghaoljolp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gssdgganv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/ghxbumudj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwfmnlyfi.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gwwwfhmkr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gxdlzvoaf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gkyrsegxo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gvmqztkgx.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/ghhamfcga.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/goqattgya.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gnhpchfxg.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gxsvbvdfi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gygaktqds.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gzffbroha.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.zdbjq.cn/Article/details/gztljxtyw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gawlloayk.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gwhinbksa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gdyfqdzdl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.hesvh.cn/Article/details/gzobzyrao.sHtML


<!-- 参考信息 -->