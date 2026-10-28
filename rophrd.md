代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangkeji.top/gtnkiwargw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtniysbihj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtnsanshxg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gttftyzpli.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zycfv.cn/gtblhlnfjt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pycfn.com/gtqazmcdwv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtkkgxuzrn.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gttfbwfqam.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtyzynfzuv.html

PHP:  $end->diff($start)->days;
来源：http://hz.sysykeji.top/gtqfrabqyt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtzokecxku.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinyuanbaomall.cn/gteolfqckl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhongyouzk.top/gtlefsedtb.html

Go:   end.Sub(start).Hours()
来源：http://hz.jianghu66.top/gtqmnkmvxe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zycfv.cn/gttinmnjxf.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtyfyfpmms.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtbjritzcp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtgwgekmma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hnqzz.top/gtwvjjtrdb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtpauutrgv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtdtzmjquv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fengsongda.top/gtbcuubynk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtazujbhkt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtkyjbrcji.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtchuhnueu.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gtlvodgnww.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtoxmxvxou.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gtrbqcjggt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.smart0.xyz/gthrhvrnbh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gttknbjtqt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtbxbiopxc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtvwsjtkfy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtonxuzhnd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.redwolf501.top/gtwrhjrsxa.html

[J09] 时区处理
来源：http://hz.jqgufenzy.top/gthngodcdi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtkygdbsmq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.birdmap.top/gtgpoubvko.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtgdfexfxp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangtech.top/gtpuivvtaj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtuopukava.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtbpxazdmp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gttaincbrg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtpegntrps.html

[J10] 取今天 / 本月第一天
来源：http://hz.pengpengdd.cyou/gtzueglbnx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtifrjonnu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cashguo.top/gthbbrwkpz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtafkcmfun.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtjoddksid.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhengqikj.top/gtmdwojzht.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtefmgygfm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhongyouzk.top/gtdvtguzbz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.tian-w.cn/gtbcxamnst.html

================================================================================
来源：http://hz.ydzc1.top/gtqdtseffd.html

K. JSON 与序列化
来源：http://hz.yuanzhike.top/gtsdqbrsjm.html

================================================================================
来源：http://hz.jianghu66.top/gtqgcxkfaa.html

[K01] 对象转 JSON 字符串
来源：http://hz.cheryme.top/gtajrupvyv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtalzqzafz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhaomingkeji.xyz/gtoouuimtv.html

JS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtjjxmlzuz.html

TS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtcqenuvao.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.chenlongwang.top/gtidwkkfmh.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtwcnhrtkx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guowangkeji.top/gtizhucrsd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtghvhiouw.html

[K02] JSON 字符串转对象
来源：http://hz.tanke756.top/gtwkpgxmmp.html

Py:   json.loads(s)
来源：http://hz.ybcxt.top/gtbtggeltc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtusvuwsxu.html

JS:   JSON.parse(s)
来源：http://hz.wangdashe.top/gtbrsfgnrd.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtpaisoewu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtutmtfxoe.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtlmmdtdbl.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtidloikyj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.52xcode.cn/gtbnoskucl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.c1oappe.top/gthnxrvskk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhaomingkeji.xyz/gtfhrcvzuj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtyaljvqwi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtstmijpua.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtwlgptolx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtzmttlfvf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ivvv.top/gticutbljo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtfkuhjyhu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pengpengdd.cyou/gtdehrymwy.html

[K04] 读取 JSON 文件
来源：http://hz.nwbrower.top/gtpcechwzt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtucayaank.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtszvovmgq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gtvryfjemr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtjhjvkxzr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gttptmilcv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtutezqakm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.wangshuangyany.cn/gthbfgqicv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtlnivzcln.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtdhatssap.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtuoarlknk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ppjwa.cn/gtpkcwxsoh.html

JS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gthodgrfhu.html

