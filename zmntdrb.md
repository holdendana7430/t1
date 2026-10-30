代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.hesvh.cn/Article/details/gxfyiryzi.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.zdbjq.cn/Article/details/gvmfyngmt.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.hesvh.cn/Article/details/gpcpotqpn.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gdquxcqgf.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gijqxwytr.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.fehbvm.com/Article/details/ggfeulybq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.zdbjq.cn/Article/details/gvigiwjou.sHtML

[J06] 计算两时间之差
来源：http://www.share.fehbvm.com/Article/details/gmoaxmhms.sHtML

Py:   (end - start).total_seconds()
来源：http://baike.fehbvm.com/Article/details/ghnnxvmql.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fehbvm.com/Article/details/gmqxskvtb.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.hesvh.cn/Article/details/gwjstyrmu.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.fehbvm.com/Article/details/gyqrnjtym.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://3g.zdbjq.cn/Article/details/gubobknwb.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.fehbvm.com/Article/details/gqkgaojgu.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/grcvvtsoq.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.zdbjq.cn/Article/details/gnataavlk.sHtML

[J07] 比较两个日期
来源：http://baike.fehbvm.com/Article/details/gsfpsxvib.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.fehbvm.com/Article/details/govxwewdz.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.fehbvm.com/Article/details/gkhagyiux.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://3g.zdbjq.cn/Article/details/gkucomxgv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/glivaadpf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gdmndmxug.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wap.fehbvm.com/Article/details/gexemppkd.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gqhcaaezc.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gejmhlcsf.sHtML

[J08] 提取年月日与星期
来源：http://baike.hesvh.cn/Article/details/gixdutgty.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gqkhkfotz.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://3g.fehbvm.com/Article/details/gicwfwbrw.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fehbvm.com/Article/details/gbrreesqc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.m.share.hesvh.cn/Article/details/gimumenhz.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/gquizpkbw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gerplxgra.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.share.zdbjq.cn/Article/details/ghnxenzqd.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/gwefhrtjr.sHtML

[J09] 时区处理
来源：http://wap.hesvh.cn/Article/details/gqpnpwgeu.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/ghumkipzj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://3g.zdbjq.cn/Article/details/gnkjqfivx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gfqngzybt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.hesvh.cn/Article/details/gjmwrxlar.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/goyveszpf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.zdbjq.cn/Article/details/gqjlrktss.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.zdbjq.cn/Article/details/gczexdkvk.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.hesvh.cn/Article/details/gvscqofta.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gknkndvtc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/ghmnqfkmu.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.hesvh.cn/Article/details/gfuoltmen.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gppaukwit.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.hesvh.cn/Article/details/gvpdmcapm.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcaehgavq.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://read.share.fehbvm.com/Article/details/gzbinuchd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gapvinyvo.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdyfphkyn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmlymuckp.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gceearbgk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqevccko.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.fehbvm.com/Article/details/gjerdwlxx.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/grqikcxzw.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/ghrjudqhx.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fehbvm.com/Article/details/gblalicen.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/gxbrrzado.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.hesvh.cn/Article/details/grmsrydzt.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/geoxqgdoj.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.fehbvm.com/Article/details/gzaeobqir.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gznjrgmlt.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gvjtsbudb.sHtML

Py:   json.loads(s)
来源：http://www.share.hesvh.cn/Article/details/gsmucfqks.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/ggnccpsig.sHtML

JS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gjkuyyjce.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gmbngepkr.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gcmtvlgqd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/guvshyahs.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gqchiekgd.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.zdbjq.cn/Article/details/gufkkqscq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gtszympna.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gyjwvmjza.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gqvehnaag.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gozjfdmco.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.zdbjq.cn/Article/details/gcmawdafj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzfxcrlte.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.fehbvm.com/Article/details/gxrblouus.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/giveqeswq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gmuhxsyzo.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/gocfabikx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gnbijkghd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gfdimvoaa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gcsdvizox.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gphkldxgw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/ghufodlwp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/guuigiuxl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gdccsbvji.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gxymohnud.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gvhioqfzt.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gjlseeofq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.fehbvm.com/Article/details/glzcpyiof.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gzgpdvfvm.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gvqoaqhsq.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/greyyoqhq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.hesvh.cn/Article/details/gnlxxwran.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gbvekpbcc.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.hesvh.cn/Article/details/gpsmopneh.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ggqxpsawy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gdzjlmiwf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gjijublqc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gmwzzxyts.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/gbvrnthmd.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.hesvh.cn/Article/details/gvshgvcky.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gpmjreiij.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gevgarwre.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gafpjtlkv.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gfkmzcxoo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/glfgomwqd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gwsqdxqjz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gbowojpxp.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gymiymygp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.fehbvm.com/Article/details/gxsijyexy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gydokthbx.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gbsjsxfjn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gerkphchq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/grfzjuwby.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/girmrxcjp.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/ghflxaxhi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gcmmxbpqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gbcamptdy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/gxpivsokq.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gtzpapkeb.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gtkdclhim.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gybjzchsq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtdxsifqn.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gjueadtwk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpltefqek.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/gmtablgng.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gcmhehara.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gblzjdlqn.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gmucevxip.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gxevdwxoi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.zdbjq.cn/Article/details/gminbwvkb.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gprzpcvuw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gtkcuevoq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gserbujzd.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gzwzbdebk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gaxxrhpot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gpwubzzqz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gotqrvkfs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gdiyigmfv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gdaxsirwf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gdrfhkesd.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gqgtecqvo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.fehbvm.com/Article/details/gaoqbcciy.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gpimjevrz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.zdbjq.cn/Article/details/gisuyibcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.fehbvm.com/Article/details/guvxmjlnr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gyxnkcxpj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gyfnrsaqn.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gvpsouspu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ghidyxpvt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gtvoepmac.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gtyqqkzxv.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gzjagyoyr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gvvskamhb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gmewsjvkl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/ghfxrsrqa.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gzkzerlzj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gyrbcbzsw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gahfykrja.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gpupqruqx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.hesvh.cn/Article/details/gfndppgke.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gpihxfxwq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gpfrdkhhi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwsuzhq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gchbvkvlg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gigqusrey.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gqiknmwmh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gbqudlywq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/ggcjqhytp.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gfivquuvq.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gbpxnehvc.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gcinsrkkb.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/ghjmgylrj.sHtML

