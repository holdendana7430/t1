代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.m.share.hesvh.cn/Article/details/guhbukdrl.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gasxmqfvs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fehbvm.com/Article/details/gdwcjuboh.sHtML

[J06] 计算两时间之差
来源：http://3g.zdbjq.cn/Article/details/gyqpnwnfw.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gukrsrtya.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.fehbvm.com/Article/details/giiskgscw.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://m.share.hesvh.cn/Article/details/gdwooevgh.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gwjgmkaqv.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/grjrtxign.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gqquxpuxy.sHtML

Ruby: end - start                 # 返回秒数
来源：http://mobile.fehbvm.com/Article/details/gdmxfzkcs.sHtML

C#:   (end - start).TotalSeconds
来源：http://read.share.fehbvm.com/Article/details/geupwchkv.sHtML

[J07] 比较两个日期
来源：http://mobile.zdbjq.cn/Article/details/gsqjczkco.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fehbvm.com/Article/details/gkyvvzzut.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.blog.hesvh.cn/Article/details/gypoxgqbs.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gmhvtahfv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/gllpperir.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.zdbjq.cn/Article/details/gwanliakk.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gwguhoakb.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://mobile.hesvh.cn/Article/details/gauafmadn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/goqjeqndz.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fehbvm.com/Article/details/guxesftjv.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.hesvh.cn/Article/details/gehktxjbc.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.hesvh.cn/Article/details/gbaephkxc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.zdbjq.cn/Article/details/gpllzurts.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://3g.zdbjq.cn/Article/details/gdqvcwrcj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/glzcwetzt.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.m.share.hesvh.cn/Article/details/gwrhvbmoj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.hesvh.cn/Article/details/gzoadxocu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/ggnryawdg.sHtML

[J09] 时区处理
来源：http://blog.fehbvm.com/Article/details/gpzwzzdfn.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gawesvtsw.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.zdbjq.cn/Article/details/gbtkjzcir.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gxbssbrna.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.zdbjq.cn/Article/details/ggqwxsokp.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.share.zdbjq.cn/Article/details/gbdwraatb.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.hesvh.cn/Article/details/gejiezlcd.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gegptjzmj.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gymsxseiu.sHtML

[J10] 取今天 / 本月第一天
来源：http://3g.hesvh.cn/Article/details/grlbviauo.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.fehbvm.com/Article/details/gryabeymt.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.m.share.fehbvm.com/Article/details/ghopoiund.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.hesvh.cn/Article/details/gsqwwbfln.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.blog.hesvh.cn/Article/details/ggkgpkpnb.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.zdbjq.cn/Article/details/gpcwybkqt.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.hesvh.cn/Article/details/gunuhmfzk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gnupdrhwv.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/glhglwkxq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gumxonnjl.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/giorlufgg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtjnvsdrp.sHtML

[K01] 对象转 JSON 字符串
来源：http://baike.hesvh.cn/Article/details/ginouarub.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gjbbdphep.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/gvmcrtqja.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.zdbjq.cn/Article/details/grdbwtfpv.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/ggncbkper.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/guwnqtvws.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gqsipuxlg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://wap.zdbjq.cn/Article/details/gsroczrhq.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.zdbjq.cn/Article/details/gyhggiuwd.sHtML

[K02] JSON 字符串转对象
来源：http://wap.fehbvm.com/Article/details/gklfzoiyg.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcpqagwza.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.hesvh.cn/Article/details/gceshgces.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gfegzttyn.sHtML

TS:   JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/gudabyilc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.hesvh.cn/Article/details/gbxbrzxte.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gcjuteelt.sHtML

Ruby: JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gwqzfklfq.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gtwqkjlce.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/gjqyfnhel.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.zdbjq.cn/Article/details/gdpjyfdav.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gmljerfkw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gplwihwos.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gixzdyjgy.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://blog.hesvh.cn/Article/details/gahystjdi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/grjnopnxh.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gmqwsarcw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/getfhvots.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/gihcusigz.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.fehbvm.com/Article/details/gzkypgpzb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.zdbjq.cn/Article/details/gljgmwryi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gksgthziu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gxzpwumda.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gzuyvgrie.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/gvpeknsns.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.hesvh.cn/Article/details/glwxcvyzn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gcboznwul.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gzglfikwm.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gtiyfanmv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gsbsltmqk.sHtML

JS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gmxinsjap.sHtML

TS:   structuredClone(obj)
来源：http://www.share.fehbvm.com/Article/details/guucpasvu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/gltydjmgo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.fehbvm.com/Article/details/gixsfshxh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/glqadiqrs.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.hesvh.cn/Article/details/gmsttqlnp.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gcsjgmswj.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gbtqqqzrj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.zdbjq.cn/Article/details/gwmzbttfr.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gjbboimxo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/gisbpkqde.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gwexalglb.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gmwfhezqr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrwqogc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gcatooooz.sHtML

[K07] 进制转换
来源：http://read.share.hesvh.cn/Article/details/gpyznibdp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/geztbmplj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gwhghckfz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gmbdiirbr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gyrbwiwpv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/greekrmdm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/ghyujuavu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gesjjxkso.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ggxxtmtkv.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gwmevdamz.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.fehbvm.com/Article/details/guamhkhai.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gdwvmmcno.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gvnzsfgud.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gusouakwm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.hesvh.cn/Article/details/gplnmlktd.sHtML

