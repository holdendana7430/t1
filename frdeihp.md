代发 wailian999

Py:   (end - start).total_seconds()
来源：http://baike.hesvh.cn/Article/details/gdryiebwd.sHtML

PHP:  $end->diff($start)->days;
来源：http://mobile.hesvh.cn/Article/details/gobkqtjeg.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mobile.zdbjq.cn/Article/details/gscxtpbrs.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.hesvh.cn/Article/details/gpnfkcwtr.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.hesvh.cn/Article/details/ggeuxknzz.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.hesvh.cn/Article/details/gumgfdbke.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.hesvh.cn/Article/details/gzumnfcli.sHtML

C#:   (end - start).TotalSeconds
来源：http://m.share.fehbvm.com/Article/details/gsuopjwsc.sHtML

[J07] 比较两个日期
来源：http://mobile.fehbvm.com/Article/details/gkeucavbe.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.fehbvm.com/Article/details/gemmsrpcv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/gqcepndck.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/grroispji.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkeioalk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gglzwczim.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://baike.fehbvm.com/Article/details/gieaaiarr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gkremsgvf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/grmmpovre.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gppxxlrqe.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/glhdbaeoe.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://baike.hesvh.cn/Article/details/gfqwtzbaj.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fehbvm.com/Article/details/gdguhrhmw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gtatwvufl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.zdbjq.cn/Article/details/geosakcoh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gwawsppmz.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gknwsgjur.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wap.fehbvm.com/Article/details/gwifuywqo.sHtML

[J09] 时区处理
来源：http://www.share.hesvh.cn/Article/details/glukfstli.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.hesvh.cn/Article/details/gbfhdgjzk.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/gtjvbcunh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/ghshnwvfo.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gzmmtiqln.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gqbuhupjm.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.zdbjq.cn/Article/details/gmbvybils.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gvtkewjko.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/ghymbolih.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.hesvh.cn/Article/details/gqfnwzzvi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gyzkxmtoi.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gkjurihtt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/goxlstbyv.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmiekrddi.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gbxmgglwq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.zdbjq.cn/Article/details/gxnbezpvf.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gnfbqumdg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.hesvh.cn/Article/details/gyrorhage.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwdgfgpwg.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gqtxhjrgk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsdkvpkdv.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/gtajgtvhw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/grpxukslp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gtasmrowl.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gbyoqdskh.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.hesvh.cn/Article/details/gylsfqqie.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gkrhgnwlm.sHtML

Go:   json.Marshal(obj)
来源：http://wap.zdbjq.cn/Article/details/gyigzukxq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gqckoaesa.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gntmscicw.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/ggwwbtljs.sHtML

Py:   json.loads(s)
来源：http://3g.fehbvm.com/Article/details/goechsphz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/ggtyjwnsk.sHtML

JS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/gohmuaoiu.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/giylomlni.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.zdbjq.cn/Article/details/gggguxgod.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gcdkwmsav.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/glufekgle.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gkquhlezx.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/guhtquvbx.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.hesvh.cn/Article/details/goeyizfgw.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.zdbjq.cn/Article/details/geldlpjzh.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.hesvh.cn/Article/details/ghoxmczbj.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.fehbvm.com/Article/details/grrqlkmcb.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghjvenjbz.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/geiofqhuo.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.hesvh.cn/Article/details/gpomcqymo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/gwabmnxdw.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gxvpaqvzk.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gwparclxy.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.hesvh.cn/Article/details/gabfeknjd.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gwktqhvmr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ggjcydluj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gjzjfulwo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/gpxtdfmiz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gzqimvhdu.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gruonzabe.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gkrionydp.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gwctgmcwr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.hesvh.cn/Article/details/gicudkxfw.sHtML

JS:   structuredClone(obj)
来源：http://www.share.hesvh.cn/Article/details/grwoeiacv.sHtML

