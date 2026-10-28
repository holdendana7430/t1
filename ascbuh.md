代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.jinqigfzy.top/gtwvcasfrb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtsgqwnaha.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtbsrpxqkg.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtvgnfvibo.html

TS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtuzmrotgt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtliiybgdh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daria6918.cn/gtrnppnvgm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gthtsdfatk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtlcxogqzv.html

[J04] 时间戳与日期互转
来源：http://hz.shangyingyoupin.top/gtuqdnifbv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gtzkjetwnp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258888.top/gtwjctjlzb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtxihrvaky.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtypgzjdlh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.316326.xyz/gtdhjrlmmv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gthvphyfjl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtworlivue.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtdtquvmxt.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtcwpjaxbi.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtqnilkisq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtzfnayxgx.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jyoumei.cn/gttbapyukj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtcctdwkie.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgufenzy.top/gtxmyeoalx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gttshpznft.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtdxptiisy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aizwys.cn/gtrqlselzo.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtofwyshps.html

Py:   (end - start).total_seconds()
来源：http://hz.redwolf501.top/gtyyvqlepq.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtvtwksbbh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtygokdnvc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.birdmap.top/gtqptrqasr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtpsjftovo.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtdwbumjcz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtdujfwwmw.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtssgijyhr.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtspclfyrp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtwzikykuz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtpulvyugu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtynhlnimr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtkgrbumxf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtwtvlawjr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtogjgtkhf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtfzotfpkx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtkzpybdul.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtihtvpwml.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.feifeiyinyue.top/gtntlgfswt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gthicvpfgt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pengpengdd.cyou/gtozivgvgj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtfcilwzcz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gttnqtyenx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtootufpqy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guannengcc.top/gtidnsybyz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtjselttfa.html

[J09] 时区处理
来源：http://hz.andypj.xyz/gtxolhjaqn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydzc1.top/gtykvevteb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtqrcwbyxl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtducxwoyb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtnydhzomf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinyuanbaomall.cn/gtlcbxvtbb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nwbrower.top/gtotokvyyv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtpvmgvxvu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenlongwang.top/gtoofsvaut.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtcplyrgrq.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zycfv.cn/gtoudfgtsu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258.top/gtzmnnjwdl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtrnmdxrot.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.smart0.xyz/gtwmwcarbj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gthhygwmkp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtkkwndhsn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gtvfhmunsr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.316326.xyz/gtqrguebvf.html

================================================================================
来源：http://hz.vqdsnc.cn/gtrcfirfjc.html

K. JSON 与序列化
来源：http://hz.chenlongwang.top/gtjcwrpneb.html

================================================================================
来源：http://hz.ybcxt.top/gtosfrdone.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtonvyszle.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtsfevuwgu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtebscehbv.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtacuywsvs.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtgdeniytg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ydzc1.top/gtfwoyfxum.html

Go:   json.Marshal(obj)
来源：http://hz.xuanzx.com/gtwjsxrqbe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtodpmmjqv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.mhx1999.top/gtnysacdip.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtcnxnihvl.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gtsxopzrgg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtddvmxwzx.html

JS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gthweuuymh.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtuhqqftju.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtcpdcvezp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gthoipfsql.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtflpzxukl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tanke756.top/gtrkmpeywn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtchaeaplv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gtvcnrnstw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fzhhl.top/gtyaqyiuhd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtjartpeyi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtroefmuok.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gthimxzrej.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tian-w.cn/gtqewpjuhq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtagodywtr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtdvobtypm.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gttnawhvhw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtnkawoosi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtdrycqewh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtcptphryy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shuidangran.top/gtuzjbdtnq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtrvnolytl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cashguo.top/gtrqckbtzq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtyeqqcklt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shangyingyoupin.top/gtupsijffn.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtivddchab.html

Py:   copy.deepcopy(obj)
来源：http://hz.yuanzhike.top/gtzcwfpsjc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hongshengwenyu.top/gtrkczoezz.html

