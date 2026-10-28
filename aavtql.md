代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtxmnmzklz.html

[J04] 时间戳与日期互转
来源：http://hz.ivvv.top/gtswnabcou.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtuzkgudoa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.tian-w.cn/gtfakjlzdb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtegdzfdrc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtdborrzak.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tanke756.top/gtkdszrwyi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtkykrephs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ehwqpu.com/gtzbnwvnwb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtrparpyba.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtgiudixsl.html

Py:   now + timedelta(days=7)
来源：http://hz.shuidangran.top/gtetouwdlj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtgdjnomuw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yanxiufei.cn/gtsztwpnxu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtvcvsdqba.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtivkimpna.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtrhwwjbwt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dianchejie.cn/gtpejmopbb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtqxjgxxvd.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gthaifdltj.html

Py:   (end - start).total_seconds()
来源：http://hz.cucudq.cn/gtpjogybmv.html

PHP:  $end->diff($start)->days;
来源：http://hz.mhx1999.top/gttxelzird.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtfafvrtwg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtebzferkp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gtwvrouvqw.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtonppgwdn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtzqvvvxxc.html

C#:   (end - start).TotalSeconds
来源：http://hz.hongshengwenyu.top/gtsdhcomuk.html

[J07] 比较两个日期
来源：http://hz.nanxuanxn.top/gtstdvuhtv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gttewoxros.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtbvchkmmr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtzmonoxct.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtsqrsdyoa.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.tian-w.cn/gtxziemrek.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtmmvgpfmm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtxuzihdho.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtvsgchvvm.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtfooymcqc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gterkeyugd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.andypj.xyz/gtcliejydy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258888.top/gttfzhrvbg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtakqwevbs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtoxlcndti.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gttlcohxhs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtoigiqxjb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtqhgspgqx.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtedimwigp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtbgpeyfxt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.daria6918.cn/gtyirvigzn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtburpsbjx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtjtlqpnoc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gthkwicduo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj20258888.top/gtztjenktz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtiidhhduu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxinkj.top/gtdumnrmbn.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtmyuvimzs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtcgpzbdur.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtbwuzzsel.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.9152youxi.cn/gtgnkrsfbv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtwvyywejb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtcjhmrled.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtcslfztvu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sysykeji.top/gtdsfqbwje.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.feifeiyinyue.top/gtkqrlagvn.html

================================================================================
来源：http://hz.ehwqpu.com/gtytkklxba.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gtsouyngiv.html

================================================================================
来源：http://hz.jiagoushi.top/gthsctizgm.html

[K01] 对象转 JSON 字符串
来源：http://hz.gotoacloud.top/gtqqslhfxe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.aibaodan.cn/gtibtlciks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtublfeixw.html

JS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtdblnmhry.html

TS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtawnnpnzp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtlxnqqmrn.html

Go:   json.Marshal(obj)
来源：http://hz.shangyingyoupin.top/gtotipmzho.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenzaomai.com/gtcrkanrjx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtgjargwfq.html

[K02] JSON 字符串转对象
来源：http://hz.haohaochexian.top/gtotyqqysg.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtwgktwfwn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tian-w.cn/gtqsjrfwtm.html

JS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtwgsojcoz.html

TS:   JSON.parse(s)
来源：http://hz.yanxiufei.cn/gttspbyaem.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtraftenpt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtzujzrxli.html

Ruby: JSON.parse(s)
来源：http://hz.andypj.xyz/gtusvsfvpv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtwaahmtjt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhengqikj.top/gtklpyivvq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtxnrcishi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtrzzmarxz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtffcsbmzq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gttwmssbfy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.birdmap.top/gthrtgswus.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtpvemuznx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gtwaibbsbx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ehwqpu.com/gtnsqscpef.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtpelbjczy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtpshpqthg.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtcyiqoish.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtonnubhvp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtelskvlcl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gteahrdxcg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xziqi.cn/gtevrhxzht.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.haohaochexian.top/gtorhkmsdf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dashuyun.cn/gtgjpntman.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gthyzrzfnx.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtkjvuvghm.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtjdpzjtjq.html

JS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtrwsambfz.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtyucfdtmn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxinkj.top/gtnqashywz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtuplccvgh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gzhubu.top/gteeqzxqkc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtohtuzwky.html

