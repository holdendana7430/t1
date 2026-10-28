代发 wailian999

TS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtexosmiqt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.dianchejie.cn/gtrdsujsfe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj202588.top/gtqwulorrt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtjrphjqav.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtmialweqg.html

[J04] 时间戳与日期互转
来源：http://hz.zhengqikj.top/gteqkormyp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtphbesjfa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtfbzvggpy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtbvnumqcz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gtpsjkeovm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtcyifxuxj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hysaishi.cn/gtqqzsgkrs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtzeztnlwr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sweek.top/gtnahcihif.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtnzewgsci.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtytbsjwfm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtkcsjlfxn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtwbygzjrx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtgakwhdzu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtxmoalznm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zdqjudy.top/gtqrghryet.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gttshvitog.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shangyingyoupin.top/gttgjmhize.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtquzinkjr.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtemkntiny.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtbjzjvpng.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yangfankeji.com/gtskxmdvwk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shangyingyoupin.top/gtiskjcvqi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtaywzvgiw.html

Go:   end.Sub(start).Hours()
来源：http://hz.0kj1m.cn/gtbvcofrfd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gthmafnzqn.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtvurneomy.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtztiulehe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtgoudutyc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtepphgzjd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtmhtgmhvj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtkwqhlkqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtpovctmhw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtwgwxgnuf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtvlqmamjg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtwlgyppqm.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gtjdzvbigl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtjvzoptal.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtxbbgypwh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.0kj1m.cn/gtstgsgqxg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuxming.cn/gtbmdqaggq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtywrtedfm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gteedckyqi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gttcmsojdq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yueranfly.top/gtzcivwgga.html

[J09] 时区处理
来源：http://hz.snrcjt.cn/gtpcgkpung.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.aibaodan.cn/gtelbmyskf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj20258888.top/gtzpbskcyc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtnwyizcim.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtgiloiyjn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gthzxydtwl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtwezciyge.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shangyingyoupin.top/gtkwabhnwo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxinkj.top/gtlfjztbfr.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gtsxrvpmol.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenlongwang.top/gtiyjvfxsy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtrnyxhccg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtnbiqxnvd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtpnknuqqj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangtech.top/gthmtvfnwc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtknyxtzfj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtpefdoeen.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtsoeqpfrm.html

================================================================================
来源：http://hz.shzxlz.cn/gtkggwlnoq.html

K. JSON 与序列化
来源：http://hz.andypj.xyz/gtirfhtedn.html

================================================================================
来源：http://hz.ybcxt.top/gtfnvkbzyl.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtqobscafh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtrmclotcg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtffogqtqy.html

JS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtwwkboywq.html

TS:   JSON.stringify(obj)
来源：http://hz.vqdsnc.cn/gtbnloffzu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jianghu66.top/gtrrfbodhf.html

Go:   json.Marshal(obj)
来源：http://hz.shanyushiyangkeji.top/gtecwhhopj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cashguo.top/gtctlpjuky.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gttcrdouuv.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtvajckuan.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtyzitvfqm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gtgekmfrrq.html

JS:   JSON.parse(s)
来源：http://hz.yongpay.top/gtobivgika.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtweixltuu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtengokgdc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtofgcnqkx.html

Ruby: JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtjakkmerv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tanke756.top/gtyvkhotii.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtwffigrvt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtaomdqjad.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtqlewgetg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtrulbebbe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtogywgvtn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtjjcdshmn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtvdygjldz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtfcidhbyb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zycfv.cn/gtnwyelydf.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gtgcugtbon.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtbumjuumo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gtqhjktfqb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtaaszxeep.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtyztutblg.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hnxiangtu.top/gtimerehgk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtjydkqqah.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtizveszus.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jqgfzy.top/gthwymxydl.html

[K05] 深拷贝对象
来源：http://hz.xinyue.icu/gthexpiszi.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtyyqccqhi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.mhx1999.top/gtdxyzpkdo.html

JS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtdhvpzvvy.html