JS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtekeudetl.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtylvxnhgv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtdwtsdzmz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtuvbgzpcn.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhongyouzk.top/gtarouqyth.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cdnleiting.top/gtajkupfmg.html

[K06] 解析 URL 查询串
来源：http://hz.c1oappe.top/gtqfrtxeps.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aibaodan.cn/gtiiyzqusc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtngwoaolv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtrtcfhvdz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtvnfilbiu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shzxlz.cn/gtvugazitr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtwknvofkf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.mhx1999.top/gtdlwnwfbu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtogdawbut.html

[K07] 进制转换
来源：http://hz.andypj.xyz/gtbdcvmjvx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gttefadnev.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ppjwa.cn/gtmxyzewhf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtxnxaodqt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtfgtgsiqu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtyllvhsew.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtpnjhecah.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xinyue.icu/gtgqjungas.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.feifeiyinyue.top/gtzrnjwdjk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtyiczlwrw.html

Py:   pickle.dumps(obj)
来源：http://hz.gogol.net.cn/gttegskfpy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.quarkkingdee.top/gttjmxfvqc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtzransxnj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ivvv.top/gtwyhuwhua.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtljubgwwz.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtjvzleeuu.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtvvuvnhfz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.quarkkingdee.top/gtonpwqyex.html

================================================================================
来源：http://hz.dianchejie.cn/gtfbbkqqdy.html

L. 网络请求
来源：http://hz.birdmap.top/gtvcngewxl.html

================================================================================
来源：http://hz.sufxvd.cn/gttqxcpbqa.html

[L01] 发送 GET 请求
来源：http://hz.havefunace.top/gtlckdpcmu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gturelagnk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yonumen.top/gtmljzooib.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gttnnczjkl.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtrvelubdk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtagnaifqg.html

Go:   resp, err := http.Get(url)
来源：http://hz.xuetiantiany.cn/gtfqxaurgo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhoulong.xyz/gtpordrjpg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jqgfzy.top/gtbzuukxru.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtunkbcacu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.hfpthk.cn/gtozxlzjwj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.hongshengwenyu.top/gtydonvobh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtbcoiibyx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangtech.top/gtqnkeqkjm.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.guannengcc.top/gtfqipgbuq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.fzhhl.top/gtlszfphht.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gthhlhxhfe.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtgsndonri.html

[L03] 设置自定义请求头
来源：http://hz.kuanghao11.cn/gtlphzkmob.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.daria6918.cn/gtaomxgtrq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gturjajgne.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.316326.xyz/gtvhibcuyi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jyoumei.cn/gttainrfix.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.mhx1999.top/gtxsclogca.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.havefunace.top/gtqcmsubnv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yanxiufei.cn/gtuctovsnf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.52xcode.cn/gtqtbxepdb.html

[L04] 设置超时
来源：http://hz.pengpengdd.cyou/gtbvrszkqs.html

Py:   requests.get(url, timeout=5)
来源：http://hz.cheryme.top/gtjwpymkjd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhijiandao.cn/gtrsqzzcac.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ydjk.org.cn/gtejuujsll.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jqgufenzy.top/gtazjojtro.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.iojbl.cn/gtylgpmudu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.tian-w.cn/gttgvhbawo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.shanyushiyangtech.top/gtqcwpasar.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gtfvjpcnqa.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtzivbdshy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.guowangkeji.top/gttmkvfylr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.jqgufenzy.top/gtderqjfwd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtjnktxoti.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.0kj1m.cn/gtibphmvgj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ivvv.top/gtkequbajp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.tianlin.xyz/gtnzpoeepe.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.shanyushiyangtech.top/gteakhshhq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.nanxinkj.top/gtojrynuik.html

[L06] 解析响应为 JSON
来源：http://hz.jinqigfzy.top/gtuuwnsqdk.html

Py:   resp.json()
来源：http://hz.ybcxt.top/gtvecwmslx.html

PHP:  json_decode($body, true);
来源：http://hz.jinghuilouyu.cn/gtbmyzhgxp.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtvgqplkcv.html

