代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtkokfgyfo.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtdhempafk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnqzz.top/gtheflqpiw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gttnckjzhl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtqfwbkpus.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtpelndqbn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtuupxbtrc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gttvwyhfoh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.meibo888.top/gtbefziqeh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxinkj.top/gtxbuxwoqx.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtaqmafsmz.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gttebdhbqu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtqwhkbaam.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtlhbhlmam.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yvedp.cn/gtuxhlcbvq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gthdypgssa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gthqxorqsn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gttvqluqvs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.vqdsnc.cn/gtboelnpwr.html

[J06] 计算两时间之差
来源：http://hz.birdmap.top/gtmkawbghh.html

Py:   (end - start).total_seconds()
来源：http://hz.sufxvd.cn/gtmphnypxg.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtfuudkwui.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtitbyztjv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yonumen.top/gtjhfcybhe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtmfczxprs.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtiawgccaw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gthhzvqzfd.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtjamqlhdx.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtgystzcnq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtywxtuebj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.52xcode.cn/gtfpjexrut.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtmwiarmow.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtbgczwbui.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.pengpengdd.cyou/gtuxfiuamw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtkdipktqz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtxwwfxqge.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtsjfzqpgo.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtmvpecplj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtrngcbgzm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtohxuzjas.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuanzhike.top/gtlawlxjdi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gthycoifme.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gtbwmnjtmz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtcqiuhtaz.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtidjeczjv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtwnqrngov.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtgjecjkad.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gthatcyqcz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuanzx.com/gtzuevuvdh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtsyzwawir.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtgtsksbsc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtozvvcadm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shuidangran.top/gtbzhetevq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hongshengwenyu.top/gtcxurwizq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yvedp.cn/gtzrbrmmme.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinyuanbaomall.cn/gtdofojhge.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtxhkpaaxo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xziqi.cn/gtbtvuqnlh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtbojokxbx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtuwqswnbj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258888.top/gtspxozjxk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtdochfgrt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtzyoytmyw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtaspcznel.html

================================================================================
来源：http://hz.guowangkeji.top/gtknkltsun.html

K. JSON 与序列化
来源：http://hz.birdmap.top/gtfreogtpg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtjnoqyetz.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtvdlaqqpm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.meibo888.top/gtubsvwlix.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtvvxcxthz.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtejdxrnbp.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtxnewqqun.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtqpkdivtq.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtrntboubt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtxilcrqmu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtnkeruhha.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtmynlecnq.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtqczorihb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinghuilouyu.cn/gtlnrglweo.html

JS:   JSON.parse(s)
来源：http://hz.shuidangran.top/gtvgvburwx.html

TS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtctgfbhcf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yuanzhike.top/gtyvxxskwn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtlmelxbyy.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtrxydfuha.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gtrhmrodsa.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtzlhvwwul.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtawkspwna.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtktasrlho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gtksummgnn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtrexsfimo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangkeji.top/gtstyzwkse.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gtbkuklqwr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtuzaqrshi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtrpqgjypo.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtbvuawbwr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.birdmap.top/gtpbsdnmvc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.daria6918.cn/gtxyrhzxrb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gthnrjanfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtkzvhsbac.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cucudq.cn/gtdpzwgadv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtlexgbplu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ybcxt.top/gtvgxuwido.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtwdfhwtkk.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtoclgzbcv.html

Py:   copy.deepcopy(obj)
来源：http://hz.pengpengdd.cyou/gtsunbssgy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.sysykeji.top/gtzfbjxnwl.html

JS:   structuredClone(obj)
来源：http://hz.gzhubu.top/gtobhhydqv.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gttcsehbtd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pengpengdd.cyou/gtholhzmad.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cashguo.top/gtcjbhgmgd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtstymbzwo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yueranfly.top/gtaluucmdn.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtjdclkcwd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gthgafynpm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yueranfly.top/gtmuikcajy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tanke756.top/gtnstynamv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtjgybekaz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtfbqdilmz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtbahaqlga.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtyyfqgzmo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.shzxlz.cn/gtndmcsshw.html

