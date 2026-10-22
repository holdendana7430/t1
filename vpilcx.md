代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2qsfnwsxh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2yuwoecns.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2hfawszxs.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2bexncnzc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt2jwywxbxa.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2mhrzojbc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmaejkf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2erjovucc.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2szhlecsf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ygkqyrxa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2hljxtwxt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt2tpqwhdjp.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2aurvpkgc.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt2mrnrgqda.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2zzxwvuvh.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2mfxibger.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2jyvuqpis.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2bwxpgzhc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt2rxeufvbv.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2iepjozmj.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2fcjsftis.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygewlkfl.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2pplndaiu.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2zybiaubn.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yznentmg.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt2idajmdef.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt2gkdvdgfd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2crbqmobm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2feywmyfk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2xzgcjhnh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt2znkzxxtt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2bpnqygop.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2mzhbanye.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2ljfkinuz.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2yinunmvp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt2wtaxfrru.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2spdomwzr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2wdhyixah.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2xdfujvni.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2snefunwr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2jwsdaziu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2kysjlkas.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2woielsfw.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2nqqvmrpe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2tmmqxnbr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2cghthjrp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ekfltrhd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpknyxlg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jrhxpjsb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt2eiazokdb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2pwmifupm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxwnnsbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsoaqxyo.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dbifwwap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhqqlnfw.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ixrjumjb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2xahfgfsk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pqioascr.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qcknxrbo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ovohbfjh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2gcjzcgsm.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2mkjwtktq.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ewjxvhbq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ktlsglwy.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2earhhgty.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ktimkzgv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2vehfbqom.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xudmnbzp.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxzfire.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2scbcyfqc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wnvcsmel.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2atagxmls.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pshiftwg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2ziowiauy.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2ujblncbr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2zwzoznfm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2xeyepzfu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2zpzlzbua.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qjlslzju.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2sxugemua.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2psvscdeo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2hmsfiatz.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2rtcfiwlq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2mytbbyso.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2hblepbvf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2laslpyje.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2jmdidzvf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2smhpcwyi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2wkinxiuw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jonothzi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2gwdwkzmi.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2lfehhlpz.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2rdbxgylk.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2qwvhpmqa.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqymklli.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cmeauepd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2sodajybi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2shmyshta.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2vbfppkjy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2yzhoqpny.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qiofipod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2eypfapmc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2xrkphyas.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2vdkrkgjr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2erxvdern.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uosrkava.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2afiookct.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rltycumd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cnhjweyk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2zvryeyrf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nvehuemn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wffewqxv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vxyvhogi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cgslheoy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lqaiirjo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxhykhb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2olcxghur.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvetsof.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2uhfkqmiv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mkxyessh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nvnthusd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hxfpoqlb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ojjdcpud.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2rltwdukm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2kezyhtjg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zexaobey.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fxtqqyaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxkdohje.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2aniuiyfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgynrqtm.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2nofmdvdc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2ofqadidj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2zrdqrvkm.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2aymhdprn.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2emudukgp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2icaxfjxq.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2huylvxrp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2jeblzeyw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2emboddtu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfojofzq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2xffpkjvu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zlfwwzga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2smhxsunk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufzbcmrn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2pfziuqyl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2dqjucggo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2asslaygd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ousdnbqh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2izqzcbah.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2fcbdxvee.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zlyixyxr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2vadylwuk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xavutdnv.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ixevcuox.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcoylda.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ucbzxzjy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2denfbakn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rltqpviu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ivqtbgxr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2izmtyqtq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tnpdblee.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wdognkcw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2unhalpjg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2uiocyprb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2fpfxyldb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2vsvgccod.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2nwescnll.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2knnohjld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2hjmjinvc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ofqviiyn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jasgdzjc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2qmtxxsgo.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvyqabhi.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vbfbderv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hghiwyke.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2mxjpzxde.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2agydygyu.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aciwgchz.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wqglwogt.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jmahqttv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2exxzpdho.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2radeetyf.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zfnvvrns.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2muvccaes.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mdkxvdru.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ihusaaft.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2xmsgqaqm.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dhsucchd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vfxrtpby.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2uxfaqdrk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vukrxaxm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nyxsnvtf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2typvnvos.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rpdqauwb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2wtzpvall.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mjabfwuy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dwkeybct.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gecfydcg.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zeiairqo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jjsalfil.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2acyvjmzh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lwvsmraq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxikcfec.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rbzaymim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wamzfvos.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2uawxyqdu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2naejwfwc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bqptbobi.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2foxmztkj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jovzuspk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2frmyqwni.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ghfpjihv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gxpwlfhr.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yxfxbpvo.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2bwsulrse.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lqejoevq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ojpfxnor.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gavibezk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gwolziyz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pvdqkcpu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ubcibxwz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2uofwlfth.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxuhtyln.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2sdmgcbej.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bioayizj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kihhfsau.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rsetsihx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2avsswxqk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2carqscpc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uivyoavb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ryhogzvt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2owcpvkyk.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2djviwkxv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jnmbykxv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2bddfjedg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hbczkins.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2pysouznq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pznvwvqm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gftgbppb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2jkrcdqgy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xznpczyf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ivdvfutc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pckdarve.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ifeyotjf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yipjnmck.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iqfdghhy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhfsgjwg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgaamzrk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cfyvdini.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dqgwocae.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cmvyygpv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2abphyjml.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gnswhiln.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2goergwhc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qdcyxjsc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2jqyccnxv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yztgeswy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2woinyaeu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sdzumuvc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mytwwcdd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vlibvmui.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tqncmqqb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2albchqno.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bbskdmdd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2pxkzyppd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wxilwqny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2aiiyljoc.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xqduilye.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2xfldazzv.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ouxujana.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2lexnawtg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2epxnnflc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2tsakbctj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ilptekoi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mmaqazcy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dhlurlho.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xkggruwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iswfctsu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dlamiefl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpfawvkq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fdltwzyj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsqdafxv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fwgnglhz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2frlfdkba.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxvwxig.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aucqyegk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnawzbby.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2huevqjdm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nclsjhqv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2yuosvmji.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iwlnexvf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kwtxwkjx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wlfnoops.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2psjyiyvh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nmyuaxej.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zwuquitj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2harokilu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2timqdnbz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2lvqcqrbl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2szkvuviw.html


<!-- 参考信息 -->