TS:   await resp.json()
来源：http://hz.yonumen.top/gtevndstzq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.guowangkeji.top/gtdndxhtlz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtsloywary.html

Ruby: JSON.parse(resp.body)
来源：http://hz.hnxiangtu.top/gtfbponlxt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.pengpengdd.cyou/gtagolooyo.html

[L07] 处理 HTTP 状态码
来源：http://hz.kuanghao11.cn/gtjrfvrkun.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.nwbrower.top/gtvrmqdgtp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gttrwuiehj.html

JS:   resp.ok;  resp.status
来源：http://hz.jinqigufen.top/gtsiauacev.html

TS:   resp.ok;  resp.status
来源：http://hz.birdmap.top/gtcjvcvgyc.html

Java: resp.statusCode()
来源：http://hz.shanyushiyangtech.top/gtutbresda.html

Go:   resp.StatusCode
来源：http://hz.hongshengwenyu.top/gtldinecls.html

Ruby: resp.code.to_i
来源：http://hz.xuetiantiany.cn/gtvponxsqd.html

C#:   (int)resp.StatusCode
来源：http://hz.dashuyun.cn/gthxqdmxtq.html

[L08] 并发请求多个地址
来源：http://hz.sysykeji.top/gtiyvfbxdg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.svipenyu.cn/gtkokwojki.html

PHP:  curl_multi_init() 系列
来源：http://hz.gzhubu.top/gtstmriuxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hammf.cn/gtmvcqxsjp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xuanzx.com/gtyrgoqdfs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.guannengcc.top/gtsqczwtyk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cdnleiting.top/gtbwouzxqk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.yongpay.top/gtbyjoenug.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.yj202588.top/gtnrgyyhsd.html

================================================================================
来源：http://hz.tian-w.cn/gtqrzryrzo.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtnbovbktz.html

================================================================================
来源：http://hz.c1oappe.top/gtgyrugqmh.html

[M01] 读取命令行参数
来源：http://hz.nwbrower.top/gtgsflgbme.html

Py:   sys.argv[1:]
来源：http://hz.xuetiantiany.cn/gtwobfpfrx.html

PHP:  $argv;  $argc;
来源：http://hz.chenzaomai.com/gtzfeutclz.html

JS:   process.argv.slice(2)
来源：http://hz.shuidangran.top/gtmgjuzwwn.html

TS:   process.argv.slice(2)
来源：http://hz.xylfe.cn/gtoipepouy.html

Java: args 数组（main 方法参数）
来源：http://hz.zhoulong.xyz/gttuqlokps.html

Go:   os.Args[1:]
来源：http://hz.c1oappe.top/gtntmhlrkb.html

Ruby: ARGV
来源：http://hz.kuanghao11.cn/gtgwacxiyp.html

C#:   args 数组（Main 方法参数）
来源：http://hz.gotoacloud.top/gtuxullygz.html

[M02] 读取环境变量
来源：http://hz.cashguo.top/gthbtviprg.html

Py:   os.environ.get("HOME")
来源：http://hz.ydzc1.top/gtvrpposvy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.tanke756.top/gtighwckii.html

JS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtqnulkvhs.html

TS:   process.env.HOME
来源：http://hz.316326.xyz/gtccpxwnty.html

Java: System.getenv("HOME")
来源：http://hz.pengpengdd.cyou/gtyhozagnc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.shangyingyoupin.top/gtxirfzdnp.html

Ruby: ENV["HOME"]
来源：http://hz.gogol.net.cn/gtbbtkwicq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.nanxuanxn.top/gtpgaqpfwd.html

[M03] 执行外部命令
来源：http://hz.jinghuilouyu.cn/gtaftkcuku.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.birdmap.top/gtusawgmqk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cheryme.top/gtvslcrnuq.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yuanzhike.top/gtjezkyqvp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ydzc1.top/gtuypvxexr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.fzhhl.top/gtowoyzrlf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.feifeiyinyue.top/gtelvslkep.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yanxiufei.cn/gtvdtbczyx.html

