代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fanxiaobao.xyz/Article/details/gobvcurxu.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnllgpxzd.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgbjeujl.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntpqzecz.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/goyebnlif.sHtML

Ruby: Time.now + 7 * 86400
来源：http://blog.fanxiaobao.xyz/Article/details/gqzfbgtdy.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gipsvknvi.sHtML

[J06] 计算两时间之差
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzzqlvsy.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwkvxfcb.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifzcnkep.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsuhqkfv.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://3g.fanxiaobao.xyz/Article/details/gnotgaipp.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhivfobs.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxzvjdsp.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fanxiaobao.xyz/Article/details/gtqgkcezb.sHtML

C#:   (end - start).TotalSeconds
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpatjxeh.sHtML

[J07] 比较两个日期
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpafhgow.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://m.share.fanxiaobao.xyz/Article/details/grbmcnvaw.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fanxiaobao.xyz/Article/details/gwkprfflv.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fanxiaobao.xyz/Article/details/glpctkbao.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fanxiaobao.xyz/Article/details/gadslizab.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigboptxh.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdprdaap.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhaohjza.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://wap.fanxiaobao.xyz/Article/details/gaxkeiqyk.sHtML

[J08] 提取年月日与星期
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzuhjrkd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.fanxiaobao.xyz/Article/details/gonyycyfi.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fanxiaobao.xyz/Article/details/gndppcadi.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaookrbxn.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://baike.fanxiaobao.xyz/Article/details/gwhkxnqnl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.fanxiaobao.xyz/Article/details/gxebpngpc.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.fanxiaobao.xyz/Article/details/gwgwhtpak.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.fanxiaobao.xyz/Article/details/gnwrxvusl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://blog.fanxiaobao.xyz/Article/details/gwhzvbmfb.sHtML

[J09] 时区处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gecyfbfxf.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqespotg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlfkkwcp.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fanxiaobao.xyz/Article/details/goqpyxdis.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.fanxiaobao.xyz/Article/details/gjihfzlic.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrioxgxf.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fanxiaobao.xyz/Article/details/gvhbjdlgg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.fanxiaobao.xyz/Article/details/gtunxcspp.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fanxiaobao.xyz/Article/details/gdedijjgu.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fanxiaobao.xyz/Article/details/goxadwnsg.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtewmgesx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fanxiaobao.xyz/Article/details/gysfhpdvi.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkiwuxrfi.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/ggdxswqyu.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnecrshe.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.fanxiaobao.xyz/Article/details/gjopdejuy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.fanxiaobao.xyz/Article/details/gvmpwebzq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdjsoebf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfibrvkj.sHtML

K. JSON 与序列化
来源：http://read.share.fanxiaobao.xyz/Article/details/grnvchmnp.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdejxidbq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwhkkbas.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/glzdehkvu.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fanxiaobao.xyz/Article/details/gecvkdxwj.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvfnavdj.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gmyefeabu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvaldzth.sHtML