TS:   structuredClone(obj)
来源：http://hz.dashuyun.cn/gtgurobbcu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtrirdauir.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuanzhike.top/gtqrvemauw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxinkj.top/gtkannbnuh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.mhx1999.top/gtysmxwqfk.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gttihwhhao.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gtyrrwzosy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtskxrvzqa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtixddxtfl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtwjsjhbvw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gtkmscwwfh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtjphwjixs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtvgopzqtg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yanxiufei.cn/gtdyhtjlyj.html

[K07] 进制转换
来源：http://hz.zycfv.cn/gtjysooiku.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gttfexklal.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xinyue.icu/gtlboljnzq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtvjahsbii.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtmwfxzxwb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtrpflzmgz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtygkgtdyn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gteaihcgih.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.fengsongda.top/gtyzegkiik.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.mhx1999.top/gtmqaszhti.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtldqgqoop.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtdlbpbxqk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtatzncamm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hongshengwenyu.top/gtcbvyuvbi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gttrplbtpa.html

Go:   encoding/gob
来源：http://hz.yj20258.top/gtattpfwrk.html

Ruby: Marshal.dump(obj)
来源：http://hz.tanke756.top/gtwtbnzund.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.tanke756.top/gtmmaoughi.html

================================================================================
来源：http://hz.snrcjt.cn/gtdjrepppw.html

L. 网络请求
来源：http://hz.zycfv.cn/gtcuygvutd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtigplbecs.html

[L01] 发送 GET 请求
来源：http://hz.sweek.top/gtpcskzcoy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtvbhlsoko.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gtwkapxmxg.html

JS:   await fetch(url)
来源：http://hz.sysykeji.top/gtfjvxpgfr.html

TS:   await fetch(url)
来源：http://hz.gzhubu.top/gtfeikjxzp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yj20258.top/gtvhndnxda.html

Go:   resp, err := http.Get(url)
来源：http://hz.jlsjyb.cn/gthkemwxqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dashuyun.cn/gtljdokjfc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.cashguo.top/gtfqytqjcg.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gtapmlzizy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtgcqqcuiu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.shzxlz.cn/gtfzhbnfdh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yuxming.cn/gtulrqmqsk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtkftjmaes.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.bjfxy.top/gtorisxgkh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cqqwz.cn/gtbofmyttf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shanyushiyangkeji.top/gtjhqwzxtc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.kuanghao11.cn/gtsfeoobxu.html

[L03] 设置自定义请求头
来源：http://hz.daria6918.cn/gtptzmuqiz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daxiang520.top/gtybastkxl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtpaqfzpvy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jqgfzy.top/gtrtgyelrm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtkyjgjlqz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtydvlznyw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zdqjudy.top/gtqbwpijhe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xinyue.icu/gtloqtjzht.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.nanxinkj.top/gtrwvqschh.html

[L04] 设置超时
来源：http://hz.fengsongda.top/gtlkcamljc.html

Py:   requests.get(url, timeout=5)
来源：http://hz.shuidangran.top/gtonbylwqb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtpezwcwtg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.fzhhl.top/gtexfbjros.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yanxiufei.cn/gtmwyhgdvt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtyufydbid.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ydzc1.top/gttpzbijnb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xylfe.cn/gtyefijlho.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cucudq.cn/gtnytzcvsh.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtbysiddnp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigufen.top/gtnjdpttjh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yangfankeji.com/gtzrmnxsqq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtsygafbnq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ehwqpu.com/gtwvgvwmho.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cucudq.cn/gtrwzlzuzp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtxmxrphzm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhixingplan.top/gtogszfdgf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.dashuyun.cn/gtqljocgzs.html

[L06] 解析响应为 JSON
来源：http://hz.yangfankeji.com/gtcdswjknj.html

Py:   resp.json()
来源：http://hz.fzhhl.top/gtfaapqipr.html

PHP:  json_decode($body, true);
来源：http://hz.zhixingplan.top/gtbexsvijx.html

JS:   await resp.json()
来源：http://hz.hnxiangtu.top/gtsmxfewwm.html