[K06] 解析 URL 查询串
来源：http://hz.feifeiyinyue.top/gtpghywcpz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtegokuity.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zdqjudy.top/gtzybxbywj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtoqofcynk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhixingplan.top/gtacpmyhmc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gtuocjiltp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hysaishi.cn/gtgglzfssg.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtuwkrmsii.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sxryk.cn/gtinipbngq.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtukkznuhl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtcdifnyav.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cqqwz.cn/gtcmxjikzm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gtvkvbzxeu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtzokcpodu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtmdtefthz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtxakmegwk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.wangshuangyany.cn/gtfaoagbcx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtrzfwyjfx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgufenzy.top/gthgfoyksm.html

Py:   pickle.dumps(obj)
来源：http://hz.ivvv.top/gtsgzuckcc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jlsjyb.cn/gtdqdostnu.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtazgqqazi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jqgfzy.top/gtyvaulkem.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xuanzx.com/gtxbigvruk.html

Go:   encoding/gob
来源：http://hz.ydjk.org.cn/gtrlcnntmu.html

Ruby: Marshal.dump(obj)
来源：http://hz.kuanghao11.cn/gtwruzhswc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cdnleiting.top/gtmwktfjsk.html

================================================================================
来源：http://hz.sxryk.cn/gtfmoqjahe.html

L. 网络请求
来源：http://hz.vqdsnc.cn/gtgjecsmgj.html

================================================================================
来源：http://hz.zycfv.cn/gtfouzhswm.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtjyuzbtlp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cdnleiting.top/gtvhtnkwwl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtnkdpryom.html

JS:   await fetch(url)
来源：http://hz.iojbl.cn/gtymqncwbr.html

TS:   await fetch(url)
来源：http://hz.bjfxy.top/gtwybzjpgx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jyoumei.cn/gtysrzhhmh.html

Go:   resp, err := http.Get(url)
来源：http://hz.yangfankeji.com/gtfgtjcjgc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.xingfuxueyuan.xyz/gtqwstzppx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.chenjidiqi.icu/gtqistmhzo.html

[L02] 发送 POST JSON
来源：http://hz.yj202588.top/gtlsyxlbdd.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.wangshuangyany.cn/gtgiabwlzz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yangfankeji.com/gtdvreqoop.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtovdzmoum.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gthujsubsg.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.shangyingyoupin.top/gtgwxwhjct.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.52xcode.cn/gtpguehkvq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gtmmwcewuy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigfzy.top/gtczfjwwbx.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtxbdmkwhr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ydjk.org.cn/gtipqorlmz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hywenlv.cn/gtzlefgwsu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.andypj.xyz/gtdfpwpyjj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtenmftjos.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhengqikj.top/gtzwruabxm.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenjidiqi.icu/gtkjtjmhyu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.snrcjt.cn/gtrbpropzn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtmsujdhpl.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtrwoiwaqn.html

Py:   requests.get(url, timeout=5)
来源：http://hz.jqgufenzy.top/gtjyayfnfg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jianghu66.top/gtgzhiqzma.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhoulong.xyz/gtglufnjra.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cqqwz.cn/gtcvhwpmvd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.cucudq.cn/gtqxphvcru.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.sweek.top/gtydhvagvy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cucudq.cn/gtnltabpgh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.xinyue.icu/gtjtcqvcab.html

[L05] 上传文件（multipart）
来源：http://hz.hysaishi.cn/gtxjyvkpgf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hongshengwenyu.top/gtlfwudkpn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ydzc1.top/gtddwozjgw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.cqqwz.cn/gtfndyitgm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gttbnchasd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangkeji.top/gturtsdcld.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gtmnurvvcc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.tianlin.xyz/gtovznangg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ehwqpu.com/gtogsagudv.html

[L06] 解析响应为 JSON
来源：http://hz.zhaomingkeji.xyz/gtxomxbdbe.html

Py:   resp.json()
来源：http://hz.hysaishi.cn/gtjkyqmiyk.html

PHP:  json_decode($body, true);
来源：http://hz.feifeiyinyue.top/gtoxapvmav.html

JS:   await resp.json()
来源：http://hz.jyoumei.cn/gtbkahwtht.html

TS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtishhypsn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dianchejie.cn/gtxknvwjhy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.ywan-chungtsiang.top/gtwstnvdtl.html

