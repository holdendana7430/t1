代发 wailian999

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gtjlhnicca.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtgsncfkkl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtugucbavl.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtwziczifq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtbjyruzjh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuanzhike.top/gtcwfvdsgh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtldioatfu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtftnbihqk.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtiyppdsxy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtvpflltjk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtxfxseonz.html

JS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtgqdsblsc.html

TS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtfucoznye.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtrgtnhxxh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtvaanaxgw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gthsaatanv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtdcyifmly.html

[J04] 时间戳与日期互转
来源：http://hz.xuetiantiany.cn/gtnntkxkff.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhiwuduotai.top/gtqhwszkwl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ywan-chungtsiang.top/gtsezjagqt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtovenvklv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gtkmgqomly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtrgxcwsdr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.bjfxy.top/gtzbnyncbf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hammf.cn/gtlqcsetbn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtbcgxyago.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtsgruacwy.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigfzy.top/gtrsmgnhac.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.smart0.xyz/gtjsxxnokl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtzzcplncg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtlowfutel.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtewjhtglg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtchaovwfa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gtyupxdbxf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtbbduvbbd.html

[J06] 计算两时间之差
来源：http://hz.sysykeji.top/gtzyydhaxw.html

Py:   (end - start).total_seconds()
来源：http://hz.0kj1m.cn/gtbydolexy.html

PHP:  $end->diff($start)->days;
来源：http://hz.snrcjt.cn/gtfzghssoh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtgfexgiyd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtlemdngon.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtlijeflqe.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gtmemponqv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258.top/gtfckyhzve.html

C#:   (end - start).TotalSeconds
来源：http://hz.aizwys.cn/gtbnwtvkiu.html

[J07] 比较两个日期
来源：http://hz.zhongyouzk.top/gtvupmceky.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtyxrtemdn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sxryk.cn/gtxhxtluto.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gteiwnwbas.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtlqfmtetu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daxiang520.top/gtwwxydgfy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtnuxarcpt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtwazhmdwj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtwmqbajsv.html

[J08] 提取年月日与星期
来源：http://hz.andypj.xyz/gtgebfxnnt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtwnlyuouh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtlgkcbmnh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtijnjpoau.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtxqqkefgd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtdueyecqa.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gteeneukts.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gttrxardjx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtdxubfmgi.html

[J09] 时区处理
来源：http://hz.feifeiyinyue.top/gtxudzfkgk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gthrreaqbh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cqqwz.cn/gtrplxzhdt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtnozdmwoy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtpfyurfvp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.vqdsnc.cn/gtdmgakbst.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnqzz.top/gtocsjrwxe.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtalnyewtb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtxoeirunl.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtxgbowzqd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.kuanghao11.cn/gtmshbptwf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtigymtuml.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gttudiuwqv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtfkuybdpn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jqgfzy.top/gtzjfpkycg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtimggruxy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtjzabijpf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtarenijks.html

================================================================================
来源：http://hz.cashguo.top/gtlgwuyrjp.html

K. JSON 与序列化
来源：http://hz.xinyue.icu/gtuqkwgirl.html

================================================================================
来源：http://hz.jinqigufen.top/gtcardzzsz.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtdwaodmtr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtglxjvrcq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gteafdyvaq.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtzitgvqyc.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtgwhxgdtz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtbrggpdbe.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtioigngui.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtvzauxlxi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtqtazokra.html

[K02] JSON 字符串转对象
来源：http://hz.jlsjyb.cn/gtwzecwwlk.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gthovzsgnn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtfukoxuep.html

JS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtkevnxpzy.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtdywygbal.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gtyxguntjc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtkjhnzfla.html