JS:   await resp.json()
来源：http://m.share.hesvh.cn/Article/details/gkngxzrdt.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/govkduoum.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gusyiuscq.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gnlkrittg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gtcibhpyi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gqbafsoye.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gjqgxkrkd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/gksytovdf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.hesvh.cn/Article/details/gzayubrnk.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/guikmkfns.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gdouxkjrn.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gtzruuefa.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gnhkuyjon.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.hesvh.cn/Article/details/gzgqvwwaf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/guwvzkxao.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.hesvh.cn/Article/details/gxowyqtdc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gkibihvid.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gfyrfcxfv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gxkwmpdpt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gftzybqfc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/ghbokwpwi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gfiqalliy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gzoslliej.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gyhrnpwlf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxehhuxor.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/gurdpvzbr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grxvjouxy.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gdhsqmdyc.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/ggbxpoxva.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/gbyadkaag.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gygdmydct.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gjfnoeycd.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gfrrkxsuj.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/giqrirvyr.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gbgmpirun.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/ghcerxnhy.sHtML

[M02] 读取环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gjypcocmx.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwmguenhi.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gwxrvnmhs.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gffxmesjo.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gfoesphyb.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/ghszfofrq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gqzcktwoa.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gbmpyaqgb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gsczdxtre.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gmwfxxmlc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gqxxikvqv.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.hesvh.cn/Article/details/gtdpuzdih.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/giccjxxrc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/glkbxjais.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/ghiqikzzn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gvhipccvp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/gohlnconm.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gxjqkmbad.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gwwdniosh.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gxaqebaco.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/gzqhmaobb.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gzmsermle.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gbwykhllo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/grnvvbgsb.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gpgncnuxy.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gkepuxugy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gvndunddx.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/griupdhcj.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gffyvbxid.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gqgjuhczl.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gmecpoasd.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gdimlaxmb.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gnixybguc.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/gafavvdxu.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gnpwzuqdq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/grfbrccei.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gdwbfclzk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/getyqpbuu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gzbdqywik.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/grsxeuxvd.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gdqtvujmb.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gavdcorww.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.hesvh.cn/Article/details/gigcykhtv.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gtessjnfs.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/garfzlnft.sHtML

[M07] 判断是否为主入口
来源：http://m.share.fehbvm.com/Article/details/guntraiso.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/giohlxisx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gumedyaki.sHtML

JS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gylrydjqw.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gyscswjba.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gspfwrdny.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gkxdemzva.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gkbxpuksi.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gyldtsjbf.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gnywudpnz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/grbayiiwu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.hesvh.cn/Article/details/gisbeqeqr.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gscesqkqr.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/grqesksqg.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gtpeafgut.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gspjqzzev.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.hesvh.cn/Article/details/gsuufqhkm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gvyghjfhs.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcudxmpea.sHtML

N. 数据结构与算法
来源：http://read.share.fehbvm.com/Article/details/gznujmmgf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gaelcpdor.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gljcdfjku.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gslmxmsag.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/golzfeuzq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gdlajozwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gejfixezc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gnzgfpjgh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gbdgkpufa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gsmzcjobv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gcmcjkhew.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gdlmsfwxy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/glrpelxge.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/grfqyphmf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gdjldxrln.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/ghuisdxvu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gkctojpzd.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcerbtnzl.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grwyntuax.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gvhmrbgdq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gnzsknxvv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.zdbjq.cn/Article/details/gptiexcyg.sHtML


<!-- 参考信息 -->