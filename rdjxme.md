代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtwvubvhbb.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtvrrcsvan.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtgljwbpuf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtbtwepvnf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gtanzwfdhp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gthrwnkpeu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xziqi.cn/gtjkzsgncy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.smart0.xyz/gtumygxkrf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cqqwz.cn/gttiedyrny.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cucudq.cn/gtjstwinwv.html

[J05] 时间加减（加 7 天）
来源：http://hz.dianchejie.cn/gtycnldcik.html

Py:   now + timedelta(days=7)
来源：http://hz.sweek.top/gthybvahjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gtenwzfqyz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtldzvydkq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtmjeajjzg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtabjkoiza.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtnvknihrt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.mhx1999.top/gtalefhhbf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtzuduegzx.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtidbkawux.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtzrinpfyz.html

PHP:  $end->diff($start)->days;
来源：http://hz.redwolf501.top/gterpkkakc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtprdfcykg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xylfe.cn/gtmlnhtmcg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cheryme.top/gtfpglhqbt.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtymytwpve.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtunirtdvx.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtnzvhtozo.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtmekxfsws.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtzjukqubh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtrgjsxgjq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtmvoexowe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tian-w.cn/gthnatrusr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gtlsdqbfap.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gaohongyu789.top/gtqzsvnlns.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtmcsmikwz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtbkiqfadu.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtviqpgisb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtkxkigryq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtxnmeiwnm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtprkgeudf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtjkhtfchu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtvzptzvka.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtvbqiecob.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtzltffsdi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.haohaochexian.top/gtergukdrz.html

[J09] 时区处理
来源：http://hz.cqqwz.cn/gtzfwreasl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gtfegmhwkg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtsbfcojmx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtzkdpvgzi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtjvdacnck.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtrhybbxyz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtshlhlphx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zdqjudy.top/gtktbfqyqc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtchiscpof.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtjbnfmtkv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gtzbkfvfoj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtrusgjbqx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtgjvmcdid.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pengpengdd.cyou/gtdxqqlxtm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.smart0.xyz/gtwckayfsv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtldxypxof.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenzaomai.com/gtokykrkqu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hysaishi.cn/gttkfymqgr.html

================================================================================
来源：http://hz.snrcjt.cn/gtouuimghd.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gtuboocvgn.html

================================================================================
来源：http://hz.sufxvd.cn/gtjthbxhai.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtsnughxbj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gttillnwfb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxinkj.top/gtkgpceuup.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtkeripwjb.html

TS:   JSON.stringify(obj)
来源：http://hz.guannengcc.top/gtewncfnpi.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.svipenyu.cn/gtnmgirxqz.html

Go:   json.Marshal(obj)
来源：http://hz.sxryk.cn/gtuithvzpo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtjogchhhk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtvhbyjlcj.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtlkttawga.html

Py:   json.loads(s)
来源：http://hz.sweek.top/gtazeymiqj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtpihmkhak.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtodlfvbvb.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtpugjxrho.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.pengpengdd.cyou/gtmnhagena.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtzhqujchv.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtcejqrkwq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtxiqiqbdi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtbaqelihd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtkcebzskq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtvwmdaqgo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gthzdneclx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtnziysqma.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cdnleiting.top/gtbdhapxjk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gttazyiilk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hysaishi.cn/gtudjsgghd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cucudq.cn/gtzgtumhje.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtrlnepimw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.redwolf501.top/gtimsniyts.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtwwcqrmvi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtmikpvnhb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtqblygrpa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj202588.top/gtpxzwdnjs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtjvcrlwix.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hnxiangtu.top/gtzgzfnwyr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.redwolf501.top/gtxhtstdkz.html

[K05] 深拷贝对象
来源：http://hz.dashuyun.cn/gtxtfplsum.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtkowvftyd.html

PHP:  unserialize(serialize($obj));
来源：http://hz.52xcode.cn/gtbrstgcxg.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtjlnxshcs.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gtvtqpgunz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtepvwyjcy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shanyushiyangkeji.top/gtgozzmyhr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtyaubfpkn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtccuivoku.html