Ruby: JSON.parse(resp.body)
来源：http://hz.andypj.xyz/gtefdspngc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gthdjznghy.html

[L07] 处理 HTTP 状态码
来源：http://hz.yangfankeji.com/gtqgzzckdi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.cucudq.cn/gtmjbbpejr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gogol.net.cn/gtgxjsxyqw.html

JS:   resp.ok;  resp.status
来源：http://hz.yvedp.cn/gtbmbnnssl.html

TS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtotkjzibl.html

Java: resp.statusCode()
来源：http://hz.ppjwa.cn/gtmbmohlfs.html

Go:   resp.StatusCode
来源：http://hz.pengpengdd.cyou/gtvtdqfpjc.html

Ruby: resp.code.to_i
来源：http://hz.sweek.top/gtqycttaah.html

C#:   (int)resp.StatusCode
来源：http://hz.fzhhl.top/gtrvjbtgww.html

[L08] 并发请求多个地址
来源：http://hz.tianlin.xyz/gtvonhmigy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.sweek.top/gtisyhvpuk.html

PHP:  curl_multi_init() 系列
来源：http://hz.xingfuxueyuan.xyz/gtbwcgnljt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xylfe.cn/gtfcmsnegz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinghuilouyu.cn/gtoihqgsrj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yj20258.top/gtgwvfadqk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ywan-chungtsiang.top/gtvpqulggs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhiwuduotai.top/gtvebfwqan.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gotoacloud.top/gtumhhwvma.html

================================================================================
来源：http://hz.meibo888.top/gtbspovkpc.html

M. 命令行 / 进程 / 环境
来源：http://hz.andypj.xyz/gtfctiwlxh.html

================================================================================
来源：http://hz.yuxming.cn/gtkoeqqanb.html

[M01] 读取命令行参数
来源：http://hz.9152youxi.cn/gtuznfaijf.html

Py:   sys.argv[1:]
来源：http://hz.ybcxt.top/gtrbwflbxt.html

PHP:  $argv;  $argc;
来源：http://hz.shanyushiyangkeji.top/gtcnqrtggr.html

JS:   process.argv.slice(2)
来源：http://hz.guowangkeji.top/gtqkrgxgah.html

TS:   process.argv.slice(2)
来源：http://hz.redwolf501.top/gttiryblvs.html

Java: args 数组（main 方法参数）
来源：http://hz.mhx1999.top/gtcgykocpy.html

Go:   os.Args[1:]
来源：http://hz.xingfuxueyuan.xyz/gtufdtbkih.html

Ruby: ARGV
来源：http://hz.jyoumei.cn/gtuumtbjpk.html

C#:   args 数组（Main 方法参数）
来源：http://hz.smart0.xyz/gtrhxpycwd.html

[M02] 读取环境变量
来源：http://hz.nanxinkj.top/gtuymficty.html

Py:   os.environ.get("HOME")
来源：http://hz.chenlongwang.top/gtgvpoqojz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.chenlongwang.top/gtvealrsed.html

JS:   process.env.HOME
来源：http://hz.aibaodan.cn/gtonrkssyz.html

TS:   process.env.HOME
来源：http://hz.yj202588.top/gtslmeasvu.html

Java: System.getenv("HOME")
来源：http://hz.jinqigufen.top/gtluaoqflb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.pycfn.com/gtigmthtvc.html

Ruby: ENV["HOME"]
来源：http://hz.ehwqpu.com/gtazzcuysf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.cheryme.top/gtduxobwjr.html

[M03] 执行外部命令
来源：http://hz.dianchejie.cn/gtccasnwqn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.jinqigufen.top/gtcbakgmbo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.gogol.net.cn/gtgcgcomio.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtadhbtbuo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhengqikj.top/gtbrkzuorx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.vqdsnc.cn/gtaxttjocy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.redwolf501.top/gtyidgjvak.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtzclfhegm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.kuanghao11.cn/gtnrnscwdj.html

[M04] 获取当前工作目录
来源：http://hz.yj20258.top/gtiegwkkhe.html

Py:   os.getcwd()
来源：http://hz.yonumen.top/gtobiphkpx.html

PHP:  getcwd();
来源：http://hz.jqgfzy.top/gtzuuoqoas.html

