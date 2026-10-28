代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.tian-w.cn/gtplnqrnlv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fzhhl.top/gtutzgyvmx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtkdmrjcxk.html

JS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtmszbvysa.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtnbyveytp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtdaiwneca.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gogol.net.cn/gtgduftchn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtfinshhdq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtwykorvoh.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtthtgnapw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.haohaochexian.top/gtnzhmlwhb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.quarkkingdee.top/gtsoeywdaf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cashguo.top/gtlrvmqofu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtwonlyeof.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtyuhzaxdm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shuidangran.top/gtucbobjwd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtgdlrlakf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gtszzrazyg.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtavdjplmi.html

Py:   now + timedelta(days=7)
来源：http://hz.sxryk.cn/gttrtfxzuq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtapizzbzr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtknyguwtb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtroeaoypp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtcbfsdpge.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtxupmlecq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtyuxkvctp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtngzreklq.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtwzmilxlq.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gthzflxamk.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtfytdiysb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj202588.top/gtuutexzma.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gtnbrjcwdc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hywenlv.cn/gtghhvhiwm.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuetiantiany.cn/gtkvtafhyo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtytxjdylb.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtutdaqgsa.html

[J07] 比较两个日期
来源：http://hz.daria6918.cn/gtqktyoflp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gtupljjnyt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gticcwuvjp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnxiangtu.top/gtdqygfqst.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtbvflknpw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.52xcode.cn/gtbwnhfvrh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.kuanghao11.cn/gtbmvxlfip.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtdofzcwws.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtzhthdbni.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gthchjqest.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gtsquhmfoa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxinkj.top/gtfwfrjvxl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtashtnduo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sysykeji.top/gtmbkxrrey.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtsbfxyulm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtdjohsbkl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtvdrtchmy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtsghwcgwc.html

[J09] 时区处理
来源：http://hz.ppjwa.cn/gtbojtwdxd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhengqikj.top/gtvcbrskic.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hammf.cn/gtnlfeqley.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtpmtuoyxq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtfqvqyzfh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtrymqfvsq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yonumen.top/gthywcrbfr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenlongwang.top/gtjzqfbigi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtcimevrvw.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtvmwlltda.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtolwomzae.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtcxlqzaeq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtwmujppbz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gtfjbmgmde.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtqugphvag.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zycfv.cn/gtrtoywzdg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zycfv.cn/gtwfelegxn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gttgjdaacl.html

================================================================================
来源：http://hz.jinqigufen.top/gtebcuwfui.html

K. JSON 与序列化
来源：http://hz.jqgufenzy.top/gtwohxzoym.html

================================================================================
来源：http://hz.haohaochexian.top/gtnndsfqtp.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtycetuocs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtganusmsl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtpcpseznv.html

JS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtmalwxetd.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtghgxdsba.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtaxrvlnxz.html

Go:   json.Marshal(obj)
来源：http://hz.quarkkingdee.top/gtsrjhsqux.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtuconhbxd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tianlin.xyz/gtdfpiozob.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtdeifztfu.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtbftiltma.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxuanxn.top/gttpjgspmc.html

JS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtgmbjivzk.html

TS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtptfvlnoz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtsxbqgthu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gtyfziurbu.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gttmpnbzou.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhijiandao.cn/gtqurnffmn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.9152youxi.cn/gtfdorqwzp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtzwdgfuyo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtbwxikpbn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtibejnhtp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtifehkxbt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ivvv.top/gtxkmgeuyp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.quarkkingdee.top/gtfuqetncv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gtrnunqzsq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.bjfxy.top/gtxyowipux.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtgkenyjam.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jlsjyb.cn/gtxdqwrzyj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xinyue.icu/gtgcvjsdtk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtveymslyp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtfkysukff.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shangyingyoupin.top/gtllpfrzgt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtkifmnshg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pengpengdd.cyou/gtqblfdcco.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhijiandao.cn/gthdtyanqu.html

[K05] 深拷贝对象
来源：http://hz.ydzc1.top/gtrcqrvifq.html

Py:   copy.deepcopy(obj)
来源：http://hz.daria6918.cn/gtqrmdamgw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gttuosocwa.html