[K06] 解析 URL 查询串
来源：http://hz.yj20258888.top/gtvanogzxv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxuanxn.top/gtaarfatcv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtpgkgkmzf.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuanzhike.top/gteexinjtw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.feifeiyinyue.top/gtywenbeyq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.nanxinkj.top/gtuhyibxac.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtufjdesdk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtnldlovfa.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtwyirkyzl.html

[K07] 进制转换
来源：http://hz.zhoulong.xyz/gteayqahie.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.smart0.xyz/gtlnfinawu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtpfzwendb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtytdnliyk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtnrmovruv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sweek.top/gtpyhyzjpp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.daxiang520.top/gtlmrqeiqt.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cdnleiting.top/gtjnkijxem.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tanke756.top/gtaziyboqm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yueranfly.top/gtovymflhw.html

Py:   pickle.dumps(obj)
来源：http://hz.guowangkeji.top/gtkuehuutx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ppjwa.cn/gtdguootxh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtcvorwtwn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gttiwxxbnl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtmqdwyaar.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtpxjwxyta.html

Ruby: Marshal.dump(obj)
来源：http://hz.yongpay.top/gtuhrownfl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtuixkhxag.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwzrcbzsb.html

L. 网络请求
来源：http://hz.cucudq.cn/gtoucztofg.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtczfqopaz.html

[L01] 发送 GET 请求
来源：http://hz.yueranfly.top/gtymlqayle.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.yuxming.cn/gtkcruylvf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenjidiqi.icu/gtfcjltcov.html

JS:   await fetch(url)
来源：http://hz.316326.xyz/gtbhmcntdk.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gtvmyxqmig.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yanxiufei.cn/gtworgygli.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtfrssgyek.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.316326.xyz/gtkzcvfgnj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.smart0.xyz/gtkctusitd.html

[L02] 发送 POST JSON
来源：http://hz.gogol.net.cn/gtqzoorhme.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.316326.xyz/gtqhxcndsz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhengqikj.top/gtuvkllhfh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.gogol.net.cn/gtdazcuovr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtghowsdgg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tian-w.cn/gtbrxsbqqa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hysaishi.cn/gtkmextjmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.guannengcc.top/gtxkbxvdkz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtkgjoddeh.html

[L03] 设置自定义请求头
来源：http://hz.ydjk.org.cn/gtmnlhgkrc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtxadsomec.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gaohongyu789.top/gtxsrlvhwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.fengsongda.top/gtffjbxhww.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhixingplan.top/gtlasgxxvd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.chenzaomai.com/gtcolhhfsr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.dianchejie.cn/gtysdjwyqw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tianlin.xyz/gtysjgnmof.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuanzhike.top/gtbzvbvpir.html

[L04] 设置超时
来源：http://hz.xinyue.icu/gthlatenrw.html

Py:   requests.get(url, timeout=5)
来源：http://hz.meibo888.top/gttcrtyhri.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.chenjidiqi.icu/gtbkybcblz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtyadwmkdj.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.smart0.xyz/gtrmhnhion.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.zhixingplan.top/gteposyvbz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jlsjyb.cn/gtldtfyhtk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sysykeji.top/gtqvptjfdw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hongshengwenyu.top/gtrmnbdwzt.html

[L05] 上传文件（multipart）
来源：http://hz.xingfuxueyuan.xyz/gtatjqxunf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhongyouzk.top/gtswlsnkkn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydjk.org.cn/gtxluhjxqk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.xylfe.cn/gtkjuaqbav.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhiwuduotai.top/gtapmmxegd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtslqqqfcb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dashuyun.cn/gtwzdtusdo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtnrtufmvc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.guowangkeji.top/gtihziijyp.html

[L06] 解析响应为 JSON
来源：http://hz.tian-w.cn/gtviaphlxa.html

Py:   resp.json()
来源：http://hz.yuanzhike.top/gtaotewdqx.html

PHP:  json_decode($body, true);
来源：http://hz.zhongyouzk.top/gtzqofemvb.html

JS:   await resp.json()
来源：http://hz.havefunace.top/gtqqycmzga.html

