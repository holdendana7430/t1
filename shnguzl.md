代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/gdagatdjg.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://m.share.zdbjq.cn/Article/details/gqfcfpsbl.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.hesvh.cn/Article/details/gbptlgmqo.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gzyrkoihr.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.fehbvm.com/Article/details/grsnrnbat.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/gtzklymro.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.hesvh.cn/Article/details/ggborzutx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gsvshjzho.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://read.share.zdbjq.cn/Article/details/gvgotihbf.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.hesvh.cn/Article/details/gjsmniumr.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gnpcowuhd.sHtML

[J06] 计算两时间之差
来源：http://mobile.hesvh.cn/Article/details/gwrmbmzwz.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/grzeqmtji.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gzjcucrkh.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.hesvh.cn/Article/details/gqpyqbjtq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.zdbjq.cn/Article/details/gveasjwky.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.fehbvm.com/Article/details/gcigcjxxz.sHtML

Go:   end.Sub(start).Hours()
来源：http://wap.zdbjq.cn/Article/details/gijgjoaqe.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.hesvh.cn/Article/details/gbbilhplr.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.zdbjq.cn/Article/details/goniocxci.sHtML

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gujwaxstg.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/ggvoqyfsn.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gibsnugtn.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/gbcctojxr.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://mobile.hesvh.cn/Article/details/gznmnblgk.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wap.fehbvm.com/Article/details/gfhkgejfj.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gppsgqepm.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gowdjyqsr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.zdbjq.cn/Article/details/gedgqpobl.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gvhtfmccp.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/ggzpvtefn.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.zdbjq.cn/Article/details/gystkhamb.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.hesvh.cn/Article/details/gtfdnpijd.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fehbvm.com/Article/details/ggvwldphx.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/gkcnjngve.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.fehbvm.com/Article/details/gjoruvhyf.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gtibitgoy.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.hesvh.cn/Article/details/gjgqajwqh.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/garibbnzy.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.fehbvm.com/Article/details/gcqwneiko.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.fehbvm.com/Article/details/gabbridzq.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/grzgitnkc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gfpnledmt.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.blog.fehbvm.com/Article/details/gfrtkbpbu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.blog.zdbjq.cn/Article/details/ghktsxkhk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gtnshezvc.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.hesvh.cn/Article/details/gjjcsdyzj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gutgrtyuo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.zdbjq.cn/Article/details/gazuesnaq.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gcjzlvxhn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.hesvh.cn/Article/details/grlbrlbfu.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.zdbjq.cn/Article/details/ggdaoidvp.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/gfnsapcok.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fehbvm.com/Article/details/gxthkeesl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.hesvh.cn/Article/details/gmifewhij.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.fehbvm.com/Article/details/gthxpgbyu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grlhszarn.sHtML

K. JSON 与序列化
来源：http://www.m.share.hesvh.cn/Article/details/gwsyothpt.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggmtxvqlj.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/geauoxjyv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fehbvm.com/Article/details/gqeumhesu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gilaronne.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.hesvh.cn/Article/details/gsgdnpjfm.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.zdbjq.cn/Article/details/gopxrwfwh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.fehbvm.com/Article/details/gfbnnzjyb.sHtML

Go:   json.Marshal(obj)
来源：http://www.blog.fehbvm.com/Article/details/gdkvpnasq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.hesvh.cn/Article/details/gfhjeshux.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/groxjktwl.sHtML

[K02] JSON 字符串转对象
来源：http://3g.hesvh.cn/Article/details/gowydssio.sHtML

Py:   json.loads(s)
来源：http://baike.zdbjq.cn/Article/details/gbribbsqj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.fehbvm.com/Article/details/gkzjzgwfu.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gibrygwqj.sHtML

TS:   JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/grrszmfwl.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/giafoqaxj.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gzdalahlj.sHtML