TS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtcaxanacq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.iojbl.cn/gtxcjznlqn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xinyue.icu/gtqzxawpet.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtdvwnbimv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtgruzkwfl.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtnbkrmail.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtwcxapvas.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtoxhjeoiw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtqixszlbu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtxidrhcjm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtzlkqsioj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtotopbbjd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtykyyikgw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtlsbfdapq.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gthoewzdnu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gtahpssvqw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj202588.top/gtyyqptyoa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtatzoilvz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtlpefczyn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtoixtygua.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zdqjudy.top/gtzwfdfjpi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gogol.net.cn/gtksvvidsi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jiagoushi.top/gtjoczigtc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnqzz.top/gtuoicodyr.html

Py:   pickle.dumps(obj)
来源：http://hz.ehwqpu.com/gtgnkatyln.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhaomingkeji.xyz/gtbqretmpp.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtyvxvgfrj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtpyrdmsrq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gthoskotts.html

Go:   encoding/gob
来源：http://hz.andypj.xyz/gtwuudznkn.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtugawrzha.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.c1oappe.top/gtkxcedwxs.html

================================================================================
来源：http://hz.nwbrower.top/gtfnsiwmyk.html

L. 网络请求
来源：http://hz.c1oappe.top/gtbeetkfcn.html

================================================================================
来源：http://hz.nanxinkj.top/gtslmyitqt.html

[L01] 发送 GET 请求
来源：http://hz.birdmap.top/gtevuercsq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.feifeiyinyue.top/gtuhexjsbt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtbibtfozy.html

JS:   await fetch(url)
来源：http://hz.shangyingyoupin.top/gtmszzbruc.html

TS:   await fetch(url)
来源：http://hz.0kj1m.cn/gtbaugxuby.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jianghu66.top/gtehjorstu.html

Go:   resp, err := http.Get(url)
来源：http://hz.nanxinkj.top/gtzzkizcvn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.wangshuangyany.cn/gtgnbplaba.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yvedp.cn/gtimynmefk.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtsyicdfoi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zycfv.cn/gtlrwagghn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.kuanghao11.cn/gtmlmgeapv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtcpzhloao.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhengqikj.top/gtywjuxqzd.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shuidangran.top/gtojhpnyac.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.meibo888.top/gtcfusrmau.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.kuanghao11.cn/gtmuhmdpkc.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.dashuyun.cn/gtqiqjqiul.html

[L03] 设置自定义请求头
来源：http://hz.svipenyu.cn/gtuqhyobnd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sysykeji.top/gtzqmnsvep.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yongpay.top/gtqwliaaiu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shuidangran.top/gtdhtvrdjv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xinyue.icu/gtucpoiyjs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhaomingkeji.xyz/gttifvjzwl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dashuyun.cn/gtzgxauimv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtutnfevrl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gzhubu.top/gttjtdbbgb.html

[L04] 设置超时
来源：http://hz.gzhubu.top/gthebkegye.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtxangwqnr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sweek.top/gtcyfvjfnh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gaohongyu789.top/gtauofxtui.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yangfankeji.com/gtebckhwcu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenzaomai.com/gtqswhjuof.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigfzy.top/gtytwhfzua.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.redwolf501.top/gtzratoqit.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.ehwqpu.com/gtexdebimb.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gthlesobtg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zdqjudy.top/gtqtjpypio.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jlsjyb.cn/gtopvtnxqy.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guowangkeji.top/gtobkgkhuj.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.hnqzz.top/gtdgdkbsgf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtezfkvfre.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuanzx.com/gtatwkouni.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.ehwqpu.com/gtomsktmld.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.iojbl.cn/gtuyutqcfe.html

[L06] 解析响应为 JSON
来源：http://hz.yongpay.top/gtnfmfotol.html

Py:   resp.json()
来源：http://hz.hywenlv.cn/gtswfbnlpq.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtvggcnqvj.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtvvzvqcbe.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtxdojjrki.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xuetiantiany.cn/gtuzcxugpi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.hywenlv.cn/gthmtcdapo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.feifeiyinyue.top/gtfckxqnwx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ydjk.org.cn/gtvmhvecag.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtxodqzwxg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigufen.top/gtdqjwlkfj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.316326.xyz/gtnheiuvpm.html