TS:   await resp.json()
来源：http://hz.ehwqpu.com/gtadrxrvks.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.chenjidiqi.icu/gtwbkmiowp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.nwbrower.top/gtcsvvimjh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.gaohongyu789.top/gtarjaspcj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shanyushiyangkeji.top/gtgfdbuhll.html

[L07] 处理 HTTP 状态码
来源：http://hz.andypj.xyz/gtkimdpiiu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shanyushiyangkeji.top/gtkqwtfzpa.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.haohaochexian.top/gtdusvzvzt.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtpmabbwuo.html

TS:   resp.ok;  resp.status
来源：http://hz.aizwys.cn/gtpyndfwnt.html

Java: resp.statusCode()
来源：http://hz.daxiang520.top/gtejenmfsv.html

Go:   resp.StatusCode
来源：http://hz.hnqzz.top/gteuerfgzz.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtnlidsoxv.html

C#:   (int)resp.StatusCode
来源：http://hz.xuetiantiany.cn/gtntlkmwfo.html

[L08] 并发请求多个地址
来源：http://hz.birdmap.top/gtslzbncsb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jiagoushi.top/gtczerxapk.html

PHP:  curl_multi_init() 系列
来源：http://hz.nanxuanxn.top/gtenvysjrk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fengsongda.top/gtnqrwjkzo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yonumen.top/gtkvzftxti.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.gaohongyu789.top/gtgfvojyik.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.shzxlz.cn/gtcinvojtc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.xuanzx.com/gturdqxkrf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhongyouzk.top/gticqwhtzk.html

================================================================================
来源：http://hz.316326.xyz/gtmmeoxhgw.html

M. 命令行 / 进程 / 环境
来源：http://hz.cashguo.top/gtqifqabsl.html

================================================================================
来源：http://hz.sweek.top/gtludtcqxc.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtpkfjycci.html

Py:   sys.argv[1:]
来源：http://hz.jinqigufen.top/gtzpzlhrro.html

PHP:  $argv;  $argc;
来源：http://hz.aizwys.cn/gtearzsckh.html

JS:   process.argv.slice(2)
来源：http://hz.sufxvd.cn/gtciygsyze.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtllbvknwf.html

Java: args 数组（main 方法参数）
来源：http://hz.gotoacloud.top/gtyelulmqn.html

Go:   os.Args[1:]
来源：http://hz.hysaishi.cn/gtqjjtxpfa.html

Ruby: ARGV
来源：http://hz.vqdsnc.cn/gtgbnjadfu.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhengqikj.top/gtfmodcdef.html

[M02] 读取环境变量
来源：http://hz.gzhubu.top/gtckktxdjs.html

Py:   os.environ.get("HOME")
来源：http://hz.316326.xyz/gtaeeovrri.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhoulong.xyz/gtaydarwfg.html

JS:   process.env.HOME
来源：http://hz.jinqigufen.top/gtwnbwnmsq.html

TS:   process.env.HOME
来源：http://hz.xingfuxueyuan.xyz/gtxqxdladd.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gttvvzqfly.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtusgzzwan.html

Ruby: ENV["HOME"]
来源：http://hz.sufxvd.cn/gtxsqrwqsl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jqgfzy.top/gtkfjetgev.html

[M03] 执行外部命令
来源：http://hz.shanyushiyangtech.top/gtreatsmnn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gthhwucuxw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yj20258888.top/gtlwqyxfal.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtcieydshh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtkhnkhjeq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.guowangkeji.top/gtdfettxyk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.xingfuxueyuan.xyz/gtiivjxkvr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xuetiantiany.cn/gtkayuihox.html

C#:   Process.Start("ls", "-l");
来源：http://hz.meibo888.top/gtwgvqdywm.html

[M04] 获取当前工作目录
来源：http://hz.feifeiyinyue.top/gtkivoqtfg.html

Py:   os.getcwd()
来源：http://hz.ywan-chungtsiang.top/gttzgkdgzt.html

