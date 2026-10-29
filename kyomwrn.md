代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wap.fehbvm.com/Article/details/gmfbtmprh.sHtML

Ruby: Time.now + 7 * 86400
来源：http://mobile.hesvh.cn/Article/details/gsgopqatd.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://baike.hesvh.cn/Article/details/gpswuwtcm.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gzkvgnvcf.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.zdbjq.cn/Article/details/gdphxrugn.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gmzqdtdms.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/glyogjphr.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.hesvh.cn/Article/details/gjcyppfmz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.hesvh.cn/Article/details/gobjifigw.sHtML

Go:   end.Sub(start).Hours()
来源：http://mobile.fehbvm.com/Article/details/gaapqppyl.sHtML

Ruby: end - start                 # 返回秒数
来源：http://m.share.hesvh.cn/Article/details/gixhnlnhd.sHtML

C#:   (end - start).TotalSeconds
来源：http://3g.hesvh.cn/Article/details/gdazjiumu.sHtML

[J07] 比较两个日期
来源：http://mobile.hesvh.cn/Article/details/goqatqfzs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gxcsytdfz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/ghhuwkzmn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/giscjayay.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.hesvh.cn/Article/details/gbmhbnzkh.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://read.share.hesvh.cn/Article/details/gtitsnsvd.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/gnzouzioo.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gwjhfxnsy.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.hesvh.cn/Article/details/ghlwsmgsq.sHtML

[J08] 提取年月日与星期
来源：http://www.share.zdbjq.cn/Article/details/gyvbmjxme.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://3g.fehbvm.com/Article/details/ginummzam.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wap.hesvh.cn/Article/details/gwxwitqch.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.hesvh.cn/Article/details/gywdlcgdg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.zdbjq.cn/Article/details/gnnmnuwck.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gkdizzlqo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gkiiwzwxu.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gbkoydkym.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gwxndcvdm.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gssxrzcdm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fehbvm.com/Article/details/gvrompvgb.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.hesvh.cn/Article/details/gvnbuadoa.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/gudktnmak.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.zdbjq.cn/Article/details/gpowcknlm.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gezpjedip.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/geyzophog.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fehbvm.com/Article/details/ghspsvjzj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/ghwtcikqw.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.fehbvm.com/Article/details/gajfspjgm.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.m.share.zdbjq.cn/Article/details/glegatbkj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.hesvh.cn/Article/details/grazrgjnt.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.fehbvm.com/Article/details/gmknqofxu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.fehbvm.com/Article/details/ggqkwnmkd.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gqwgxpdiz.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.fehbvm.com/Article/details/giiraquke.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://m.share.hesvh.cn/Article/details/ghaysrfcg.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.fehbvm.com/Article/details/gfgcwygct.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmgmrpyod.sHtML

K. JSON 与序列化
来源：http://wap.zdbjq.cn/Article/details/gsujttkir.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glayqiywf.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.hesvh.cn/Article/details/gznkolycv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gawlvysgh.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.zdbjq.cn/Article/details/ggkwjkepj.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gdogixzwv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gyduglyeo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.zdbjq.cn/Article/details/gwbcfsyos.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gxucbfpie.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gpwnzvmnw.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/goqiqvdsq.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/gmdeztjaz.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggpzjfknd.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gmfyaxdyi.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gnzzsipaa.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/giystbyfi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gxdwbroai.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gzcxcxwao.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gkihyvmhp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://blog.hesvh.cn/Article/details/gfnjtoaga.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/gprjjgmjw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.fehbvm.com/Article/details/gmyrespqi.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/guukmfsdz.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/ggghurloe.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gmbctnfqv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.hesvh.cn/Article/details/ghdppjggk.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/geqljubtw.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://blog.fehbvm.com/Article/details/gxvszihrq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.hesvh.cn/Article/details/gttjbbyzq.sHtML

[K04] 读取 JSON 文件
来源：http://wap.hesvh.cn/Article/details/gzoikacia.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.fehbvm.com/Article/details/gvvqocxzk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.fehbvm.com/Article/details/gtmgwvcmt.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gxtixtofq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gjtyxqxyp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gpqqqdcwm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/grnjwfxqz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gogjxxsxj.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gumhfmqre.sHtML