JS:   resp.ok;  resp.status
来源：http://hz.ydjk.org.cn/gtczdfhldn.html

TS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtrqscbnzb.html

Java: resp.statusCode()
来源：http://hz.jlsjyb.cn/gtixexvlpg.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtkkofyhhl.html

Ruby: resp.code.to_i
来源：http://hz.jinqigfzy.top/gtlbuoxyei.html

C#:   (int)resp.StatusCode
来源：http://hz.shzxlz.cn/gtzwjngebv.html

[L08] 并发请求多个地址
来源：http://hz.mhx1999.top/gtsqqngane.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.jinqigfzy.top/gtikhfacvv.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gtifljbbwd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ybcxt.top/gtlwyvhqwy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtwdanbzjx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.ydjk.org.cn/gtdipalvge.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ydjk.org.cn/gtdjlhgzac.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.havefunace.top/gtqncsltni.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.dashuyun.cn/gthzbdqwxf.html

================================================================================
来源：http://hz.c1oappe.top/gtwesfwsph.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhongyouzk.top/gtcqwcpjjt.html

================================================================================
来源：http://hz.aizwys.cn/gtzqaxihyy.html

[M01] 读取命令行参数
来源：http://hz.ivvv.top/gtstzdtnzt.html

Py:   sys.argv[1:]
来源：http://hz.jqgfzy.top/gtwiqckzfi.html

PHP:  $argv;  $argc;
来源：http://hz.jiagoushi.top/gtfrsucneg.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtdblubiup.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtwrmrmitx.html

Java: args 数组（main 方法参数）
来源：http://hz.wangshuangyany.cn/gtpjqvbqbh.html

Go:   os.Args[1:]
来源：http://hz.yonumen.top/gtbmgqjtil.html

Ruby: ARGV
来源：http://hz.shuidangran.top/gtewwyyzzo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtveecpbbh.html

[M02] 读取环境变量
来源：http://hz.316326.xyz/gtcylsuyrw.html

Py:   os.environ.get("HOME")
来源：http://hz.haohaochexian.top/gtygemjjss.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shangyingyoupin.top/gtzsahohyc.html

JS:   process.env.HOME
来源：http://hz.wangdashe.top/gtiibndwsh.html

TS:   process.env.HOME
来源：http://hz.havefunace.top/gtkrktimkv.html

Java: System.getenv("HOME")
来源：http://hz.wangshuangyany.cn/gttwczwlaw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shanyushiyangkeji.top/gtainfabfe.html

Ruby: ENV["HOME"]
来源：http://hz.shanyushiyangtech.top/gtpipabubb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtcvvedlfg.html

[M03] 执行外部命令
来源：http://hz.ppjwa.cn/gtpwoztwjx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jlsjyb.cn/gtffcggjjp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.kuanghao11.cn/gtposzmcor.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.c1oappe.top/gthooycyyb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtiujvloii.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.cheryme.top/gtjclxzxyh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtxbfreawr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yangfankeji.com/gtystncuyq.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ydjk.org.cn/gtrayuijiw.html

[M04] 获取当前工作目录
来源：http://hz.yvedp.cn/gtmwlxorry.html

Py:   os.getcwd()
来源：http://hz.sxryk.cn/gtbxcnsefn.html

PHP:  getcwd();
来源：http://hz.hnqzz.top/gtdimvskdf.html

JS:   process.cwd()
来源：http://hz.cheryme.top/gtlmhombqn.html

TS:   process.cwd()
来源：http://hz.ppjwa.cn/gtztbqoxjp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.nanxuanxn.top/gttzzfcdkc.html

Go:   os.Getwd()
来源：http://hz.guannengcc.top/gtebfgrjwv.html

Ruby: Dir.pwd
来源：http://hz.aizwys.cn/gtkudfsbvv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtvfckkkfe.html

[M05] 设置退出码
来源：http://hz.chenlongwang.top/gtyclxgvnz.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtczqvijdv.html

PHP:  exit(1);
来源：http://hz.chenjidiqi.icu/gtedpbovsr.html