PHP:  getcwd();
来源：http://hz.aibaodan.cn/gtfdmzbbwi.html

JS:   process.cwd()
来源：http://hz.nwbrower.top/gticyhesuv.html

TS:   process.cwd()
来源：http://hz.c1oappe.top/gthgfglgll.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.hfpthk.cn/gtkmskiymn.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtyvmjijsf.html

Ruby: Dir.pwd
来源：http://hz.feifeiyinyue.top/gtxwgnmhbb.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.ywan-chungtsiang.top/gtzoavjllc.html

[M05] 设置退出码
来源：http://hz.birdmap.top/gthowxseuj.html

Py:   sys.exit(1)
来源：http://hz.chenjidiqi.icu/gtkgnjjvke.html

PHP:  exit(1);
来源：http://hz.havefunace.top/gtatiuvblo.html

JS:   process.exit(1)
来源：http://hz.hysaishi.cn/gthpgvesco.html

TS:   process.exit(1)
来源：http://hz.ywan-chungtsiang.top/gtabwxqhvd.html

Java: System.exit(1)
来源：http://hz.zhoulong.xyz/gtvbczxvjr.html

Go:   os.Exit(1)
来源：http://hz.iojbl.cn/gtidtuyrzl.html

Ruby: exit 1
来源：http://hz.gotoacloud.top/gtjwitauge.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtojhoxtjx.html

[M06] 向标准错误输出
来源：http://hz.xinyue.icu/gteauwsydl.html

Py:   print("err", file=sys.stderr)
来源：http://hz.hnxiangtu.top/gtrpmotjhb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.snrcjt.cn/gtsmrzwbfx.html

JS:   console.error("err")
来源：http://hz.yj20258.top/gtghkoygzi.html

TS:   console.error("err")
来源：http://hz.hfpthk.cn/gtlvkhohfv.html

Java: System.err.println("err")
来源：http://hz.sufxvd.cn/gtegfzvliv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinqigufen.top/gtvuosovzk.html

Ruby: warn "err"
来源：http://hz.hysaishi.cn/gtneettmig.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.hfpthk.cn/gtcggzvwoa.html

[M07] 判断是否为主入口
来源：http://hz.xinyue.icu/gtknrketeu.html

Py:   if __name__ == "__main__":
来源：http://hz.zhengqikj.top/gtboevswcj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.nanxuanxn.top/gtizmpjkdn.html

JS:   require.main === module
来源：http://hz.yonumen.top/gtaihhekek.html

TS:   require.main === module
来源：http://hz.shzxlz.cn/gtmajuenth.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtsdkzbwli.html

Go:   func main()
来源：http://hz.0kj1m.cn/gtfqlxzopk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.yvedp.cn/gtfvjawxrf.html

C#:   static void Main(string[] args)
来源：http://hz.shuidangran.top/gtvtmrzqqo.html

[M08] 获取系统与运行时信息
来源：http://hz.zhengqikj.top/gtbfaeqgge.html

Py:   platform.system();  platform.python_version()
来源：http://hz.redwolf501.top/gtypsnlktj.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xuanzx.com/gtzobikhww.html

JS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtgcxhelqm.html

TS:   process.platform;  process.version
来源：http://hz.gogol.net.cn/gtmwjospmi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.pengpengdd.cyou/gtnjhfmwxv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.svipenyu.cn/gtfqqcxstx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.nanxuanxn.top/gtatblbqxp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.redwolf501.top/gtczwomzdu.html

================================================================================
来源：http://hz.bjfxy.top/gtdpiiutja.html

N. 数据结构与算法
来源：http://hz.yj202588.top/gtruxtfanf.html

================================================================================
来源：http://hz.gotoacloud.top/gtvqibbxpa.html

[N01] 二分查找（有序数组）
来源：http://hz.ywan-chungtsiang.top/gtpklymxgk.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.jqgufenzy.top/gtmmycivaq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.andypj.xyz/gtyvurysha.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.zhaomingkeji.xyz/gtclqergsg.html


<!-- 参考信息 -->