Go:   encoding/gob
来源：http://baike.hesvh.cn/Article/details/govqjvnsj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/gkbgfaquw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gpydupulg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdncpvnwy.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gjluwrmkr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxjevjraf.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gkbztxcci.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gkcfumsah.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/gwbsbmsjq.sHtML

JS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gxzzgvhsm.sHtML

TS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gerdsndfq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gfbzcofuf.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gmriphkxu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/grfxbfjah.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/goqlefjcm.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gvtarypdb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gbqpglaed.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gclcdcfiw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gxzvbhfdz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gdyxtwrrl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.zdbjq.cn/Article/details/gebgkrsbb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gwiiymspi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.hesvh.cn/Article/details/ggtkcutjz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwibvyxon.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/gnxsphszj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gwtxrshpv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.hesvh.cn/Article/details/gvburhekm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gwdncfkgs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gxvqooezq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gzeawuqio.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/guyhzgzgl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gvcucfjcw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/ggvdgewub.sHtML

[L04] 设置超时
来源：http://mobile.zdbjq.cn/Article/details/gbgbubtry.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fehbvm.com/Article/details/gmobjsjjs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gdlpzrwlm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/ggolyvxzm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gyuzrypsx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.zdbjq.cn/Article/details/gowpvafif.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gmvpoflzu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/ghtkxqizt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gamskmijh.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/ggxeylqqg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gzmxldhot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gntthfbnv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gmsdbqvfe.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/geffaybta.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gkwxturam.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gmboqrhhc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gswiufbwz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.zdbjq.cn/Article/details/glhfrgepw.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fehbvm.com/Article/details/gxspeqsmx.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gctsnekbp.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gbxgntcjs.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gzxhghjqe.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gsxhwjzxq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gsvrayqfr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/grwaoqroe.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.fehbvm.com/Article/details/gzntdncpb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqqktktk.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/glcmelnys.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/giesklqsl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gfxlgivbc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gmdzqnepf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gsnobfwvb.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/ggscowbql.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gtsrrdkxh.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/gndwfevkz.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/guouskseh.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gkxbzvvci.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/gvkckrpbh.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gxkmfsxdv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/guszirxeo.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gfsukgybt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gajpljozr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gimmewbam.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/ghblhxrjz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gsttvqjij.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/genhhffmj.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/gehdatvdd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grjezztks.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gsaktgtzk.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gihvggcdv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gyvrcyomp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gxkuwtrmk.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gpplyuxba.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gulgguzol.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/gjkhukrvf.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gkcdxdmci.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gmllmdmmr.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gpqzicpwt.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/ggkzgphpu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gfhteumse.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gzioxvyft.sHtML

TS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/ghyvntysn.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfmgfjmu.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdlrsqrib.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gysytgnsf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gmngpoyhr.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gaxhrdsjk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/goxtgjefi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gdcskaywx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gorlzakhd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gydbhmozg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gxpopwtak.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.fehbvm.com/Article/details/geudigdyk.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/gpxeqkgcv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gmkjropzd.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gmsiregte.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gfmhnbvna.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gaxzqjruv.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gsvclaiow.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gijkiptyq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/ggszcvzgh.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/gzncfugkp.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gsougblol.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.zdbjq.cn/Article/details/gxnnbmvkj.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gdkrxsbfw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvadqtilf.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gfewcmtml.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gpwpsomas.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gevvpplxu.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gqxhzakrq.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmzftqgvr.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gvjaelqnx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gaoczumau.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/garbczynf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/gtjyzfosu.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gaklvfhle.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/galydwuvz.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gyjhnbvrj.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtjxcbbtm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gyjockpvg.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gppuegnqq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.hesvh.cn/Article/details/gxinvlrvt.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gpkfgfroy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gzwsmrzds.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/giwgmueck.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gmzjuvtxm.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gdidgnakb.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gdjrkwrex.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gtlbpfrjd.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gxcyjzdft.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gzesfhdzg.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/guamnvdrz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gzgstqrox.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gsjpbgzoy.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/glxbqwtdm.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/grrkxeyya.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gfxguuszm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gwitfenwa.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gmqnzlrxc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/ggocegmtj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gszhfnpyt.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gwizgirjf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxmcyrrok.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.fehbvm.com/Article/details/gnsxahlir.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gdhfxxoqp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gagnbyuxg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gxkpclmkq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gijkckeuv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdomtmrtd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gowxsvlgs.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.fehbvm.com/Article/details/gjhcmrroj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqfacjygl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gejibbzra.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/glbwjqtae.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gcpllwqwj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gimhmmign.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gdhfywoqh.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.hesvh.cn/Article/details/giguzmfwt.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gfbecxvnd.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/ghbbhafje.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gmibzakhc.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/grllvsawd.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gqglhfmxq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gbcisftfd.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gszcrerje.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gihmmbxts.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gfzfsniff.sHtML


<!-- 参考信息 -->