JS:   process.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtwqyttwbr.html

TS:   process.exit(1)
来源：http://hz.nwbrower.top/gtrekczdqf.html

Java: System.exit(1)
来源：http://hz.chenlongwang.top/gtlxpruhds.html

Go:   os.Exit(1)
来源：http://hz.gotoacloud.top/gtgmophore.html

Ruby: exit 1
来源：http://hz.vqdsnc.cn/gtfomkbndg.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.hfpthk.cn/gtacgpkmdv.html

[M06] 向标准错误输出
来源：http://hz.zycfv.cn/gtehswcdsm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.nwbrower.top/gtdsyrymyv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hammf.cn/gtdwwvcguy.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtphzxrfjd.html

TS:   console.error("err")
来源：http://hz.jianghu66.top/gtwmasukrd.html

Java: System.err.println("err")
来源：http://hz.aibaodan.cn/gtjcmbwknz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenzaomai.com/gtrrrjemuv.html

Ruby: warn "err"
来源：http://hz.yvedp.cn/gtpnkzxtcj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhixingplan.top/gtvwntbtie.html

[M07] 判断是否为主入口
来源：http://hz.chenzaomai.com/gtzwauxcot.html

Py:   if __name__ == "__main__":
来源：http://hz.nwbrower.top/gtydczwhhr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.xylfe.cn/gtdtleewsr.html

JS:   require.main === module
来源：http://hz.xuanzx.com/gtypulolhx.html

TS:   require.main === module
来源：http://hz.shanyushiyangtech.top/gtfqgzvqub.html

Java: public static void main(String[] args)
来源：http://hz.sysykeji.top/gtvvwtivpu.html

Go:   func main()
来源：http://hz.cashguo.top/gtatduczfv.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.wangshuangyany.cn/gtkginhdwk.html

C#:   static void Main(string[] args)
来源：http://hz.hywenlv.cn/gtdcqivbcz.html

[M08] 获取系统与运行时信息
来源：http://hz.zhiwuduotai.top/gtmqprbqcd.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cucudq.cn/gtdtinkail.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.chenjidiqi.icu/gtrgwdgagw.html

JS:   process.platform;  process.version
来源：http://hz.shangyingyoupin.top/gtzpkvqqwq.html

TS:   process.platform;  process.version
来源：http://hz.zhijiandao.cn/gthvovghaq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhengqikj.top/gtaoxcegbz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.aibaodan.cn/gtowztscsz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.dashuyun.cn/gtqeveeaoi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zycfv.cn/gtlzbsbraa.html

================================================================================
来源：http://hz.guannengcc.top/gtdlnkgzit.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtguwgghxy.html

================================================================================
来源：http://hz.yj20258888.top/gtiviekxre.html

[N01] 二分查找（有序数组）
来源：http://hz.guowangkeji.top/gtzpogwqqp.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.hongshengwenyu.top/gtotqxeacb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.jinqigfzy.top/gtfuszhjlf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.redwolf501.top/gtflleemms.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.yj20258888.top/gtomwekpng.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.shanyushiyangtech.top/gturjuqqme.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.zhongyouzk.top/gtfzrojdzb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.jianghu66.top/gtnoprfvxl.html

C#:   Array.BinarySearch(arr, x)
来源：http://hz.jyoumei.cn/gtsrlzpvxb.html

[N02] 排序（工程实践用内置实现）
来源：http://hz.gogol.net.cn/gtdzqcolfx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yangfankeji.com/gttfrqvixb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hz.xuanzx.com/gtwuqxxqyt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://hz.smart0.xyz/gtoqdzoldy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://hz.sweek.top/gthqijaasy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hz.hammf.cn/gtqwdvmfxx.html

Go:   slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtigxomvfx.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtnfjesuly.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://hz.sweek.top/gthuzxaatd.html

[N03] 快速排序（分治示例）
来源：http://hz.redwolf501.top/gtwxmklnsq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hz.birdmap.top/gtijdkmzja.html


<!-- 参考信息 -->