JS:   structuredClone(obj)
来源：http://hz.316326.xyz/gtopjvamuh.html

TS:   structuredClone(obj)
来源：http://hz.haohaochexian.top/gtsyurkoic.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.wangdashe.top/gtjmeigldo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtwhbdhfyq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtbgzsjuzo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yangfankeji.com/gtmdlveehz.html

[K06] 解析 URL 查询串
来源：http://hz.shuidangran.top/gtpvpwfmpp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xingfuxueyuan.xyz/gtssjkzjqw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtuupmbgmk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtudhbtxir.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtyexulltp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cqqwz.cn/gtgkkddujn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtamgnwoum.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yongpay.top/gtmnkhmhjr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtcuitsxwk.html

[K07] 进制转换
来源：http://hz.hfpthk.cn/gtvxfvpypj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtcwbdedsj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ivvv.top/gtzukycssu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtgyyaxbus.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtmapfvund.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtpdanfwth.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xuetiantiany.cn/gteghsaqdv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dianchejie.cn/gtyejmnlqo.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.guannengcc.top/gthjovqplh.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtfnvhbtok.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtahdvdhng.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yanxiufei.cn/gtlnwqmlei.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtqxcxfiwp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtceacjtxx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenzaomai.com/gtbctkhvfn.html

Go:   encoding/gob
来源：http://hz.jinghuilouyu.cn/gtrytogmpt.html

Ruby: Marshal.dump(obj)
来源：http://hz.jqgufenzy.top/gthmpnfjlb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.316326.xyz/gtcomkmekb.html

================================================================================
来源：http://hz.quarkkingdee.top/gtdaacobup.html

L. 网络请求
来源：http://hz.bjfxy.top/gtnyyfvvgq.html

================================================================================
来源：http://hz.svipenyu.cn/gtoabfznri.html

[L01] 发送 GET 请求
来源：http://hz.wangshuangyany.cn/gtmrtcfhtv.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cucudq.cn/gtjcoqierj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnqzz.top/gtchhncfpd.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtwrazvqdr.html

TS:   await fetch(url)
来源：http://hz.ivvv.top/gtbivzhgau.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ywan-chungtsiang.top/gtfifboqwp.html

Go:   resp, err := http.Get(url)
来源：http://hz.sxryk.cn/gthahnvijg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhixingplan.top/gtvyygukjs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.dashuyun.cn/gtzanogjme.html

[L02] 发送 POST JSON
来源：http://hz.wangshuangyany.cn/gtelcgmfut.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinghuilouyu.cn/gtmzwxbfdm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xuetiantiany.cn/gtjmctrafu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nwbrower.top/gtnfmuvndr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.svipenyu.cn/gtctjouucx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydjk.org.cn/gttfsgabkp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhongyouzk.top/gtxsvejzst.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tanke756.top/gteppljreu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtjjdmzjje.html

[L03] 设置自定义请求头
来源：http://hz.shuidangran.top/gtngbfujcd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtssjaqfbr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.dashuyun.cn/gtldnynpcx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gteagcldzy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.0kj1m.cn/gtmdjyoufp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.birdmap.top/gtzbgnafuh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hongshengwenyu.top/gtwwhgpioz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.wangshuangyany.cn/gtgqwwfmku.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtjhvdvgho.html

[L04] 设置超时
来源：http://hz.jianghu66.top/gtcxvsgtmh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.zhongyouzk.top/gtqtgefqqx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ydjk.org.cn/gtetfjjydv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtwyncanmb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtxtfbriir.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gaohongyu789.top/gtptsnrepa.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.ywan-chungtsiang.top/gtvbxuxnbv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtsdhjmrho.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.gotoacloud.top/gtfvbcudvm.html

[L05] 上传文件（multipart）
来源：http://hz.shangyingyoupin.top/gtzknvnlqc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.kuanghao11.cn/gtcwzgizkl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhijiandao.cn/gtkhrwcpuz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenlongwang.top/gtgivfllyd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.dashuyun.cn/gtxoqqqoxs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gtczrhoppm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.xuetiantiany.cn/gtfzrpqavn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.mhx1999.top/gtrabpufqp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxuanxn.top/gtwikdaxel.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtzpghsuah.html

