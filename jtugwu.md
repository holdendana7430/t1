代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtpcwhqegu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuetiantiany.cn/gtpgqolrhk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gttcftxpfl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gttadhnlzg.html

[J03] 字符串解析为日期
来源：http://hz.zhiwuduotai.top/gtakcnrzaf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jlsjyb.cn/gtggabtoxl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtzetuowtp.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtxlfgfipa.html

TS:   new Date("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtnyocvbyi.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtigpjbral.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtcomxkwmp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sweek.top/gtfivgewmg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gtogkuggxr.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtcwkoewqt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtdwuavpbp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zdqjudy.top/gtjrurezsf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtdwmpreeh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gzhubu.top/gtrduupsoe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtdkhhxxqq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtepahnbau.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgfzy.top/gtsdywmneq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gthlwcahms.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydjk.org.cn/gtfrxinmbj.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gthgiqokyz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tianlin.xyz/gtuyjwygnt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtzztbfkzl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtmtycartw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.birdmap.top/gtlaumrxfi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtkttqyyhl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sysykeji.top/gtpjmmavaw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtolwivslb.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtlfpuvpcv.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtwvagwcvh.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtdrypjyys.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yvedp.cn/gtvydorydc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtkdqalpta.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gthhvhkphj.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtvzqmqrqc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gthpeqgcdq.html

C#:   (end - start).TotalSeconds
来源：http://hz.guannengcc.top/gtfhtjksda.html

[J07] 比较两个日期
来源：http://hz.zycfv.cn/gtgefvsoml.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gthjbcethd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtxyzxkrrq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtstqixvdj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtudtsirgc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtgzmdygqu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtxtlucrki.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtxsvrjtwy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gthjajejfo.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtnhutxhum.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtmalrtqrw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jyoumei.cn/gttomlhmqx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtcopojlmd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtzvcisqdc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigufen.top/gtsixilhqm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ehwqpu.com/gtueismdga.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gtuleijiru.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtokbacmos.html

[J09] 时区处理
来源：http://hz.sweek.top/gthtdiyjrw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.c1oappe.top/gtlmgyrpww.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gtihtrvcji.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtzdrmuqqn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gthbuqvvkh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtywhxapao.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aizwys.cn/gtqldpkksl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sweek.top/gtwylxtioe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gtdoxjgyql.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gthmqypuka.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtenyilptg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gttnprkosl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtgiejzyub.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtkayoehhp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj202588.top/gtxjjxuajz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jianghu66.top/gtcergbzlm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gtdvaydxes.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtfeaiteav.html

================================================================================
来源：http://hz.smart0.xyz/gtjanopami.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gterjijrlz.html

================================================================================
来源：http://hz.snrcjt.cn/gtscuzpida.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtpwygswnp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtaokmkgnq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtdzeqbcmn.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtivberppo.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtvzwhpqkw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtvpinpthd.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtwdayrdvk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangshuangyany.cn/gtyfldeijy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtbohewqqi.html

[K02] JSON 字符串转对象
来源：http://hz.iojbl.cn/gtwthihtcp.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangkeji.top/gtissqnscy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydzc1.top/gtdfbwsblq.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtdnisazyc.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtorsktjrj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydjk.org.cn/gtzfihsesh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtcrrlgbxq.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtnwqcgdge.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dianchejie.cn/gtaqcnyxmn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gtcwdkrvuz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtbndnjohg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtzmygbonh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtefkmbzmp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cqqwz.cn/gtwpoevejo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gogol.net.cn/gtejxgfyrx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jianghu66.top/gtxevkpapa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtxfqzrbrj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtbydmchul.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtajimwutd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenlongwang.top/gtippqslko.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jlsjyb.cn/gtpbhxftsc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtxuzhcsbd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtgxzaxmhq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gteyxvjhig.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtwhcxpenp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zycfv.cn/gtaoiyhrey.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.haohaochexian.top/gtuwvbpyju.html

[K05] 深拷贝对象
来源：http://hz.vqdsnc.cn/gtdujdrdog.html

Py:   copy.deepcopy(obj)
来源：http://hz.vqdsnc.cn/gtacbgkepy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtqqbqsblf.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtfbkzsxhr.html

TS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtairapktu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtcbbrjcqz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydzc1.top/gtczkqnsoh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cucudq.cn/gtxfvttprm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hfpthk.cn/gtmffsoktt.html

[K06] 解析 URL 查询串
来源：http://hz.jqgufenzy.top/gtipymrynf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinqigufen.top/gtscbegelv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhixingplan.top/gtmgwiagda.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yueranfly.top/gtnutirdgb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtzwjzfjti.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuxming.cn/gtpfnjatkh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.mhx1999.top/gtpwhnifll.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtsqraegqc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhijiandao.cn/gthqnpoosa.html

[K07] 进制转换
来源：http://hz.9152youxi.cn/gtsuallyoc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtzvwmucmc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.pengpengdd.cyou/gttytnvcly.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtuoupnlze.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtyopirqgq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtqppwpspy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.haohaochexian.top/gtixgauuae.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxinkj.top/gtuxjhoaap.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gttmcqbulv.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shuidangran.top/gtafmgnqic.html

Py:   pickle.dumps(obj)
来源：http://hz.yueranfly.top/gthjopezfz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtgdoexetn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtlotvhalu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtkheoljvi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtpuaqirik.html

Go:   encoding/gob
来源：http://hz.cashguo.top/gtzunlxurn.html

Ruby: Marshal.dump(obj)
来源：http://hz.mhx1999.top/gtjsmhyjzl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cqqwz.cn/gtmbpqxlch.html

================================================================================
来源：http://hz.jiagoushi.top/gtckiadcop.html

L. 网络请求
来源：http://hz.svipenyu.cn/gtewoqgvwo.html

================================================================================
来源：http://hz.cqqwz.cn/gtbabkgwqm.html

[L01] 发送 GET 请求
来源：http://hz.nwbrower.top/gtygnlmbpo.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cheryme.top/gtbsdxhtgu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jianghu66.top/gtwradrwsi.html

JS:   await fetch(url)
来源：http://hz.daxiang520.top/gtxangsjbh.html

TS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtottdwbxl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hywenlv.cn/gtbktklrwd.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtjeytbspu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jqgufenzy.top/gttrjytoyb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtbrinhagw.html

[L02] 发送 POST JSON
来源：http://hz.zhijiandao.cn/gtrlsormul.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhiwuduotai.top/gtdkqyfuwl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xingfuxueyuan.xyz/gtyldcdtwv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtoqtppzrl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigfzy.top/gtwjxrszdq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xziqi.cn/gtyxlwfanh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yonumen.top/gtolgmowhp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtrshxxdgv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jinqigufen.top/gtovaxlrpp.html

[L03] 设置自定义请求头
来源：http://hz.hfpthk.cn/gtvlilpibx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.fengsongda.top/gtickneosw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gtdaxnnqps.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.hnqzz.top/gtcpteneka.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cheryme.top/gtxpdtrlpe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtpywavwdr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.chenlongwang.top/gtmxvgbpsn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hnxiangtu.top/gtrqjyhyvj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.hysaishi.cn/gthjhcwynm.html

[L04] 设置超时
来源：http://hz.yuanzhike.top/gtbwmfxjkh.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yongpay.top/gttiphjjky.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj20258888.top/gtexasahsd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhiwuduotai.top/gttxkguwez.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinyuanbaomall.cn/gtkksysdsv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ppjwa.cn/gtzrtwaapp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.dashuyun.cn/gtbgvquwmw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.hysaishi.cn/gtrqjxfcbt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.zhixingplan.top/gthejsqpsh.html

[L05] 上传文件（multipart）
来源：http://hz.ydjk.org.cn/gtmldfayiy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yangfankeji.com/gtnproqupn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hfpthk.cn/gtfvegbtes.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.daria6918.cn/gtpwkvtcqb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtsyioviof.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.fzhhl.top/gtdxocedkn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.birdmap.top/gtymltkofw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xylfe.cn/gtvhlkpden.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtfbjnlpfj.html

[L06] 解析响应为 JSON
来源：http://hz.havefunace.top/gtjxomrfsb.html

Py:   resp.json()
来源：http://hz.feifeiyinyue.top/gtisucwkjs.html

PHP:  json_decode($body, true);
来源：http://hz.jinyuanbaomall.cn/gtfptgzvfj.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtzrzsaxjf.html

TS:   await resp.json()
来源：http://hz.jinqigfzy.top/gtcmfzdmzk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.xinyue.icu/gtyiftebxc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.sufxvd.cn/gtmbtszteh.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shzxlz.cn/gtebqbrrbp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.hfpthk.cn/gtdcvhwupv.html

[L07] 处理 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gtmswvbxel.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shuidangran.top/gtoedmhqtw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jyoumei.cn/gtxyhkqnhw.html

JS:   resp.ok;  resp.status
来源：http://hz.pengpengdd.cyou/gtvffoeyad.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtcuypbtjt.html

Java: resp.statusCode()
来源：http://hz.yj20258.top/gtlbxxakem.html

Go:   resp.StatusCode
来源：http://hz.nanxinkj.top/gtbgbfuxai.html

Ruby: resp.code.to_i
来源：http://hz.chenlongwang.top/gtlgqaleqe.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtgkyssbai.html

[L08] 并发请求多个地址
来源：http://hz.xziqi.cn/gthvypybra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.ehwqpu.com/gtrzcxubmv.html

PHP:  curl_multi_init() 系列
来源：http://hz.yonumen.top/gtfkzsdmwq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.zdqjudy.top/gtijlhphnt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xingfuxueyuan.xyz/gtbfgcxern.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.cheryme.top/gtmuglbbxw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zycfv.cn/gtskxhgiir.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zdqjudy.top/gtcoueuvqi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jiagoushi.top/gtgzatytbd.html

================================================================================
来源：http://hz.xziqi.cn/gtvxfsgerr.html

M. 命令行 / 进程 / 环境
来源：http://hz.ybcxt.top/gtzjwpaiiy.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthqloitsh.html

[M01] 读取命令行参数
来源：http://hz.xziqi.cn/gtbfxmhkoz.html

Py:   sys.argv[1:]
来源：http://hz.ivvv.top/gtfmwuuntt.html

PHP:  $argv;  $argc;
来源：http://hz.xziqi.cn/gtrlldhdhz.html

JS:   process.argv.slice(2)
来源：http://hz.ppjwa.cn/gtgzbztter.html

TS:   process.argv.slice(2)
来源：http://hz.wangshuangyany.cn/gtlnczlwxv.html

Java: args 数组（main 方法参数）
来源：http://hz.zycfv.cn/gtucgvkntq.html

Go:   os.Args[1:]
来源：http://hz.birdmap.top/gtcfhnlowi.html

Ruby: ARGV
来源：http://hz.tanke756.top/gtvqjtvrfl.html

C#:   args 数组（Main 方法参数）
来源：http://hz.daxiang520.top/gttxuohqqh.html

[M02] 读取环境变量
来源：http://hz.hammf.cn/gtsodjqzrb.html

Py:   os.environ.get("HOME")
来源：http://hz.shangyingyoupin.top/gthjetwayx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jiagoushi.top/gtnhcmbhos.html

JS:   process.env.HOME
来源：http://hz.smart0.xyz/gtsafsfbcl.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtljeoqqyn.html

Java: System.getenv("HOME")
来源：http://hz.yuanzhike.top/gthofzhxqr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yongpay.top/gtpbykgjbl.html

Ruby: ENV["HOME"]
来源：http://hz.snrcjt.cn/gtcjvyfcfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.tianlin.xyz/gtlgawslnf.html

[M03] 执行外部命令
来源：http://hz.ydzc1.top/gtmflbuelj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.sufxvd.cn/gtjmogqxag.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.cashguo.top/gtedjhcqbh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.hongshengwenyu.top/gtubwqwgfg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.tianlin.xyz/gtuhephsvw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.zhaomingkeji.xyz/gtxhexggps.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.bjfxy.top/gttbtzzrxi.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.zhixingplan.top/gtnjtsotpe.html

C#:   Process.Start("ls", "-l");
来源：http://hz.zhiwuduotai.top/gtbabsooux.html

[M04] 获取当前工作目录
来源：http://hz.xziqi.cn/gtjqosiasi.html

Py:   os.getcwd()
来源：http://hz.xylfe.cn/gtffqlmtuq.html

PHP:  getcwd();
来源：http://hz.sysykeji.top/gtlfspdgmi.html

JS:   process.cwd()
来源：http://hz.hongshengwenyu.top/gtydjrzbty.html

TS:   process.cwd()
来源：http://hz.c1oappe.top/gtznsewyjc.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.jiagoushi.top/gtvumvhljx.html

Go:   os.Getwd()
来源：http://hz.316326.xyz/gtjhficawv.html

Ruby: Dir.pwd
来源：http://hz.cashguo.top/gtedfpbwtv.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shanyushiyangkeji.top/gtjbhxfxuq.html

[M05] 设置退出码
来源：http://hz.sysykeji.top/gtkdpdrbmk.html

Py:   sys.exit(1)
来源：http://hz.jqgfzy.top/gttsiyhikf.html

PHP:  exit(1);
来源：http://hz.jlsjyb.cn/gtwliveqnt.html

JS:   process.exit(1)
来源：http://hz.guannengcc.top/gtwcsksxfx.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gtkaualkwe.html

Java: System.exit(1)
来源：http://hz.fengsongda.top/gtttfvzlea.html

Go:   os.Exit(1)
来源：http://hz.cqqwz.cn/gtalqatpfa.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtpgqfwcfv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.chenlongwang.top/gtjwhryuya.html

[M06] 向标准错误输出
来源：http://hz.zycfv.cn/gtmnescuko.html

Py:   print("err", file=sys.stderr)
来源：http://hz.cheryme.top/gtrfozqohi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.ydjk.org.cn/gtzybmgcyl.html

JS:   console.error("err")
来源：http://hz.zhongyouzk.top/gtrufgikvv.html

TS:   console.error("err")
来源：http://hz.andypj.xyz/gtmpxldhcs.html

Java: System.err.println("err")
来源：http://hz.nanxinkj.top/gtktfszvev.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.shanyushiyangtech.top/gtdadtcmcu.html

Ruby: warn "err"
来源：http://hz.vqdsnc.cn/gtfwhxnhoi.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.shanyushiyangtech.top/gtaoanbwrp.html

[M07] 判断是否为主入口
来源：http://hz.cucudq.cn/gtymwctjtk.html

Py:   if __name__ == "__main__":
来源：http://hz.yj20258.top/gtwrucimwo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.c1oappe.top/gtumydgzpu.html

JS:   require.main === module
来源：http://hz.ywan-chungtsiang.top/gtazlxotbu.html

TS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtpjigakta.html

Java: public static void main(String[] args)
来源：http://hz.smart0.xyz/gthgmmeqas.html

Go:   func main()
来源：http://hz.quarkkingdee.top/gtxldsntnr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.ydjk.org.cn/gtuwhkltdf.html

C#:   static void Main(string[] args)
来源：http://hz.ydjk.org.cn/gtgqhpnwop.html

[M08] 获取系统与运行时信息
来源：http://hz.cucudq.cn/gtfbmvjpuv.html

Py:   platform.system();  platform.python_version()
来源：http://hz.52xcode.cn/gtdeewwitn.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.9152youxi.cn/gtvskigqho.html

JS:   process.platform;  process.version
来源：http://hz.jianghu66.top/gtvkpkeshv.html

TS:   process.platform;  process.version
来源：http://hz.quarkkingdee.top/gthtkmjywq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinghuilouyu.cn/gtfvgreutj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.xingfuxueyuan.xyz/gtkakdetfn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.vqdsnc.cn/gtjlhbeqbx.html


<!-- 参考信息 -->