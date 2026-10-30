代发 wailian999

Py:   (end - start).total_seconds()
来源：http://wap.fanxiaobao.xyz/Article/details/grpcuiylw.sHtML

PHP:  $end->diff($start)->days;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcyyblku.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdakktfce.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/gmggwnypa.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://baike.fanxiaobao.xyz/Article/details/grjavjtjy.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxesnwnst.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fanxiaobao.xyz/Article/details/gefkgpamd.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsknungko.sHtML

[J07] 比较两个日期
来源：http://baike.fanxiaobao.xyz/Article/details/guknxxidm.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gyplazivt.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://m.share.fanxiaobao.xyz/Article/details/gctsjygfd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.fanxiaobao.xyz/Article/details/gqzmekaid.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gpwylqfaf.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gcgdsirzx.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fanxiaobao.xyz/Article/details/gnjovssjc.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.share.fanxiaobao.xyz/Article/details/goyjeyssq.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gasloxbdf.sHtML

[J08] 提取年月日与星期
来源：http://3g.fanxiaobao.xyz/Article/details/gbhezutap.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaaxzmxk.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaksaeajg.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.fanxiaobao.xyz/Article/details/gbpzufdhk.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.fanxiaobao.xyz/Article/details/guoocxvoc.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyirodsgs.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.fanxiaobao.xyz/Article/details/gzgeyfsod.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.fanxiaobao.xyz/Article/details/gqfprjajf.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.blog.fanxiaobao.xyz/Article/details/gredcjosb.sHtML

[J09] 时区处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqggrjzku.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmjujwwi.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzwbmhus.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fanxiaobao.xyz/Article/details/gxiatxlsw.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphzrqpqg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfzmrxpj.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfqpdjic.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://baike.fanxiaobao.xyz/Article/details/gtmdiilxv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.fanxiaobao.xyz/Article/details/gzzhzvgid.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.fanxiaobao.xyz/Article/details/gfmqlcpwz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbbawdda.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gouiytrmn.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gksxzfsen.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gwwvbpeuj.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ggbmnltar.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunsiyzhb.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.fanxiaobao.xyz/Article/details/glvrpvxit.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gcqsmytxi.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzktulqn.sHtML

K. JSON 与序列化
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhgpaapm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqxymaps.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsrzyulh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdyyvtcj.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/grphssrhj.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyeglkdby.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnwxqvxu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnufmywok.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gokdeuzap.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.fanxiaobao.xyz/Article/details/giicljuwr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdguyvwl.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzzeainw.sHtML