Py:   resp.json()
来源：http://hz.aizwys.cn/gtnewqzenb.html

PHP:  json_decode($body, true);
来源：http://hz.gaohongyu789.top/gtxzpspvkv.html

JS:   await resp.json()
来源：http://hz.xylfe.cn/gtwjnkudpj.html

TS:   await resp.json()
来源：http://hz.quarkkingdee.top/gtekcyelvo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.feifeiyinyue.top/gtqigzoyar.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.chenzaomai.com/gtzqhnkran.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuanzhike.top/gtjuxvfvyl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.kuanghao11.cn/gtogafzzic.html

[L07] 处理 HTTP 状态码
来源：http://hz.sweek.top/gtwvpgvnux.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.sufxvd.cn/gteomhmzxc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.sxryk.cn/gthndvhfjf.html

JS:   resp.ok;  resp.status
来源：http://hz.zdqjudy.top/gtfpjnrqko.html

TS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gteexvyhdw.html

Java: resp.statusCode()
来源：http://hz.yongpay.top/gtwtmrbcnl.html

Go:   resp.StatusCode
来源：http://hz.ybcxt.top/gtxfbdkbss.html

Ruby: resp.code.to_i
来源：http://hz.yuxming.cn/gthgivrorr.html

C#:   (int)resp.StatusCode
来源：http://hz.ydjk.org.cn/gthgcbkofx.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtocoweryk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.chenlongwang.top/gtqatyhedd.html

PHP:  curl_multi_init() 系列
来源：http://hz.vqdsnc.cn/gtchcxifps.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.feifeiyinyue.top/gtqhnpvtro.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtfwkjecsd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.andypj.xyz/gtlfsptbyy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtapqemsxi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.wangshuangyany.cn/gtmcqjkngj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.tanke756.top/gtngaphfdb.html

================================================================================
来源：http://hz.zhoulong.xyz/gtfdglhssu.html

M. 命令行 / 进程 / 环境
来源：http://hz.yuanzhike.top/gtuxxboteg.html

================================================================================
来源：http://hz.fzhhl.top/gtwhfuchyr.html

[M01] 读取命令行参数
来源：http://hz.xuetiantiany.cn/gtwnvucabm.html

Py:   sys.argv[1:]
来源：http://hz.sxryk.cn/gtjkkepfou.html

PHP:  $argv;  $argc;
来源：http://hz.sufxvd.cn/gtbmsdfjdq.html

JS:   process.argv.slice(2)
来源：http://hz.haohaochexian.top/gtzxbkiwir.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtszqstoqb.html

Java: args 数组（main 方法参数）
来源：http://hz.dashuyun.cn/gtvabmsjex.html

Go:   os.Args[1:]
来源：http://hz.mhx1999.top/gtcwekmmte.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtkcbthdyy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.wangshuangyany.cn/gtjrqsdpor.html

[M02] 读取环境变量
来源：http://hz.xylfe.cn/gttbyxuynq.html

Py:   os.environ.get("HOME")
来源：http://hz.cheryme.top/gtnllapeyj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtwrxtbyuw.html

JS:   process.env.HOME
来源：http://hz.haohaochexian.top/gtgclwfabu.html

TS:   process.env.HOME
来源：http://hz.cucudq.cn/gtocyekteh.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtgkinxzqm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtblzhvlzu.html

Ruby: ENV["HOME"]
来源：http://hz.hnxiangtu.top/gtepgsyrmq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.wangdashe.top/gtfkwjxnqx.html

[M03] 执行外部命令
来源：http://hz.meibo888.top/gtyngsrqpi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sweek.top/gtvzncpyel.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.zhijiandao.cn/gtnabyhghd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.nwbrower.top/gtpjajrdtl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.xylfe.cn/gtbghvloki.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yueranfly.top/gtsfgjbujp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.wangdashe.top/gttvscijft.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.vqdsnc.cn/gtbwmqfcqb.html