C#:   Process.Start("ls", "-l");
来源：http://hz.nanxuanxn.top/gtzxjyelfb.html

[M04] 获取当前工作目录
来源：http://hz.xuetiantiany.cn/gtrnjosdyb.html

Py:   os.getcwd()
来源：http://hz.0kj1m.cn/gtplqqfidv.html

PHP:  getcwd();
来源：http://hz.smart0.xyz/gtlzwmopcx.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtceoeatbm.html

TS:   process.cwd()
来源：http://hz.xuetiantiany.cn/gtomtrpdpm.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.zhiwuduotai.top/gtlkglbflf.html

Go:   os.Getwd()
来源：http://hz.sweek.top/gtmqweqnok.html

Ruby: Dir.pwd
来源：http://hz.gogol.net.cn/gtrfsrbohx.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.snrcjt.cn/gtovcommhd.html

[M05] 设置退出码
来源：http://hz.jlsjyb.cn/gtydhkibjz.html

Py:   sys.exit(1)
来源：http://hz.wangshuangyany.cn/gtfqhjphsu.html

PHP:  exit(1);
来源：http://hz.yonumen.top/gtechywmwg.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtgcyfuwhs.html

TS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtimlcgaqo.html

Java: System.exit(1)
来源：http://hz.shangyingyoupin.top/gttbkluvxr.html

Go:   os.Exit(1)
来源：http://hz.ywan-chungtsiang.top/gtknlendqk.html

Ruby: exit 1
来源：http://hz.hnxiangtu.top/gtuhjjhkhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.xingfuxueyuan.xyz/gtolfwpere.html

[M06] 向标准错误输出
来源：http://hz.iojbl.cn/gtfdmyiwji.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ybcxt.top/gtifzrjzbs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yonumen.top/gtpnorvabu.html

JS:   console.error("err")
来源：http://hz.xuetiantiany.cn/gtqjczkjaq.html

TS:   console.error("err")
来源：http://hz.zhiwuduotai.top/gtszqbaivt.html

Java: System.err.println("err")
来源：http://hz.ydzc1.top/gtjhpsggvc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.jlsjyb.cn/gtwpwoxhtg.html

Ruby: warn "err"
来源：http://hz.yangfankeji.com/gtsodqudxc.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.jinqigufen.top/gtuahbazws.html

[M07] 判断是否为主入口
来源：http://hz.nanxinkj.top/gtzhoptvzj.html

Py:   if __name__ == "__main__":
来源：http://hz.daxiang520.top/gtdtjdbmcp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.316326.xyz/gtgxuyzrcs.html

JS:   require.main === module
来源：http://hz.iojbl.cn/gtczkkljck.html

TS:   require.main === module
来源：http://hz.dashuyun.cn/gtxfoosoch.html

Java: public static void main(String[] args)
来源：http://hz.cucudq.cn/gthruucyrp.html

Go:   func main()
来源：http://hz.sxryk.cn/gtmtxtmkek.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cucudq.cn/gtboswfuph.html

C#:   static void Main(string[] args)
来源：http://hz.sweek.top/gtspaxsskm.html

[M08] 获取系统与运行时信息
来源：http://hz.birdmap.top/gtkvuhuulu.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fengsongda.top/gtmwtgpnzp.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cheryme.top/gtkecbrnbx.html

JS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtuyhvmxwn.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtzsaawzau.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.xinyue.icu/gtuthdjkaa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.shzxlz.cn/gtvjbdmdkk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.hnxiangtu.top/gtfcadzqsu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.xinyue.icu/gtpcevskbm.html

================================================================================
来源：http://hz.gzhubu.top/gtvbdknhts.html

N. 数据结构与算法
来源：http://hz.pycfn.com/gtbqhjsaoa.html

================================================================================
来源：http://hz.ivvv.top/gtmwtpczlq.html


<!-- 参考信息 -->