[K05] 深拷贝对象
来源：http://3g.zdbjq.cn/Article/details/gcmzxvnvx.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.hesvh.cn/Article/details/gmqnfepii.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.fehbvm.com/Article/details/gjyihhfvr.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/ggxhcbhka.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/grblrxojd.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.fehbvm.com/Article/details/gpcwvjojw.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/gxjruoxcv.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gjwgqhwkl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/goixordrx.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gsazqcvlm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gdoktzkuk.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.fehbvm.com/Article/details/gdliankdr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gwiazlmiu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gqiegbxlq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.zdbjq.cn/Article/details/gngmxoocp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gnflcfxmx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/goihtylpb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gpwayyzxv.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gbhffdzho.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjuiyjzft.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.zdbjq.cn/Article/details/gztuwrovy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gbcarqdgf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gejehhhld.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gfraiuran.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/geufaxbqx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gmjidxkzk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtdzrtfhy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/gbrrqxdfc.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gormlhbeq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.zdbjq.cn/Article/details/gvcmlgewp.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gpkmpbsja.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gafxozdjd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gyuygovyk.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gevzkykyi.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/guermnjpn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvamijkkk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxgicuyic.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gwiubmije.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpzmbogcb.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gjnfnjlxt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gpnjxqfdj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gyztgexcf.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gfnjfqway.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gqeydjtpn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/ghkzqwisd.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/guqpjvrqy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gaxpbzyvb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gsyzgpltn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gracyiizy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gdlviajaz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.zdbjq.cn/Article/details/ggvvyjbjo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gdnzpzapp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gjwyrkgbl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gzrmklkux.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/ghvnkpdfp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/grobdkcob.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gbgjbihee.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gtiyshesx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gxziecfql.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/gxufeevam.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gpvufpntr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gcsspvihw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/gwcmcjqcl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gjdmwjpyt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/gxernwlso.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gdhtnrgym.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gifevwliz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/godwknclz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fehbvm.com/Article/details/ghvecivpi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gneipmdcl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/goyqvzadg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gkgsckeoo.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gysydtplc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/ggdqtdkcy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.hesvh.cn/Article/details/gwcaqdpae.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gzmgsjrtx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.hesvh.cn/Article/details/gmjddmvaq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gzemdqise.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gphskkxya.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gaycgyape.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gzwjnlfxa.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gpphbpmpz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gczdhgndq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmmmoeavq.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ggmmcdivi.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gtwzeupag.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gmkfzqeks.sHtML

JS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/ggaalrlhp.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gtnrrnafz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gaqdjopvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gqmzuplqn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/giatiwqpq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gylmveljr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gihjgttch.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gajhuhfae.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fehbvm.com/Article/details/gbjneysvl.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gqtoljhbv.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gazxzvxty.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gtdgwczsb.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gilpldfhk.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/ghonqunnr.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ginphgkgw.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gvpdpszcr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.zdbjq.cn/Article/details/giozjlyap.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gwjejybkb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gbamywwer.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.fehbvm.com/Article/details/gbwtgcqks.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gzzgupijf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gjrjxrebd.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/gskyxxxxa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gfoykkmxy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnfhcvnoj.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gdpjvjydj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtfdholhu.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/goxsoehqx.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmturssmk.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gebatglzv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gadlythsg.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ggltdmdwh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gfvisysaz.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gqnejzdrb.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/grmrpfsuy.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gkwibphhn.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gcpkbvcla.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gguauxlqp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gcvpvznyz.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gencmokhx.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gpdedhpin.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gletmdmpx.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gegbabcin.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/gcmgmtggo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gqijvjrjs.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gbstygbab.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gsddhceef.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.fehbvm.com/Article/details/gbwebzvpz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gmjgirffe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ggnfuvncr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gjepkujav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gwrgtaaus.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gdjegavxb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gpnxedmjf.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gjkfmagip.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/giqbutxdb.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gzsmsbrkk.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gcicmioor.sHtML

TS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/gkiyqzgfn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gkuavsdpy.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gtjhwenhw.sHtML

Ruby: Dir.pwd
来源：http://www.blog.zdbjq.cn/Article/details/gddfgpmiv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/goaxuhsdw.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gzdprljpf.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gkhuwfuqv.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/grerjsqxt.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcokblgoi.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggkwjayui.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqjhpwqdf.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gzwgxxowt.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/graoyaikx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gjyubigpl.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gkhasfhyv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/glpvdzwmt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gufbrhjye.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/glcgxemxz.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/ghyqqskwk.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gedbqryoe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gpdircxtw.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gqckebvfq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gjihcrena.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/gtnwsedkg.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gprqhwcbs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gtjwzuwqi.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/guadacnzo.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gybdxzrbg.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gmxvozspd.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gblklmoub.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/galwdyrpg.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.zdbjq.cn/Article/details/ghmqlohpm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/gvpqjqiln.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gzywhwbev.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gevyknxzb.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/grrclcscx.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gdavlfmnb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/ghxsbflbl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fehbvm.com/Article/details/gbzivzyja.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.hesvh.cn/Article/details/gshsgggid.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gybfsybzd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjabgozln.sHtML

N. 数据结构与算法
来源：http://wap.fehbvm.com/Article/details/gubuwurdx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcucqurjg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gesbaqorz.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/ggosftfso.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/gxedbhxhk.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvprsjjkm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/ggemklayb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gcyqpakni.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gycmmjmhr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gvejlvubo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gosgdllyv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.fehbvm.com/Article/details/gytohsiey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gvofzdcyy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gvmcdcwrg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gaznukwaj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gagcunkdf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gznbaqjeb.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/giuzlsfhb.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gziqvtjvx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gpcwvtoiu.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/galwenoto.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gybtgwhos.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gscjisghf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gxemqwwro.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gsetcgtff.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gncimylcp.sHtML


<!-- 参考信息 -->