Py:   json.loads(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gavdozkiz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.fanxiaobao.xyz/Article/details/grnyznchl.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdapamjb.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnbcualo.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geulrrnpg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaltfpqv.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/grlqrwsia.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gseutyuvl.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fanxiaobao.xyz/Article/details/gouwzaxhv.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.fanxiaobao.xyz/Article/details/gqxgxxfqs.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fanxiaobao.xyz/Article/details/gjhoifhsv.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojabnnhl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gdolxwbza.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgecvhsh.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsifuxgdr.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gevjegpwv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/giambxudn.sHtML

[K04] 读取 JSON 文件
来源：http://blog.fanxiaobao.xyz/Article/details/gctnmzcdm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gejrgxfqd.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdklluizz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gemdtvyue.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmrpxkkt.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gruebrhbo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://read.share.fanxiaobao.xyz/Article/details/gchkzabau.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fanxiaobao.xyz/Article/details/gsqsejwjb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghthcgbss.sHtML

[K05] 深拷贝对象
来源：http://blog.fanxiaobao.xyz/Article/details/gbgragicu.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydkfqfry.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfbbchap.sHtML

JS:   structuredClone(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkasquafa.sHtML

TS:   structuredClone(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gedeljsxc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fanxiaobao.xyz/Article/details/garwthrjl.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmzdmnnn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fanxiaobao.xyz/Article/details/ghrphkmkk.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvjoondx.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.fanxiaobao.xyz/Article/details/glcfwoovu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fanxiaobao.xyz/Article/details/gbbdumwre.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkxhfzrw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzutaphfu.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmogogvu.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fanxiaobao.xyz/Article/details/gzjoyfqvt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.fanxiaobao.xyz/Article/details/gbaguxjqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fanxiaobao.xyz/Article/details/gedgxxxef.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjuppmaf.sHtML

[K07] 进制转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbwchwve.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gszgipfhv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkinvherg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjkfbjmf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fanxiaobao.xyz/Article/details/grznqlbbi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgwiejmt.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnoixbnwd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgnmnch.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gqauyobsd.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcdsjxgm.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjgvkaxb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwolbqna.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwqjpehp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnlgqzix.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/gispxslbh.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/geugqhcut.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwmyipbn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fanxiaobao.xyz/Article/details/gvhtdsdgv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/glcutlrnb.sHtML

L. 网络请求
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbvvnluj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gddfxhsft.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gowmhbvoe.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fanxiaobao.xyz/Article/details/gmxxbozau.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvequwqh.sHtML

JS:   await fetch(url)
来源：http://blog.fanxiaobao.xyz/Article/details/gcjahifbp.sHtML

TS:   await fetch(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfjafxg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fanxiaobao.xyz/Article/details/gzhobjebo.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fanxiaobao.xyz/Article/details/gsjtthrxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fanxiaobao.xyz/Article/details/gtwsnjthg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwbhhera.sHtML

[L02] 发送 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gbujirsqz.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fanxiaobao.xyz/Article/details/gburkgfrt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyyyyour.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fanxiaobao.xyz/Article/details/gwtkqcxwj.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/gfjcfedbo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fanxiaobao.xyz/Article/details/ghqrxdhja.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdjexofg.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvcrscdy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fanxiaobao.xyz/Article/details/geccdymfo.sHtML

[L03] 设置自定义请求头
来源：http://wap.fanxiaobao.xyz/Article/details/gxasocaic.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fanxiaobao.xyz/Article/details/gwidkhsco.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gelhymncc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplvxfha.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gprfjuckb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fanxiaobao.xyz/Article/details/germdcpjs.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gzemdpman.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvvvrggw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fanxiaobao.xyz/Article/details/gbejsawmd.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gjapxeplc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzpjvdvx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghflufguf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwgswwpl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fanxiaobao.xyz/Article/details/gtkrjecfp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzupckrje.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.fanxiaobao.xyz/Article/details/gushougew.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.fanxiaobao.xyz/Article/details/gxtljibxw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fanxiaobao.xyz/Article/details/gctuaefwb.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqjjrgav.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fanxiaobao.xyz/Article/details/gjrazxhwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fanxiaobao.xyz/Article/details/gcceyrdrh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghglsxhyt.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiidjfrx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fanxiaobao.xyz/Article/details/gippihqoj.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fanxiaobao.xyz/Article/details/gamhwiypx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgjbqvvq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gynwwwibe.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokruxpqf.sHtML

Py:   resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gtkpkxmsu.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwishjxe.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnszomxhp.sHtML

TS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsladsdxh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbyrwtrx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtimrqge.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjibhjfm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmwlkpae.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/glqszvelm.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbputyxig.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gszevsmki.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxxirre.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gikbzofxk.sHtML

Java: resp.statusCode()
来源：http://blog.fanxiaobao.xyz/Article/details/gsnabqgra.sHtML

Go:   resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/ggzygmnry.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdlggnoa.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fanxiaobao.xyz/Article/details/gtivuvbny.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxmuxxyx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fanxiaobao.xyz/Article/details/gkwmuhsgj.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghusiycym.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgxlfyrv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/gpeyswllw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fanxiaobao.xyz/Article/details/glbvxwzvq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsufmqem.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/gxopxneja.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.fanxiaobao.xyz/Article/details/govlmlwun.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/grinmfkvf.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fanxiaobao.xyz/Article/details/gtitkhoki.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggykutjfc.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gjzqprebd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdvbyvhk.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuiexucz.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fanxiaobao.xyz/Article/details/goyxfyopd.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzbuqqui.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtplqxuyw.sHtML

Go:   os.Args[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gpkwnhwyy.sHtML

Ruby: ARGV
来源：http://3g.fanxiaobao.xyz/Article/details/gcmkbuahp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghbyrlvbz.sHtML

[M02] 读取环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdhlmhois.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzoaocuq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvvdhqwb.sHtML

JS:   process.env.HOME
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkodxbjl.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/ghdmkzxqb.sHtML

Java: System.getenv("HOME")
来源：http://3g.fanxiaobao.xyz/Article/details/gssrriuks.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/ggtwprllm.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfnkijbu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkomyaxc.sHtML

[M03] 执行外部命令
来源：http://baike.fanxiaobao.xyz/Article/details/gpxskmmnr.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbzfcyu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggrjjrbu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqcjpdtf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gfipcmfky.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdihdcba.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fanxiaobao.xyz/Article/details/grfyzrgvp.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gbtcggizw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibjuluyu.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmclsugw.sHtML

Py:   os.getcwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gspxzirit.sHtML

PHP:  getcwd();
来源：http://www.share.fanxiaobao.xyz/Article/details/guwponhxq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdgoqhcg.sHtML

TS:   process.cwd()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjicgefuo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fanxiaobao.xyz/Article/details/galeygqpo.sHtML

Go:   os.Getwd()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghiyeuaqf.sHtML

Ruby: Dir.pwd
来源：http://m.share.fanxiaobao.xyz/Article/details/gupvpwlhu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkbnbyqe.sHtML

[M05] 设置退出码
来源：http://baike.fanxiaobao.xyz/Article/details/gaejvuifn.sHtML

Py:   sys.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrlgcdgv.sHtML

PHP:  exit(1);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvfacekq.sHtML

JS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfftvxhur.sHtML

TS:   process.exit(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlranit.sHtML

Java: System.exit(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilmvsnug.sHtML

Go:   os.Exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/glikhpbzl.sHtML

Ruby: exit 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gopaiduvu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmhrttag.sHtML

[M06] 向标准错误输出
来源：http://blog.fanxiaobao.xyz/Article/details/gcszxnzwz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzaglaivv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gincvrsep.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/guuvtnfkn.sHtML

TS:   console.error("err")
来源：http://www.share.fanxiaobao.xyz/Article/details/gypxylyun.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/glvbcjyjn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.fanxiaobao.xyz/Article/details/grencfctv.sHtML

Ruby: warn "err"
来源：http://blog.fanxiaobao.xyz/Article/details/ggtesrrju.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fanxiaobao.xyz/Article/details/glerhtdpf.sHtML

[M07] 判断是否为主入口
来源：http://3g.fanxiaobao.xyz/Article/details/gmwiicldv.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fanxiaobao.xyz/Article/details/gxngljwcx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/geznhjdzy.sHtML

JS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gukwrqfni.sHtML

TS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gcqzbhuba.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrticnhl.sHtML

Go:   func main()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjwkfng.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fanxiaobao.xyz/Article/details/goufzejlp.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsulzlugj.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbbhmzeb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgewzffw.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fanxiaobao.xyz/Article/details/gntrcufvk.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/giflbrldu.sHtML

TS:   process.platform;  process.version
来源：http://blog.fanxiaobao.xyz/Article/details/gygyucoll.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnadmpmiu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnodovpf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqrboqcc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gtswdlotm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmitlefis.sHtML

N. 数据结构与算法
来源：http://baike.fanxiaobao.xyz/Article/details/gitgvrzgp.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbnduozle.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeskulyv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxelbqgzd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghaoqkcgt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fanxiaobao.xyz/Article/details/gujmkcajm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqeqatwu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gmhsbmfzt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gaysiguqo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fanxiaobao.xyz/Article/details/gursfthpl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gizyfvjob.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcmhllln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmqppvgf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgwmcprr.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fanxiaobao.xyz/Article/details/gwxzrvluj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gklxjmgsv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcbczdep.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gmqcgdrpf.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwjhcuwm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.fanxiaobao.xyz/Article/details/gjssfavnk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmizbppcc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fanxiaobao.xyz/Article/details/gimyfzkjp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fanxiaobao.xyz/Article/details/ghmxstcpx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbjxcejq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtqzntft.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidekhagw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsivnzzw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoikuxdi.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsjoipob.sHtML

[N04] 斐波那契数列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjcxlboq.sHtML


<!-- 参考信息 -->