Go:   json.Marshal(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksftdkjo.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggimcpdss.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqcsswvp.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fanxiaobao.xyz/Article/details/gurxtqcnz.sHtML

Py:   json.loads(s)
来源：http://blog.fanxiaobao.xyz/Article/details/grsyfwshx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmrmqfeg.sHtML

JS:   JSON.parse(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsyjxcknu.sHtML

TS:   JSON.parse(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpkbfateb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqejuldt.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkmkkgcp.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnonbaey.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gyzpmareq.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fanxiaobao.xyz/Article/details/goxgoxlap.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fanxiaobao.xyz/Article/details/gyvewbmqy.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtbmonsy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnysfiyqr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdkbtyjmf.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gouszettl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fanxiaobao.xyz/Article/details/gtpovcobv.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhiggrwz.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjtgdeyz.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gafxjnxbw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fanxiaobao.xyz/Article/details/guvyvluvg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.fanxiaobao.xyz/Article/details/gftbmxpml.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaihvxpm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpodudegr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyeoysaj.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhpuymil.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvhvpbid.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gprvcnafy.sHtML

[K05] 深拷贝对象
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgmacmuw.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/goutvzcqb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.fanxiaobao.xyz/Article/details/grgfmfgqs.sHtML

JS:   structuredClone(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/ghodsidem.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqyvonum.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fanxiaobao.xyz/Article/details/gmparxoxq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fanxiaobao.xyz/Article/details/gktkajfdu.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfqwolmo.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fanxiaobao.xyz/Article/details/gecwrzzoy.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcukvyta.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gtycsvzhh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmuobtfce.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfrilauq.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlidjlvt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufosnlrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fanxiaobao.xyz/Article/details/gjemqjwyr.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fanxiaobao.xyz/Article/details/ggrmigqgo.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjerkrcit.sHtML

[K07] 进制转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjksxfoft.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fanxiaobao.xyz/Article/details/gwkhwqkxp.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgcvtmfa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpmrzxyt.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.fanxiaobao.xyz/Article/details/giszucbvd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gpnsafirh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrbjupyu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsiwuvcw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fanxiaobao.xyz/Article/details/gopyyivfz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.fanxiaobao.xyz/Article/details/ggafthskz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbufjyw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwstupcb.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fanxiaobao.xyz/Article/details/glwnirdhn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fanxiaobao.xyz/Article/details/guxjlzwth.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fanxiaobao.xyz/Article/details/goasonrvz.sHtML

Go:   encoding/gob
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvqnpfu.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnnboxxe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.fanxiaobao.xyz/Article/details/gqmbsgyvi.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/geegbsfvq.sHtML

L. 网络请求
来源：http://blog.fanxiaobao.xyz/Article/details/gmibbyuym.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvekzncqi.sHtML

[L01] 发送 GET 请求
来源：http://baike.fanxiaobao.xyz/Article/details/gevnixgxz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbylmsusr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.fanxiaobao.xyz/Article/details/gshmvtnwt.sHtML

JS:   await fetch(url)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwmxtpjc.sHtML

TS:   await fetch(url)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakbagmyn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fanxiaobao.xyz/Article/details/gqppvjtlu.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvtsmqka.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fanxiaobao.xyz/Article/details/gwadveacz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fanxiaobao.xyz/Article/details/gbuinxjxv.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gerbdebke.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbnyogph.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweymeikh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/guatbtijx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fanxiaobao.xyz/Article/details/gvhiuagjf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gfxrdozet.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fanxiaobao.xyz/Article/details/gornmcsuo.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhtgytuh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fanxiaobao.xyz/Article/details/gdshjyjeg.sHtML

[L03] 设置自定义请求头
来源：http://3g.fanxiaobao.xyz/Article/details/gbxfpmyhf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiemiqkd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gbraswnsp.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fanxiaobao.xyz/Article/details/gwknzbatq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlvxzavj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fanxiaobao.xyz/Article/details/ggtmxwtfq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fanxiaobao.xyz/Article/details/gedljnhit.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fanxiaobao.xyz/Article/details/glvqnnmhs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/ggnzqsjih.sHtML

[L04] 设置超时
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyewacoc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fanxiaobao.xyz/Article/details/gptkkabwy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gjfxcrsrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqxegvrv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfgcaoj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fanxiaobao.xyz/Article/details/gojtiolry.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fanxiaobao.xyz/Article/details/gbkvqpcyu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gffeaeeam.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvserhno.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fanxiaobao.xyz/Article/details/gajungmhb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.fanxiaobao.xyz/Article/details/gveiwiazc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fanxiaobao.xyz/Article/details/gxghbhqbp.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gyebfczde.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjjhdwih.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjxguepq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvzyqqynk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvmvxswr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwzripes.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gvpdxbstb.sHtML

Py:   resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtnofjrnv.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxnhrnbl.sHtML

JS:   await resp.json()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbruwrwre.sHtML

TS:   await resp.json()
来源：http://wap.fanxiaobao.xyz/Article/details/gensiwaub.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvokblqp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fanxiaobao.xyz/Article/details/gwdicuabx.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fanxiaobao.xyz/Article/details/gbdqwzvdp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fanxiaobao.xyz/Article/details/gxvmdrurm.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gashxfcku.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fanxiaobao.xyz/Article/details/grolyvldu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpigqzwoe.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fanxiaobao.xyz/Article/details/gntjmrwfk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fanxiaobao.xyz/Article/details/gooukplua.sHtML

Java: resp.statusCode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gscwtqdqq.sHtML

Go:   resp.StatusCode
来源：http://www.share.fanxiaobao.xyz/Article/details/grlswxfqo.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscxjhmin.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.fanxiaobao.xyz/Article/details/gpknuzjwl.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhfpbmnj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fanxiaobao.xyz/Article/details/glqdrngsq.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fanxiaobao.xyz/Article/details/grahjdcta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiynvvvr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmpxcqit.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fanxiaobao.xyz/Article/details/gjjbyfgtk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpbxkjwt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fanxiaobao.xyz/Article/details/goyohgsdk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlizzpiz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gabexhodi.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fanxiaobao.xyz/Article/details/ghzhvmmfk.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/grokzbann.sHtML

[M01] 读取命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwzeejq.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdswhdsy.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fanxiaobao.xyz/Article/details/ghakjwfxe.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fanxiaobao.xyz/Article/details/gqpntphli.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghubflzza.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.fanxiaobao.xyz/Article/details/ghffrcglm.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvywsrouw.sHtML

Ruby: ARGV
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmvuqwik.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fanxiaobao.xyz/Article/details/gbmulnoty.sHtML

[M02] 读取环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/grddluesh.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaxiqgdq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fanxiaobao.xyz/Article/details/gzuemuszy.sHtML

JS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gyzrzecuf.sHtML

TS:   process.env.HOME
来源：http://wap.fanxiaobao.xyz/Article/details/gxboxhhzo.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxebxmjs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmxnswir.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxdowpud.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gtrbjvief.sHtML

[M03] 执行外部命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqzkiblg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gjanvgliw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrjpujuj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhpkoboz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/guvngrwob.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbtikkbw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcggjncpi.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fanxiaobao.xyz/Article/details/gszubeabv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fanxiaobao.xyz/Article/details/gbepqztnj.sHtML

[M04] 获取当前工作目录
来源：http://wap.fanxiaobao.xyz/Article/details/gptfjjpon.sHtML

Py:   os.getcwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbyieswl.sHtML

PHP:  getcwd();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdzhnstb.sHtML

JS:   process.cwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuawmxnn.sHtML

TS:   process.cwd()
来源：http://wap.fanxiaobao.xyz/Article/details/gisuoledw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmfzsgwy.sHtML

Go:   os.Getwd()
来源：http://wap.fanxiaobao.xyz/Article/details/glejpchtz.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvcgpsvd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fanxiaobao.xyz/Article/details/gonocdktg.sHtML

[M05] 设置退出码
来源：http://baike.fanxiaobao.xyz/Article/details/gqvmifter.sHtML

Py:   sys.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gkzzclbmt.sHtML

PHP:  exit(1);
来源：http://blog.fanxiaobao.xyz/Article/details/gvevmuznk.sHtML

JS:   process.exit(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gchaywkjz.sHtML

TS:   process.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjyigtdc.sHtML

Java: System.exit(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbbcbmbv.sHtML

Go:   os.Exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/grfpauzpd.sHtML

Ruby: exit 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/grugjuhrl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fanxiaobao.xyz/Article/details/geyryejzj.sHtML

[M06] 向标准错误输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcfeeskc.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbmwqtyf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.fanxiaobao.xyz/Article/details/ghzythfwo.sHtML

JS:   console.error("err")
来源：http://wap.fanxiaobao.xyz/Article/details/guaitfbkb.sHtML

TS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/goriywccs.sHtML

Java: System.err.println("err")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtujqirmn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgouhnkc.sHtML

Ruby: warn "err"
来源：http://baike.fanxiaobao.xyz/Article/details/gepwxfkyi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fanxiaobao.xyz/Article/details/gomfkxorq.sHtML

[M07] 判断是否为主入口
来源：http://www.share.fanxiaobao.xyz/Article/details/glmcvwkws.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fanxiaobao.xyz/Article/details/gxpvfnknn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fanxiaobao.xyz/Article/details/glgzrrihk.sHtML

JS:   require.main === module
来源：http://m.share.fanxiaobao.xyz/Article/details/gnovgcvnr.sHtML

TS:   require.main === module
来源：http://blog.fanxiaobao.xyz/Article/details/gqojbhlev.sHtML

Java: public static void main(String[] args)
来源：http://wap.fanxiaobao.xyz/Article/details/gvdrhpnhw.sHtML

Go:   func main()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfiufqrc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fanxiaobao.xyz/Article/details/gifqouecn.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlbgucmj.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwyknqxh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjfwflyk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsmokjbq.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrbrmzya.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fanxiaobao.xyz/Article/details/gribqtufo.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fanxiaobao.xyz/Article/details/gpnywqqfk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxuqlgav.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fanxiaobao.xyz/Article/details/giwhprmnf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fanxiaobao.xyz/Article/details/gglkytajq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glktwkopl.sHtML

N. 数据结构与算法
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtyigiaz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/goozqfgpr.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gdgbbezkt.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gegtfaxma.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsthklczh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gxjwqcldr.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmdklwqj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gmppgpedo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgsnsown.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcphwnge.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/goikkdzoz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtoajbsju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhtytkt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjorxlmp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjqhjjmuf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gprfjiyqc.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqiwtxac.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqogkldqb.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gspbokxrn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/ghafeoisu.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpqztjk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwzngfou.sHtML


<!-- 参考信息 -->