Ruby: JSON.parse(s)
来源：http://hz.ppjwa.cn/gtdzsiccpt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shangyingyoupin.top/gtpbqwnbyv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xingfuxueyuan.xyz/gtymxzidzk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtnmpewbjg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sufxvd.cn/gtzvtdsnxk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtgxtsvkrk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtwrcpxvvo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtymqhfhxw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.snrcjt.cn/gtxfhpfptf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gotoacloud.top/gtntwipvpf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtkrygoton.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtdusgxuqv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gtpddbkzpr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.tanke756.top/gtkuwbrtop.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtxvnaysyd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtngvqihkc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtvufunucf.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtgpbngnlp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtdhjjmfqo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtrcdjssgr.html

[K05] 深拷贝对象
来源：http://hz.xziqi.cn/gtblsjpqxa.html

Py:   copy.deepcopy(obj)
来源：http://hz.cqqwz.cn/gtirqcrzzo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtfxdhygrk.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtcgjgdrvp.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtuegazhxo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tian-w.cn/gtworzgdim.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.c1oappe.top/gtrgjclzye.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gtjrzrpwss.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtivmqvcth.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gthqyenuew.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gtwvpzwbmb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gthwbhwsuq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.dashuyun.cn/gtympgaibe.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtzwykkfks.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtraftbjhh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ybcxt.top/gtvjkgsyjv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtvuiakjaz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtcvosobsq.html

[K07] 进制转换
来源：http://hz.meibo888.top/gtawxixtxs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.meibo888.top/gtallvestp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.daria6918.cn/gtdducdhyn.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sufxvd.cn/gtdbrdpmah.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtqjmevwvs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtpqoktgoc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtmbmknmzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zhoulong.xyz/gtbwoftmxz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhixingplan.top/gtfmlogkrc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtcveoofxe.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtykcbugll.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.nwbrower.top/gtdfbgekhb.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zycfv.cn/gtnehfptbm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gthckccdtm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtqvyhadon.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtwcftjaid.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtpvfipxwt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fzhhl.top/gtdhnnwtjx.html

================================================================================
来源：http://hz.jinqigufen.top/gtiorlikzh.html

L. 网络请求
来源：http://hz.316326.xyz/gtxrmwlywl.html

================================================================================
来源：http://hz.hnxiangtu.top/gthpbcjmmj.html

[L01] 发送 GET 请求
来源：http://hz.hnxiangtu.top/gtviudhyyt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtwlkdjcvb.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.nwbrower.top/gtvqtazxmr.html

JS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtbnhdjdqn.html

TS:   await fetch(url)
来源：http://hz.feifeiyinyue.top/gtrwhgeour.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gtvtuinqdk.html

Go:   resp, err := http.Get(url)
来源：http://hz.hongshengwenyu.top/gtvmmhvvsg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yj202588.top/gtgasrkddr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hongshengwenyu.top/gtlkbgxshd.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtlraptavx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zdqjudy.top/gtlswfzybm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cqqwz.cn/gtuffqcvhw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jyoumei.cn/gtbvpkelsp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuanzx.com/gtwswobotz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guowangkeji.top/gtetbxfpxg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.sufxvd.cn/gtapzmvbve.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nanxuanxn.top/gtexqwjbjf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.0kj1m.cn/gtjazuduat.html

[L03] 设置自定义请求头
来源：http://hz.jlsjyb.cn/gtgmlkxlcd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.sweek.top/gtaxfqtskl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zhengqikj.top/gthitdeosc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtmpahfhua.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yj20258888.top/gtouurksqa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhijiandao.cn/gthpyixedu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhixingplan.top/gtniqjogph.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.0kj1m.cn/gtoaxdmjtc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.bjfxy.top/gtwlbgiobo.html

[L04] 设置超时
来源：http://hz.smart0.xyz/gtrsguywdn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yj20258888.top/gtezseagcq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.daria6918.cn/gtbcdjulfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtqfgceeqz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.sxryk.cn/gtfevjbypc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sxryk.cn/gtsnjhfmql.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.snrcjt.cn/gtjjnzugmd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.dianchejie.cn/gtogthozhd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.andypj.xyz/gtylomuuni.html