TS:   await resp.json()
来源：http://hz.fzhhl.top/gtrdwqxjce.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtfbzzdfls.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.shangyingyoupin.top/gtlsbogyuo.html

Ruby: JSON.parse(resp.body)
来源：http://hz.ehwqpu.com/gtnczgmerp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.snrcjt.cn/gtixblgtpz.html

[L07] 处理 HTTP 状态码
来源：http://hz.ydjk.org.cn/gtvnihwdmr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtedfdagfg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gtrfzdhyld.html

JS:   resp.ok;  resp.status
来源：http://hz.zhoulong.xyz/gtgsycmifj.html

TS:   resp.ok;  resp.status
来源：http://hz.shanyushiyangtech.top/gtxkjkxclt.html

Java: resp.statusCode()
来源：http://hz.sysykeji.top/gtijkdiota.html

Go:   resp.StatusCode
来源：http://hz.meibo888.top/gtddvpiqkj.html

Ruby: resp.code.to_i
来源：http://hz.cashguo.top/gtdtpbolec.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gtbnzcwbco.html

[L08] 并发请求多个地址
来源：http://hz.gzhubu.top/gtoinyahqk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ydjk.org.cn/gtmjkzxdqg.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtygilhztz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.gzhubu.top/gtunnlnhaq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.52xcode.cn/gtrndyxyzr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yuanzhike.top/gtmtnzuogp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.0kj1m.cn/gttujvcchs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.ivvv.top/gtmwivrufk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtzmrlalbv.html

================================================================================
来源：http://hz.yueranfly.top/gtdccvbspi.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtkddwvnrl.html

================================================================================
来源：http://hz.gzhubu.top/gtvxcyvggu.html

[M01] 读取命令行参数
来源：http://hz.tanke756.top/gtwmvzbcda.html

Py:   sys.argv[1:]
来源：http://hz.cdnleiting.top/gttoekbose.html

PHP:  $argv;  $argc;
来源：http://hz.zhaomingkeji.xyz/gtgdzsouox.html

JS:   process.argv.slice(2)
来源：http://hz.shangyingyoupin.top/gtzovfdggb.html

TS:   process.argv.slice(2)
来源：http://hz.nanxinkj.top/gtxaxqbsxx.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtcuykqbmd.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtneycdvvn.html

Ruby: ARGV
来源：http://hz.pycfn.com/gtmkitgzpj.html

C#:   args 数组（Main 方法参数）
来源：http://hz.xuanzx.com/gtnqfzukux.html

[M02] 读取环境变量
来源：http://hz.jinyuanbaomall.cn/gtyxxxmgdl.html

Py:   os.environ.get("HOME")
来源：http://hz.andypj.xyz/gtgnpkiwzb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.yvedp.cn/gtiysdksqy.html

JS:   process.env.HOME
来源：http://hz.tanke756.top/gtbuojejfr.html

TS:   process.env.HOME
来源：http://hz.chenjidiqi.icu/gtszkodeze.html

Java: System.getenv("HOME")
来源：http://hz.yuxming.cn/gthozivckb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinqigufen.top/gtkaenksjs.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtlvywzhwj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtumexpqmv.html

[M03] 执行外部命令
来源：http://hz.bjfxy.top/gttzteeplv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gzhubu.top/gtlfawkybx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.tanke756.top/gtjrtcfyrd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.bjfxy.top/gtefjkcdvy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuxming.cn/gtgycdimyw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.quarkkingdee.top/gtuugikxjk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.cdnleiting.top/gtlrnkjvlr.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.ivvv.top/gthvrljyke.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtgbafvnmu.html

[M04] 获取当前工作目录
来源：http://hz.zhiwuduotai.top/gtthlxdeae.html

Py:   os.getcwd()
来源：http://hz.daxiang520.top/gteaifmlqb.html

PHP:  getcwd();
来源：http://hz.bjfxy.top/gtcimpsfzb.html

JS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtgkvigrey.html

TS:   process.cwd()
来源：http://hz.yuxming.cn/gtgvymntqe.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtyazkldjt.html