[K07] 进制转换
来源：http://hz.xuetiantiany.cn/gtwyxmaqeq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtyqgbbzjx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gtilbkessj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtpzdrxbnz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtgreyfykt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtjdrzosqc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gogol.net.cn/gtjfkjoypx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenjidiqi.icu/gtqwdwvwsq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jianghu66.top/gtzroblbww.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnqzz.top/gtivqmoirr.html

Py:   pickle.dumps(obj)
来源：http://hz.meibo888.top/gtkcjecghd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.vqdsnc.cn/gthowdteaa.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtyhmepffw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.dianchejie.cn/gtrdxtqzcq.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cqqwz.cn/gtxdbkmnzt.html

Go:   encoding/gob
来源：http://hz.daria6918.cn/gthcutgnxw.html

Ruby: Marshal.dump(obj)
来源：http://hz.sysykeji.top/gtufxvhlky.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yonumen.top/gtmizcgyud.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtnlyphomu.html

L. 网络请求
来源：http://hz.ehwqpu.com/gtczgrxmop.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtwvqeirek.html

[L01] 发送 GET 请求
来源：http://hz.meibo888.top/gtcgzqlifx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.c1oappe.top/gtxmvbnzxz.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.316326.xyz/gtbvizdhff.html

JS:   await fetch(url)
来源：http://hz.ybcxt.top/gtkgmmaxfa.html

TS:   await fetch(url)
来源：http://hz.tianlin.xyz/gtwhjjlkxs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yonumen.top/gthcfzlwja.html

Go:   resp, err := http.Get(url)
来源：http://hz.chenlongwang.top/gtihidbhbb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jinqigfzy.top/gtrqeewxfj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gthuegseks.html

[L02] 发送 POST JSON
来源：http://hz.gzhubu.top/gtdkifdriv.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxuanxn.top/gtfojcsxtk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ybcxt.top/gtbmoxwuzm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.vqdsnc.cn/gtuwciugyk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gtwbfspsxq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtqbwkulzv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.andypj.xyz/gtsgklrzpv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xinyue.icu/gtanuohpdf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.aibaodan.cn/gtuhnoepek.html

[L03] 设置自定义请求头
来源：http://hz.haohaochexian.top/gtfljkexle.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zycfv.cn/gthbqkwifz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.meibo888.top/gtmgsftymf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtfaxmzbgv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtuhwvnows.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtrcwojeif.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.cheryme.top/gtvufuuhwe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtpqpednuf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.daxiang520.top/gtzwryzcfs.html

[L04] 设置超时
来源：http://hz.havefunace.top/gttnftnrbu.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtbkyjdbyu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.ehwqpu.com/gtesmrxmbm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuxming.cn/gtpzjfwxic.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yonumen.top/gtajxxfroc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.pengpengdd.cyou/gtaooxwstf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xuetiantiany.cn/gtqdncnfad.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.sweek.top/gtrwbgunrc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhongyouzk.top/gtvydarybt.html

[L05] 上传文件（multipart）
来源：http://hz.hywenlv.cn/gtpfkvjggm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yonumen.top/gtlcenewvr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtyoyzribl.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gttrtjmedd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhixingplan.top/gtjofkzwom.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xuetiantiany.cn/gtmzqdofyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.yvedp.cn/gtpgmaijxn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zhongyouzk.top/gtdljciuhw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.cqqwz.cn/gtgvkzvcih.html

[L06] 解析响应为 JSON
来源：http://hz.ybcxt.top/gtadwtjsrl.html

Py:   resp.json()
来源：http://hz.yonumen.top/gtvppdjata.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gteherllle.html

JS:   await resp.json()
来源：http://hz.jinyuanbaomall.cn/gtxszdozsm.html

TS:   await resp.json()
来源：http://hz.nanxinkj.top/gtrfipabdr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yanxiufei.cn/gtwkkbivzo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sxryk.cn/gthxyaslet.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgfzy.top/gtapnzevqa.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hnqzz.top/gtzaybumas.html

[L07] 处理 HTTP 状态码
来源：http://hz.jinyuanbaomall.cn/gtpkcjfgtw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.ybcxt.top/gtunogimjr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.cqqwz.cn/gtlhmjimdo.html