[L05] 上传文件（multipart）
来源：http://hz.snrcjt.cn/gtsrvdhvjt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.smart0.xyz/gtvforetwv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.xingfuxueyuan.xyz/gtymtllaqw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gteixzsasn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.yanxiufei.cn/gtspgyxlpb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ybcxt.top/gtwpoznysc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.zhijiandao.cn/gtprcmpaca.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhiwuduotai.top/gtnkzprikx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtlpelxpcc.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gtugsfcyes.html

Py:   resp.json()
来源：http://hz.9152youxi.cn/gtvdxxmeek.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtohgcopwv.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtmgmschvz.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtkdxcszcx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.feifeiyinyue.top/gtmtebemvj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtzdcggfiz.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtmotywqph.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.tanke756.top/gtgxxprdvq.html

[L07] 处理 HTTP 状态码
来源：http://hz.daria6918.cn/gtlhaidfgx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.haohaochexian.top/gtyiatojws.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtdnwwnewb.html

JS:   resp.ok;  resp.status
来源：http://hz.hysaishi.cn/gteryhhrqx.html

TS:   resp.ok;  resp.status
来源：http://hz.chenzaomai.com/gtcwvsrsuw.html

Java: resp.statusCode()
来源：http://hz.sufxvd.cn/gtkaacoidh.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtqljnhwpl.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtmkrpprnn.html

C#:   (int)resp.StatusCode
来源：http://hz.yvedp.cn/gtiuprmekk.html

[L08] 并发请求多个地址
来源：http://hz.jlsjyb.cn/gtilnukpdu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.havefunace.top/gtuhwiqkvj.html

PHP:  curl_multi_init() 系列
来源：http://hz.shanyushiyangtech.top/gtjcsidcrn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuetiantiany.cn/gtdhaifaxd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.svipenyu.cn/gtfcsbvjey.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.c1oappe.top/gtflefpzyj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.pengpengdd.cyou/gtbdbhdtuz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.smart0.xyz/gtuhaaufix.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj20258888.top/gtuxtvakcv.html

================================================================================
来源：http://hz.haohaochexian.top/gttrmtpscq.html

M. 命令行 / 进程 / 环境
来源：http://hz.jlsjyb.cn/gtbebscmag.html

================================================================================
来源：http://hz.jiagoushi.top/gtecjekdut.html

[M01] 读取命令行参数
来源：http://hz.dianchejie.cn/gtvzllfdrv.html

Py:   sys.argv[1:]
来源：http://hz.pengpengdd.cyou/gtlcacarva.html

PHP:  $argv;  $argc;
来源：http://hz.yvedp.cn/gttpbehppf.html

JS:   process.argv.slice(2)
来源：http://hz.zhongyouzk.top/gtvvempybf.html

TS:   process.argv.slice(2)
来源：http://hz.fzhhl.top/gtjutfwbss.html

Java: args 数组（main 方法参数）
来源：http://hz.yangfankeji.com/gtlffsypxy.html

Go:   os.Args[1:]
来源：http://hz.zhiwuduotai.top/gtbbhsylzb.html

Ruby: ARGV
来源：http://hz.pengpengdd.cyou/gtvkrxikrv.html

C#:   args 数组（Main 方法参数）
来源：http://hz.quarkkingdee.top/gtsvbjhvxd.html

[M02] 读取环境变量
来源：http://hz.redwolf501.top/gtnpjioafy.html

Py:   os.environ.get("HOME")
来源：http://hz.jinqigufen.top/gtleqmmqqq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.pengpengdd.cyou/gtfmxxwcgs.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gtbtueiehw.html

TS:   process.env.HOME
来源：http://hz.hongshengwenyu.top/gthoknnqce.html

Java: System.getenv("HOME")
来源：http://hz.yvedp.cn/gtnnrhxzwf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.nanxuanxn.top/gttgwpnpia.html

Ruby: ENV["HOME"]
来源：http://hz.zhixingplan.top/gtwzmgwohy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.haohaochexian.top/gtfgnnauip.html