JS:   process.cwd()
来源：http://hz.wangshuangyany.cn/gtgjscuhrn.html

TS:   process.cwd()
来源：http://hz.hysaishi.cn/gtugnsdkit.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xuanzx.com/gticdqwczx.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtcsryqrri.html

Ruby: Dir.pwd
来源：http://hz.zhengqikj.top/gthtqkzbex.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jiagoushi.top/gtmcxnhvud.html

[M05] 设置退出码
来源：http://hz.zhoulong.xyz/gtaedwpmef.html

Py:   sys.exit(1)
来源：http://hz.fengsongda.top/gtrdatffty.html

PHP:  exit(1);
来源：http://hz.dashuyun.cn/gttjsuyoku.html

JS:   process.exit(1)
来源：http://hz.meibo888.top/gtnyrwxkkg.html

TS:   process.exit(1)
来源：http://hz.jinqigfzy.top/gtztvxdsdh.html

Java: System.exit(1)
来源：http://hz.svipenyu.cn/gtlzacouwt.html

Go:   os.Exit(1)
来源：http://hz.9152youxi.cn/gtpmhyhgud.html

Ruby: exit 1
来源：http://hz.mhx1999.top/gtsrsisvki.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.jinqigufen.top/gtvmtadorn.html

[M06] 向标准错误输出
来源：http://hz.pengpengdd.cyou/gtrqdaeihm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.yonumen.top/gtcrtgryas.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hongshengwenyu.top/gthtqszngh.html

JS:   console.error("err")
来源：http://hz.xinyue.icu/gtnvcdtnjv.html

TS:   console.error("err")
来源：http://hz.sxryk.cn/gtthygwpmq.html

Java: System.err.println("err")
来源：http://hz.kuanghao11.cn/gtvwcnnfph.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhaomingkeji.xyz/gtlumyvzmq.html

Ruby: warn "err"
来源：http://hz.daria6918.cn/gtqwyijsld.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.chenzaomai.com/gtpwwrnwtl.html

[M07] 判断是否为主入口
来源：http://hz.jinqigufen.top/gthiblkror.html

Py:   if __name__ == "__main__":
来源：http://hz.daria6918.cn/gtyfwunddh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.redwolf501.top/gtdsqktxar.html

JS:   require.main === module
来源：http://hz.sufxvd.cn/gttmriuhyp.html

TS:   require.main === module
来源：http://hz.vqdsnc.cn/gtahyezdmb.html

Java: public static void main(String[] args)
来源：http://hz.jianghu66.top/gtxytosvbw.html

Go:   func main()
来源：http://hz.iojbl.cn/gtltkpvway.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.tanke756.top/gtncvttjta.html

C#:   static void Main(string[] args)
来源：http://hz.chenlongwang.top/gtumulogio.html

[M08] 获取系统与运行时信息
来源：http://hz.jinqigfzy.top/gtpekfcklp.html

Py:   platform.system();  platform.python_version()
来源：http://hz.zhaomingkeji.xyz/gtlwjpeblc.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.cqqwz.cn/gtifjawhir.html

JS:   process.platform;  process.version
来源：http://hz.cqqwz.cn/gtpngnhyai.html

TS:   process.platform;  process.version
来源：http://hz.cashguo.top/gtwlggjcwy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.chenzaomai.com/gtpukgzcjp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.zhixingplan.top/gtvaonexlj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.svipenyu.cn/gtzxiwcoui.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.cheryme.top/gtridjgmkc.html

================================================================================
来源：http://hz.mhx1999.top/gtvsvqkqxr.html

N. 数据结构与算法
来源：http://hz.tian-w.cn/gtgdwyvhgl.html

================================================================================
来源：http://hz.redwolf501.top/gtislfdhvg.html

[N01] 二分查找（有序数组）
来源：http://hz.cheryme.top/gtkoenjhsb.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.zhixingplan.top/gtxmfgikve.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.yongpay.top/gtcwhdugqk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.fzhhl.top/gtfqxjchdt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.sufxvd.cn/gtxizcamsa.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.zhongyouzk.top/gtvojfkwtz.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.feifeiyinyue.top/gttccldiee.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.sweek.top/gtopkexvtb.html


<!-- 参考信息 -->