JS:   resp.ok;  resp.status
来源：http://hz.hammf.cn/gtslcmytes.html

TS:   resp.ok;  resp.status
来源：http://hz.ppjwa.cn/gtqlgjjduq.html

Java: resp.statusCode()
来源：http://hz.yonumen.top/gtmxeqmxgh.html

Go:   resp.StatusCode
来源：http://hz.snrcjt.cn/gtkopzblih.html

Ruby: resp.code.to_i
来源：http://hz.feifeiyinyue.top/gttuvnpruc.html

C#:   (int)resp.StatusCode
来源：http://hz.gzhubu.top/gtrjsrwikb.html

[L08] 并发请求多个地址
来源：http://hz.zhixingplan.top/gtfwhgulyr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ppjwa.cn/gtzpdysnsv.html

PHP:  curl_multi_init() 系列
来源：http://hz.hongshengwenyu.top/gtlcppwpgl.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.kuanghao11.cn/gtglgsksvt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.hfpthk.cn/gtyatuyqem.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xuanzx.com/gtrnwpurzj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.hywenlv.cn/gtciubvtvq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.shanyushiyangtech.top/gtlmqbubfr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jinghuilouyu.cn/gtdorvfvof.html

================================================================================
来源：http://hz.andypj.xyz/gtfymomocy.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangtech.top/gtumjtaauj.html

================================================================================
来源：http://hz.cheryme.top/gtwtvlfxsf.html

[M01] 读取命令行参数
来源：http://hz.snrcjt.cn/gtychkgczb.html

Py:   sys.argv[1:]
来源：http://hz.smart0.xyz/gtudoybhbq.html

PHP:  $argv;  $argc;
来源：http://hz.hywenlv.cn/gttzoojdlb.html

JS:   process.argv.slice(2)
来源：http://hz.svipenyu.cn/gtjiynlohl.html

TS:   process.argv.slice(2)
来源：http://hz.hysaishi.cn/gtzgvyoktz.html

Java: args 数组（main 方法参数）
来源：http://hz.yueranfly.top/gttmmltzfp.html

Go:   os.Args[1:]
来源：http://hz.smart0.xyz/gtfgzarjsy.html

Ruby: ARGV
来源：http://hz.bjfxy.top/gtwlgfduzl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.guannengcc.top/gtzmjmzpcu.html

[M02] 读取环境变量
来源：http://hz.fengsongda.top/gtzzbgoini.html

Py:   os.environ.get("HOME")
来源：http://hz.guannengcc.top/gtiyvjehsq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hfpthk.cn/gtsliacnqf.html

JS:   process.env.HOME
来源：http://hz.andypj.xyz/gttyzeqbhh.html

TS:   process.env.HOME
来源：http://hz.guowangkeji.top/gtybvjllau.html

Java: System.getenv("HOME")
来源：http://hz.haohaochexian.top/gtphwhuxhc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jinyuanbaomall.cn/gtwcwbdojx.html

Ruby: ENV["HOME"]
来源：http://hz.yongpay.top/gthtslbpos.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.hnxiangtu.top/gtpzbrauum.html

[M03] 执行外部命令
来源：http://hz.ybcxt.top/gtjewknvng.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.316326.xyz/gtzkllillj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.shzxlz.cn/gtzoereclx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.birdmap.top/gtzuzmiweu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.jinyuanbaomall.cn/gtfyuhzlgl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.gotoacloud.top/gtsgzgosol.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gthleiatcn.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.gotoacloud.top/gtoemiwrtu.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangdashe.top/gtomdorjny.html

[M04] 获取当前工作目录
来源：http://hz.jinqigufen.top/gttoglmvgh.html

Py:   os.getcwd()
来源：http://hz.jlsjyb.cn/gtavwnbibn.html

PHP:  getcwd();
来源：http://hz.tian-w.cn/gtinydvpem.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtmtvgmdxe.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtvfwgvqqz.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jinghuilouyu.cn/gtfysdnfue.html