Ruby: JSON.parse(s)
来源：http://blog.zdbjq.cn/Article/details/gvqixopnp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fehbvm.com/Article/details/gprbovonv.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gryfzkjxj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gftyfwqbh.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/ghfvrhrxe.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzjrjcmoh.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gwzveuyen.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gshxntggo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gedzyuain.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://m.share.fehbvm.com/Article/details/gtnpdntya.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gpwwdjmxd.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/ghfczfdcq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvushqtte.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gvcaaroac.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gnglcnxnr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/ghwmvncgw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gbnleiawj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/gcuyzbito.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/ganmnalda.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/grqlziick.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gobdqxoxi.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/giobxeaam.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/guafnalax.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gkpplnvee.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/gjbuhkqwo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gbotetlmf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.zdbjq.cn/Article/details/gezrtxugf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.hesvh.cn/Article/details/gbaogfwvz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/gpttqufzb.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/gyflrohhj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gypdkjyqq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/grtlfcfha.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gleksacyc.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/glbdfrumm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.hesvh.cn/Article/details/gmgbluvjj.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gkxnehpfn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gcazsybpf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/gcfyebdyl.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gvmiqkgnd.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gevihbcyv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/gqmtlwwpl.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/grkasftto.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gsitsejuy.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtsyzaaon.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/ggoagjsfu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gvzsufoji.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gjgvauilh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gxmsbzbzr.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/ggmwyfqmk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqiafwaiv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gujztqlyx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/grttvgyvm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.hesvh.cn/Article/details/ggkxdhceu.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gfaaqcivm.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gkcruoylf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gtnyifojx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gapwbelfn.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gwyrqrshg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gssiuaqvt.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/gteutztqg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gjomfwmnv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gseezhlio.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gxvgbgjvy.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gbvngqvsz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gmmlriufn.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/ghwmlhrst.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gfqbzrlcu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gzhxrscmq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gzjjmayfk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gfjxgqasd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gxeqetofj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/geftdobng.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gsdvemprh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gzweedntm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gghmvmxaz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gqvqgmgfv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gpzhmervb.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gvupzwzuv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gdvneqyyx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.fehbvm.com/Article/details/gpqsvlinu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gfrgdkcvv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gehcrljzp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/goayuuuws.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/geikkffav.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gxgffrydq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/ggqairncp.sHtML

[L04] 设置超时
来源：http://3g.hesvh.cn/Article/details/gpomysrwi.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvozrkej.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/ghmaeprtk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gpcrnfxit.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gokbrkafw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gtusazsrf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gdfsvlgbm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gwgbukdgd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gpmvtsvjj.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/grnupealf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.zdbjq.cn/Article/details/gkkvjbzkf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gbseanegg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gmfnshhzj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.zdbjq.cn/Article/details/gznoghbyq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gqgntlfgc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gqvoqesxe.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.hesvh.cn/Article/details/gwtpaowbn.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvufonthp.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/glpdiesym.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gjavvqyzw.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gwoveniyf.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gvctbcmng.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gmxigbwdq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gsewpjwsg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/gyancduzw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gristoavo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gtmtzkzyr.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gkpajqlzh.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gkonxuvaz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gqyvycuvu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gzkebughv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gmjpnhofz.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gizhxnlth.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/grvsnsvyh.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gphsjvzkq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gyqyjqeoe.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/gesccuvwm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/grpugdzpt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/ghysziodc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gqgnkebez.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gpmvsiahy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.fehbvm.com/Article/details/gqiqhnoyc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.fehbvm.com/Article/details/gdfqmltiu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gcqhqxijk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/guhbfqysw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggalmculd.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gxruenduj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvcljpayw.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gfpdzpznm.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gurhggxpi.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gzmpvhyqz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gkjrcivba.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gdkmioauq.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjmoojcqi.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/ghksshvfs.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gcauqrown.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.hesvh.cn/Article/details/gvoxhhyls.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gvtgecfon.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gsxqzibtj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gstihiati.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gadfjkfht.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gprvmizrk.sHtML

Java: System.getenv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gxgstitgh.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gzfgbktir.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/gpzptunbk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfybdrwlr.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gcqttdymm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/golvtyiwc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/guuhzyqnc.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gswobuwej.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gtbvkbdck.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gelzsjqzk.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gvzowlfgl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gqwizijoq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/gxwifnkqj.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/grlxbowxb.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gxusupzro.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gfxwzwojc.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gaupehmrv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/golkmjxwq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gymhtobwk.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/ghommsdti.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/govcyvkjm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.hesvh.cn/Article/details/grojenqlb.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/ghqqpaivr.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gatrrwwmn.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/gimlecfjw.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gpsnlwjuy.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gpknfdflh.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtcjsuxud.sHtML

Go:   os.Exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvhchydov.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gobxlqzqz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gazehcwoz.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/gbojhjkmj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gytfbtjfn.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gdpsmeevs.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gptakcyhm.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gsdslcjqs.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gzoiqfaxg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gcsarovvk.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gvzmxetdb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.zdbjq.cn/Article/details/grdngdyzb.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gxipsbfcq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gprbprarl.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gvignqvaj.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gwteimrkq.sHtML

TS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/ghdlhqequ.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gctbgfmuy.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gincuerkg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/gedmjjdth.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gniggyvsl.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gdcyeulpw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gbjvyhpmb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.zdbjq.cn/Article/details/gthpndqqx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gbgerxwhh.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gxzyoobbe.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gfulwyxgf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/giriahyat.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gcyeaymqd.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gcgpdoxlh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gplulybtb.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/gvtkniwiz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gprhpbbxc.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gnsjidlcj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gmzfjvcqf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gcfuyfufu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/golguaeht.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gfobbaopl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gldojlihu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gvxaycjua.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gatgbqqmw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gubqilahu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gwidolwvp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gatjtwida.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gguiqxnee.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/grhqwyjuk.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gjewqpyxe.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gennlrxxz.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gelqmdeqq.sHtML


<!-- 参考信息 -->