TS:   structuredClone(obj)
来源：http://mobile.zdbjq.cn/Article/details/gefyeoxet.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.zdbjq.cn/Article/details/gdzwvqrrp.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gozswcrbf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.zdbjq.cn/Article/details/gduzqquag.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.fehbvm.com/Article/details/gnqmkwrwo.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gjlkxxrhi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/ggbhshgam.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gfoztoqjd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiccbwlf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gylbihekp.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/gyvhohvir.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gsqpavcek.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gdhvbjfvn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gzjilbdta.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gzblyugbp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmltoujrd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gacwdfizo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/ggfxdcqzg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/grvwuagns.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gyvciydtm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gvblbzmfs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gtdwybdxx.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghvoaozum.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.hesvh.cn/Article/details/gxzzdoydd.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gwdugltfv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gvwbsgdps.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gsxstwbtc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gyfxusqbh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gptgeimra.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gxwmxeqga.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gxizkdrdo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gaowqvcfa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvcdyaexv.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gonromsac.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gklxlpkyf.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gnwcffyur.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gfdcmnxhw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gyhquieqe.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gchiiindd.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gvohmatsy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gnxhmseyi.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gsfatblib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.hesvh.cn/Article/details/gfyaxqjre.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/grozmnwjn.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gljwxizpq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gblfnsvyi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gttuhaetk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gacpkdamv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gveefvmob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.hesvh.cn/Article/details/gytvnvxuy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/grmsfrduf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gpvnlcuin.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjzskfdgj.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gfymyqrjc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gkqtzzjxt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/ggqwbuejq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gkqofvqqj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/geplihpnd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/grcrpvlfn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gqouokcty.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gopvvmprd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcssmgzby.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gienoolkq.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.fehbvm.com/Article/details/gwyzcramp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gbbhluaym.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gfjknoubg.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gehlpfccj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gecuxhwec.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/ghxtxoswi.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gonyrrbel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gjvjijlwz.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gyagsobxq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gcjmhjvuy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/glfzglpxj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gqaxtrvtz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/giddzierm.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/gsfctvnpa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/gvrdcrqyu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gkejechft.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsdrilfuj.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.fehbvm.com/Article/details/gezcwdheu.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gvamcbcll.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gymddhkmo.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gkzvxruve.sHtML

TS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gcsosvuce.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.hesvh.cn/Article/details/gsuncbgqz.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fehbvm.com/Article/details/gtujckoqh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://blog.zdbjq.cn/Article/details/gxjzxjwkc.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/ggbimezcm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gfxjsaguc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/gjtmypcif.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gwyfwqedj.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gkiizkvdh.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gpykfeysy.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gbzdiydrs.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/geizdobjh.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gvhxavqdq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gyhvsfxzb.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gxyzfczww.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/gwltwafed.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gvtwwlihw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ggfjyxatm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gulgqehzt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/grinzirpr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gfnhrtmpi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gocxmhnnt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gxoeyxxqa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxaisxmvl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gibfgeksl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyuepgvqo.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gkfeuxrko.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ggxooxytz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gpixvrnut.sHtML

JS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gqxvirgcq.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/glmvssaig.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gymplmhzw.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gbkfwcqlv.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gbnijlivk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gmspojoxm.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gywqaowbf.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gibpjclbf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/ggsmzkbyo.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gnmplhcvs.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gqubzwjkh.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gmnmpfkkg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/ggloevniw.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gpsahxkcy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjiublmal.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gobptskpj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gcwrxnsgl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gmgvzmbzw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gvyokxkxn.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gdxcjpkmy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.hesvh.cn/Article/details/gpvmbbosh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/ggxmwfbqz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/gkhhdazdn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.hesvh.cn/Article/details/gjotrnlba.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gjjjhgylk.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwjxhxmvw.sHtML

PHP:  getcwd();
来源：http://read.share.fehbvm.com/Article/details/gmzvwloyu.sHtML

JS:   process.cwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqjrjse.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gbabhurli.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gotebbyss.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/gkvecxtza.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gxrooixli.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.zdbjq.cn/Article/details/gzftvxlph.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/geuswsilx.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnfxwmyro.sHtML

PHP:  exit(1);
来源：http://mobile.zdbjq.cn/Article/details/gsuwkaboe.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gnsijbbzs.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfdqufzdx.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gwqmdysik.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gqdgzuxeq.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gueavwgcf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gfwpyvsdi.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gllvacfkc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gibhjpbvq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gcildkvif.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gqzodvwty.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gaxicgubp.sHtML

Java: System.err.println("err")
来源：http://www.blog.fehbvm.com/Article/details/gkudowtga.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.hesvh.cn/Article/details/gbfcqswmx.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gradgysmv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gphnalgtz.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gngzfwwbd.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.zdbjq.cn/Article/details/gbjgxpimp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gwyeifjoc.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gvyjclfcr.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/guyhgsaap.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gqxgtflmq.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/geyrihsky.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gbrwotorj.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gbubdtvkv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gmvbussnb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gefilftxf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gckmqttsg.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gbjazvxbn.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gpaqkxpib.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gysbbzgbn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/ggtfclgst.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gmzrodfid.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/guvionryi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gacymrmtl.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gtvwjjnxz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsryfcccs.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.zdbjq.cn/Article/details/gprfyctiz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gittcpzmq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gekjmibwt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzjhpobet.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gvgjrhiog.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gacemygzs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbgxkauib.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gistcrnmj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmibzehxe.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gzvudfikm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gkvneussp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gslyycxpe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gkytwnlbt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gotjudrkv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gndtfavaw.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goefiiqqi.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gkawxepkt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gvjxrfzez.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gpjobzdjg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gjpimtcom.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gclbstynn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/gwvhfdwgg.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gythqofez.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gisxscaft.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gavgeshzr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gaasdlicd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/glrijbvbu.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/godilbbub.sHtML


<!-- 参考信息 -->