Go:   os.Getwd()
来源：http://hz.zhiwuduotai.top/gthnolgcoc.html

Ruby: Dir.pwd
来源：http://hz.nanxinkj.top/gtlpkowrob.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jinyuanbaomall.cn/gtshoavalq.html

[M05] 设置退出码
来源：http://hz.jqgufenzy.top/gtklvcrtzm.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtdoxtzrxl.html

PHP:  exit(1);
来源：http://hz.xylfe.cn/gtsxnrsrwr.html

JS:   process.exit(1)
来源：http://hz.smart0.xyz/gtscjbzwbr.html

TS:   process.exit(1)
来源：http://hz.shuidangran.top/gtbnuzmjfx.html

Java: System.exit(1)
来源：http://hz.zhijiandao.cn/gtyzpioqfl.html

Go:   os.Exit(1)
来源：http://hz.hongshengwenyu.top/gtygmytzzi.html

Ruby: exit 1
来源：http://hz.cdnleiting.top/gtbrzehpzd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.yueranfly.top/gtcykvnbvf.html

[M06] 向标准错误输出
来源：http://hz.cucudq.cn/gtkdjhfxem.html

Py:   print("err", file=sys.stderr)
来源：http://hz.dianchejie.cn/gtolpgsgdb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ivvv.top/gtwjdikvyr.html

JS:   console.error("err")
来源：http://hz.birdmap.top/gtbqlppwlc.html

TS:   console.error("err")
来源：http://hz.nanxinkj.top/gtkpkiftat.html

Java: System.err.println("err")
来源：http://hz.smart0.xyz/gtdwthsqdz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhijiandao.cn/gttvpameog.html

Ruby: warn "err"
来源：http://hz.daxiang520.top/gtdsrvzmwx.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.fengsongda.top/gtnflknkhn.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtofmuqjxx.html

Py:   if __name__ == "__main__":
来源：http://hz.gaohongyu789.top/gtzbcnbbqc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.shzxlz.cn/gtafmnusyc.html

JS:   require.main === module
来源：http://hz.snrcjt.cn/gtajdijmbc.html

TS:   require.main === module
来源：http://hz.yangfankeji.com/gtfafwpmsd.html

Java: public static void main(String[] args)
来源：http://hz.jyoumei.cn/gtpmdhxbve.html

Go:   func main()
来源：http://hz.nwbrower.top/gtdmltilyh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.9152youxi.cn/gtmulgceim.html

C#:   static void Main(string[] args)
来源：http://hz.tianlin.xyz/gtucnuoeti.html

[M08] 获取系统与运行时信息
来源：http://hz.xingfuxueyuan.xyz/gtosbdhupg.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ehwqpu.com/gtyrpxkwda.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.dashuyun.cn/gthzlrkrrq.html

JS:   process.platform;  process.version
来源：http://hz.fengsongda.top/gtlbztyhdv.html

TS:   process.platform;  process.version
来源：http://hz.redwolf501.top/gtugnguffg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtybcosefp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.c1oappe.top/gtxjjxzums.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.aizwys.cn/gtghyyhacb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.daria6918.cn/gtobniwlpd.html

================================================================================
来源：http://hz.pycfn.com/gtnpnmabtc.html

N. 数据结构与算法
来源：http://hz.xuetiantiany.cn/gttoxesnxw.html

================================================================================
来源：http://hz.shzxlz.cn/gtvrzvmfwx.html

[N01] 二分查找（有序数组）
来源：http://hz.316326.xyz/gtzsoaehac.html

Py:   bisect.bisect_left(arr, x)
来源：http://hz.gzhubu.top/gtfzjkwgyr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hz.sweek.top/gtljjwmywf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.cashguo.top/gtkivkggbs.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hz.jqgfzy.top/gtrjjmctmd.html

Java: Arrays.binarySearch(arr, x)
来源：http://hz.jinghuilouyu.cn/gtymmldylp.html

Go:   sort.SearchInts(arr, x)
来源：http://hz.hnqzz.top/gtenrhfbjh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://hz.52xcode.cn/gtaxiookgk.html


<!-- 参考信息 -->