[M03] 执行外部命令
来源：http://hz.yj20258.top/gthlylhwvf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.pycfn.com/gthkekcaxl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cdnleiting.top/gtrrydxjac.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.feifeiyinyue.top/gtraahfrqu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinqigufen.top/gtlkscqwpo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.aizwys.cn/gtwnlgpeim.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtwopahtco.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zycfv.cn/gtpyoygohx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.pycfn.com/gtrajtjjfo.html

[M04] 获取当前工作目录
来源：http://hz.guowangkeji.top/gtbpqbtncp.html

Py:   os.getcwd()
来源：http://hz.jqgfzy.top/gtsmkmgyam.html

PHP:  getcwd();
来源：http://hz.fengsongda.top/gtkfjsycyh.html

JS:   process.cwd()
来源：http://hz.andypj.xyz/gtdwwundad.html

TS:   process.cwd()
来源：http://hz.jlsjyb.cn/gtxrcrkjdq.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhongyouzk.top/gtmrvxvccu.html

Go:   os.Getwd()
来源：http://hz.c1oappe.top/gtyspeehhx.html

Ruby: Dir.pwd
来源：http://hz.chenzaomai.com/gtntqcdtgd.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yongpay.top/gtiagwjiff.html

[M05] 设置退出码
来源：http://hz.yuxming.cn/gtshuuwnng.html

Py:   sys.exit(1)
来源：http://hz.hywenlv.cn/gtqspqeshq.html

PHP:  exit(1);
来源：http://hz.jqgfzy.top/gtjplkmsyu.html

JS:   process.exit(1)
来源：http://hz.zhiwuduotai.top/gtbjefndlj.html

TS:   process.exit(1)
来源：http://hz.zhixingplan.top/gtvuygzhca.html

Java: System.exit(1)
来源：http://hz.shanyushiyangkeji.top/gtihvtcnhk.html

Go:   os.Exit(1)
来源：http://hz.ivvv.top/gtuyjbguzf.html

Ruby: exit 1
来源：http://hz.yj20258.top/gtngmrpnjr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.haohaochexian.top/gtyirrzxiv.html

[M06] 向标准错误输出
来源：http://hz.zycfv.cn/gtibnyqadw.html

Py:   print("err", file=sys.stderr)
来源：http://hz.zhiwuduotai.top/gtqzojjgyo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.aizwys.cn/gtwvgbxcby.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtzilktyng.html

TS:   console.error("err")
来源：http://hz.jiagoushi.top/gtxenfsskj.html

Java: System.err.println("err")
来源：http://hz.tianlin.xyz/gtyhqeayxk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jinyuanbaomall.cn/gtkppydmls.html

Ruby: warn "err"
来源：http://hz.xingfuxueyuan.xyz/gtgfpuonag.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.nanxinkj.top/gtjxbitqbc.html

[M07] 判断是否为主入口
来源：http://hz.gzhubu.top/gtmpcnhuss.html

Py:   if __name__ == "__main__":
来源：http://hz.guannengcc.top/gtvhtlyhti.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.wangdashe.top/gtamebxfte.html

JS:   require.main === module
来源：http://hz.shzxlz.cn/gtnwksiqye.html

TS:   require.main === module
来源：http://hz.tanke756.top/gtqinoxjzo.html

Java: public static void main(String[] args)
来源：http://hz.quarkkingdee.top/gtaqtpaflu.html

Go:   func main()
来源：http://hz.shzxlz.cn/gtufjzyonr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.aizwys.cn/gtyliaszmz.html

C#:   static void Main(string[] args)
来源：http://hz.nanxuanxn.top/gthpcnwvqz.html

[M08] 获取系统与运行时信息
来源：http://hz.ppjwa.cn/gtvmvioqnn.html

Py:   platform.system();  platform.python_version()
来源：http://hz.quarkkingdee.top/gtjmiwawnz.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yj202588.top/gtbcnjxbqm.html

JS:   process.platform;  process.version
来源：http://hz.chenlongwang.top/gtplhgduzz.html


<!-- 参考信息 -->