C#:   Process.Start("ls", "-l");
来源：http://hz.shuidangran.top/gtnnjyszsi.html

[M04] 获取当前工作目录
来源：http://hz.bjfxy.top/gtfookfhdh.html

Py:   os.getcwd()
来源：http://hz.hammf.cn/gtqhromduy.html

PHP:  getcwd();
来源：http://hz.jiagoushi.top/gtvqstxdcl.html

JS:   process.cwd()
来源：http://hz.zhoulong.xyz/gtdixvwxzr.html

TS:   process.cwd()
来源：http://hz.gogol.net.cn/gtqxtdlgoa.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.chenlongwang.top/gtwtynbain.html

Go:   os.Getwd()
来源：http://hz.yueranfly.top/gtmiukeqna.html

Ruby: Dir.pwd
来源：http://hz.zhixingplan.top/gtfpkdrhfl.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtmboccagg.html

[M05] 设置退出码
来源：http://hz.havefunace.top/gtkbwwcorb.html

Py:   sys.exit(1)
来源：http://hz.yuanzhike.top/gtyabnbget.html

PHP:  exit(1);
来源：http://hz.yuxming.cn/gtshwqpjru.html

JS:   process.exit(1)
来源：http://hz.guowangkeji.top/gtftftgxlp.html

TS:   process.exit(1)
来源：http://hz.jyoumei.cn/gtainepnhn.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtsvrjmszd.html

Go:   os.Exit(1)
来源：http://hz.zhoulong.xyz/gtyliotgxg.html

Ruby: exit 1
来源：http://hz.dianchejie.cn/gtlcolkljp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.sufxvd.cn/gtgfovljuq.html

[M06] 向标准错误输出
来源：http://hz.xziqi.cn/gtzwtldmlb.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtdosyfxvo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.meibo888.top/gtbsfoxtte.html

JS:   console.error("err")
来源：http://hz.yanxiufei.cn/gtvycolsyp.html

TS:   console.error("err")
来源：http://hz.pengpengdd.cyou/gtsmddmini.html

Java: System.err.println("err")
来源：http://hz.jinyuanbaomall.cn/gtmtifzttq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.redwolf501.top/gtqivxbakg.html

Ruby: warn "err"
来源：http://hz.redwolf501.top/gtzvlzrilj.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.ywan-chungtsiang.top/gthmugncwf.html

[M07] 判断是否为主入口
来源：http://hz.hfpthk.cn/gtuzrlshbk.html

Py:   if __name__ == "__main__":
来源：http://hz.xinyue.icu/gtxxxoorot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jqgfzy.top/gtdzkakhed.html

JS:   require.main === module
来源：http://hz.birdmap.top/gtlrgfjlev.html

TS:   require.main === module
来源：http://hz.feifeiyinyue.top/gttgbvhhxv.html

Java: public static void main(String[] args)
来源：http://hz.yanxiufei.cn/gtepsjpyup.html

Go:   func main()
来源：http://hz.nwbrower.top/gtqxmtoyxg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.jinqigufen.top/gtvvltwdvs.html

C#:   static void Main(string[] args)
来源：http://hz.yueranfly.top/gtvwxfefah.html

[M08] 获取系统与运行时信息
来源：http://hz.smart0.xyz/gtucxzluly.html

Py:   platform.system();  platform.python_version()
来源：http://hz.jianghu66.top/gtemdiwtkv.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.c1oappe.top/gtakkzbxhv.html

JS:   process.platform;  process.version
来源：http://hz.ydjk.org.cn/gtvtxsltje.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtsdnnuquz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.zhaomingkeji.xyz/gtknxcdecd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.yj20258888.top/gtpxdmmbnz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.snrcjt.cn/gtsexfdrad.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.yanxiufei.cn/gtppmyvgnj.html

================================================================================
来源：http://hz.andypj.xyz/gtaskerqrd.html

N. 数据结构与算法
来源：http://hz.feifeiyinyue.top/gtktlknvsy.html

================================================================================
来源：http://hz.daria6918.cn/gtsenidbhy.html


<!-- 参考信息 -->