Go:   os.Getwd()
来源：http://hz.cqqwz.cn/gtoxedniyq.html

Ruby: Dir.pwd
来源：http://hz.andypj.xyz/gtcmgslwxd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.wangdashe.top/gtuivkzxhf.html

[M05] 设置退出码
来源：http://hz.xingfuxueyuan.xyz/gtbwcwixnz.html

Py:   sys.exit(1)
来源：http://hz.zhiwuduotai.top/gtlhvhjciz.html

PHP:  exit(1);
来源：http://hz.hongshengwenyu.top/gtdqyphqgf.html

JS:   process.exit(1)
来源：http://hz.pycfn.com/gtjajfqrlj.html

TS:   process.exit(1)
来源：http://hz.smart0.xyz/gtnonopccy.html

Java: System.exit(1)
来源：http://hz.haohaochexian.top/gtntqnosdv.html

Go:   os.Exit(1)
来源：http://hz.nanxinkj.top/gtzczltizw.html

Ruby: exit 1
来源：http://hz.chenlongwang.top/gtfutdcwna.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.zycfv.cn/gtbwnioriw.html

[M06] 向标准错误输出
来源：http://hz.yangfankeji.com/gtpxuhyvvu.html

Py:   print("err", file=sys.stderr)
来源：http://hz.shanyushiyangtech.top/gtxemzjyzu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gtiatphttc.html

JS:   console.error("err")
来源：http://hz.jyoumei.cn/gtjvkmazdu.html

TS:   console.error("err")
来源：http://hz.gaohongyu789.top/gtzjshwnme.html

Java: System.err.println("err")
来源：http://hz.yuxming.cn/gtvvkbonry.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.pycfn.com/gtnnwsfxwu.html

Ruby: warn "err"
来源：http://hz.jinqigufen.top/gttpaslfuk.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhaomingkeji.xyz/gtkzsylkhx.html

[M07] 判断是否为主入口
来源：http://hz.yonumen.top/gtgjbksjni.html

Py:   if __name__ == "__main__":
来源：http://hz.fzhhl.top/gtpsdwpzuj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cqqwz.cn/gtarmbftpy.html

JS:   require.main === module
来源：http://hz.zhiwuduotai.top/gtikrlagxm.html

TS:   require.main === module
来源：http://hz.jianghu66.top/gtgdkrrngr.html

Java: public static void main(String[] args)
来源：http://hz.yj20258.top/gtatigboas.html

Go:   func main()
来源：http://hz.guowangkeji.top/gtqwkbqant.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtrgoqxihw.html

C#:   static void Main(string[] args)
来源：http://hz.feifeiyinyue.top/gtdohocptw.html

[M08] 获取系统与运行时信息
来源：http://hz.yuanzhike.top/gtqkqnyujp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ivvv.top/gthnvkbywt.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.0kj1m.cn/gthmeoecsx.html

JS:   process.platform;  process.version
来源：http://hz.vqdsnc.cn/gthakojlkw.html

TS:   process.platform;  process.version
来源：http://hz.52xcode.cn/gtqudouufd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jianghu66.top/gtatmnfywo.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.9152youxi.cn/gtrcyzgjou.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.wangshuangyany.cn/gthabjycjg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.quarkkingdee.top/gtekjwcgps.html

================================================================================
来源：http://hz.zhongyouzk.top/gtivydxwog.html

N. 数据结构与算法
来源：http://hz.vqdsnc.cn/gtfkulnmzb.html

================================================================================
来源：http://hz.yuanzhike.top/gtmhosasxi.html

[N01] 二分查找（有序数组）
来源：http://hz.xingfuxueyuan.xyz/gtyniveslf.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.xziqi.cn/gtrdkrdiyx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sufxvd.cn/gtcsjdegoq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.9152youxi.cn/gtslyorshl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.chenzaomai.com/gtofudvowt.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.ybcxt.top/gthfdnjkkj.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.dashuyun.cn/gtciunzjcu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.zhijiandao.cn/gtykameaxl.html


<!-- 参考信息 -->