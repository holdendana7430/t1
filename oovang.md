代发 wailian999

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtunsmvgrn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtlacbryfo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtyhpgpiaz.html

JS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gtozqpkggb.html

TS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtuwupqxev.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtfzfsbibo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtfxixrdwe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtwxcoyusz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhoulong.xyz/gtucdhgmjd.html

[J04] 时间戳与日期互转
来源：http://hz.ppjwa.cn/gtewhdqngv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtgszfzogw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hongshengwenyu.top/gtcdwqzoqi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnqzz.top/gtetndhejl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xylfe.cn/gtqtovwhfs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtblfhqeqt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtbmykxsta.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtgdnbmvpu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtkxdrcyke.html

[J05] 时间加减（加 7 天）
来源：http://hz.sxryk.cn/gthdmbzrmw.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtjzklgfhb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtjwdipkaa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtlhivunhw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtopdsgxkl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtgmmsugqi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangkeji.top/gtvgdmtche.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtshfanihe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtzffrxbow.html

[J06] 计算两时间之差
来源：http://hz.nwbrower.top/gtuatdrgwz.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtedqvtunq.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtzgplnjxf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pycfn.com/gtfxlpowrp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtmzxhwncb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtfpmaznkd.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtzkbdiyrt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtddvktqkv.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gtmjdyxxkw.html

[J07] 比较两个日期
来源：http://hz.sufxvd.cn/gtzpcrmxgs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtxcykufhz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sweek.top/gtcfxgmdma.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtrceagmya.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.9152youxi.cn/gtyhhnrpaf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenlongwang.top/gtarhmjtqe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shangyingyoupin.top/gtozibolfo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtdqoaebzw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtzedqziem.html

[J08] 提取年月日与星期
来源：http://hz.gogol.net.cn/gtyddmmoxk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtzkhzemue.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gtnizowunv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtvmgnkini.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtsrryntqs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuetiantiany.cn/gtjidyipov.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtrdpnfbfs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hongshengwenyu.top/gtbhvhemvz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtleakrsfm.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtpqwgzlwn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtanebnmjb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shuidangran.top/gtniqrtbpp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gthhroxziw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gturedqveg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj202588.top/gttaxnazcl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtesnmiqrg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtgdkkjmar.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtlcrdicuf.html

[J10] 取今天 / 本月第一天
来源：http://hz.tanke756.top/gtyxlytxnr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tianlin.xyz/gtcrsjymwx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtlkwxcrue.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zycfv.cn/gtzfntjpuy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtxdfzozbi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.meibo888.top/gtyfzjjmph.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtfnbbvswt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtumxjqzfw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtteyhrqho.html

================================================================================
来源：http://hz.cashguo.top/gtdathwraw.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtwhnrmzvd.html

================================================================================
来源：http://hz.wangdashe.top/gtfnnqnmel.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuxming.cn/gtvlupuchb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtcvotoiwi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shuidangran.top/gtjllucsti.html

JS:   JSON.stringify(obj)
来源：http://hz.xuanzx.com/gtpdbtdhxd.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gthsnhcahm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtcomvgrfk.html

Go:   json.Marshal(obj)
来源：http://hz.xylfe.cn/gtcpxkimlf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gtjphkfkkh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtvfjagicf.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtdgyfxibr.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtdcokbrke.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtdtkcgvxm.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtdnnyjvub.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtnqmzgcdm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.birdmap.top/gtqgbbfxio.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gtasopqapr.html

Ruby: JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtkvkpzcxy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtadexaabc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtycdfpbug.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yonumen.top/gtxltpiolo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtamnulses.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtdiuymiau.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtxpiozmez.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gtzyogjxcd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtmiguvaxc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtdpvtizli.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cashguo.top/gtkrqhnhhn.html

[K04] 读取 JSON 文件
来源：http://hz.xuetiantiany.cn/gtgmgwtvnr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.aizwys.cn/gtmybnqyae.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.mhx1999.top/gtktelpekr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtlmtowmry.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtbsevlare.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtnuhqrfdc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtxukxxvdw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtiumxsnhh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtljtiscmt.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtwsubbzwt.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtdoahhmdr.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtnlsibipl.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtlkwlpmhf.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtrybzwgsc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gthhcrersm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtlkirvole.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtwphazcpt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xinyue.icu/gtsdjyagym.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtwjheoshx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shuidangran.top/gtwvudfgoj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtewjpyheg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtpjheeafz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtrjtnypgv.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jiagoushi.top/gtycqzyadc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zycfv.cn/gtebibgsjt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zycfv.cn/gtcbciqnbn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtfzqqetul.html

[K07] 进制转换
来源：http://hz.gaohongyu789.top/gtwijdroju.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtrixalmtj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gzhubu.top/gtybhajyuj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtkexggxjj.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cucudq.cn/gtjhxapbzx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtfvsfploo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.ydjk.org.cn/gtustsebnf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtnguruubk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hammf.cn/gtbujbxdbb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtguulnpuo.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gtpscfvkmq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtvchozaio.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gteclwajly.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtajsfhpis.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.sxryk.cn/gtlwokivdy.html

Go:   encoding/gob
来源：http://hz.kuanghao11.cn/gtctlopdlt.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydjk.org.cn/gtkxxclayr.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.nanxuanxn.top/gtcnusrumz.html

================================================================================
来源：http://hz.xylfe.cn/gtgitgmizy.html

L. 网络请求
来源：http://hz.jinghuilouyu.cn/gtgrhhsfed.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtouphnnxo.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtklyaccju.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigufen.top/gtgjvgztmh.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.haohaochexian.top/gtwajmfeyc.html

JS:   await fetch(url)
来源：http://hz.ydzc1.top/gtlgkghmom.html

TS:   await fetch(url)
来源：http://hz.meibo888.top/gtdwvckiqb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shangyingyoupin.top/gtocaaxvje.html

Go:   resp, err := http.Get(url)
来源：http://hz.shzxlz.cn/gtvsxpwucb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.andypj.xyz/gtliizokfb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jiagoushi.top/gtodldpjpk.html

[L02] 发送 POST JSON
来源：http://hz.zhixingplan.top/gtkfayoqhw.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nanxinkj.top/gtypukjoek.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.dianchejie.cn/gtzpjnoimv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xuetiantiany.cn/gtzxfrbzib.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.pengpengdd.cyou/gtnvfyulgc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yanxiufei.cn/gtgzklnrim.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgufenzy.top/gtwptgfudn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nwbrower.top/gtrsfchqwg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtfelpjkdg.html

[L03] 设置自定义请求头
来源：http://hz.hnxiangtu.top/gtovktruxt.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hywenlv.cn/gtflmzfeuo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zdqjudy.top/gthdvjrfpr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtgajqwzyu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtjswvhncg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.daria6918.cn/gtzqhimvmg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.316326.xyz/gtfphnrkxf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.cheryme.top/gtkfoznesa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinghuilouyu.cn/gtbdrkqdzz.html

[L04] 设置超时
来源：http://hz.tanke756.top/gtygyvxekv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ehwqpu.com/gtfnnayppx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.dianchejie.cn/gtvycfwkob.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cashguo.top/gtqlrwkklz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.pycfn.com/gtumwlwgbc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.xuanzx.com/gtghfdkeqg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.daxiang520.top/gtwiyhabpo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.kuanghao11.cn/gtvbgzdwkb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hfpthk.cn/gtfmftncno.html

[L05] 上传文件（multipart）
来源：http://hz.yanxiufei.cn/gtwzbzwgcf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.dianchejie.cn/gtnyvcpvof.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.aizwys.cn/gtehgtswtr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtcvxzuagu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.birdmap.top/gtcnpvdphc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.feifeiyinyue.top/gtnhklgkrs.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.iojbl.cn/gttgiucqwn.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sweek.top/gtnazhbfhc.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jqgfzy.top/gtfkdpkixe.html

[L06] 解析响应为 JSON
来源：http://hz.gzhubu.top/gtrgjmhscz.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtssmtjfqm.html

PHP:  json_decode($body, true);
来源：http://hz.fengsongda.top/gtdenkegyq.html

JS:   await resp.json()
来源：http://hz.sysykeji.top/gtwlcvjacv.html

TS:   await resp.json()
来源：http://hz.jinghuilouyu.cn/gtbxiiafna.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.jinqigfzy.top/gtxduifuez.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.316326.xyz/gtjqshknfy.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangtech.top/gtezdjptxt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.ehwqpu.com/gtawniafdc.html

[L07] 处理 HTTP 状态码
来源：http://hz.sufxvd.cn/gtwsikhkdj.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hnxiangtu.top/gtvjmwuuop.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.havefunace.top/gtfxriarno.html

JS:   resp.ok;  resp.status
来源：http://hz.guannengcc.top/gtbyzzqxwf.html

TS:   resp.ok;  resp.status
来源：http://hz.yanxiufei.cn/gtyptahhpz.html

Java: resp.statusCode()
来源：http://hz.tanke756.top/gtrpabhdzq.html

Go:   resp.StatusCode
来源：http://hz.hammf.cn/gtcutlxjlz.html

Ruby: resp.code.to_i
来源：http://hz.daxiang520.top/gtscwtyjhp.html

C#:   (int)resp.StatusCode
来源：http://hz.feifeiyinyue.top/gtskwjrfde.html

[L08] 并发请求多个地址
来源：http://hz.ehwqpu.com/gtcubulspb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fengsongda.top/gtawlajzcm.html

PHP:  curl_multi_init() 系列
来源：http://hz.yueranfly.top/gtubrqouex.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.chenjidiqi.icu/gtswffcklo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtifahfiqf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tian-w.cn/gtskedabfe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.yuxming.cn/gtetiixufl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.guowangkeji.top/gtxufbpnki.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.wangdashe.top/gtiuoeappl.html

================================================================================
来源：http://hz.zhoulong.xyz/gtqpqzahqr.html

M. 命令行 / 进程 / 环境
来源：http://hz.sweek.top/gtpglqwcwl.html

================================================================================
来源：http://hz.iojbl.cn/gtxsfnjdpr.html

[M01] 读取命令行参数
来源：http://hz.xylfe.cn/gtovwkaqxm.html

Py:   sys.argv[1:]
来源：http://hz.dianchejie.cn/gtaqmowqfx.html

PHP:  $argv;  $argc;
来源：http://hz.gogol.net.cn/gtqgwyypgo.html

JS:   process.argv.slice(2)
来源：http://hz.hnqzz.top/gtuyffjvtr.html

TS:   process.argv.slice(2)
来源：http://hz.shanyushiyangtech.top/gtwdygvclv.html

Java: args 数组（main 方法参数）
来源：http://hz.sweek.top/gtqywiayiq.html

Go:   os.Args[1:]
来源：http://hz.jianghu66.top/gtdzuppzms.html

Ruby: ARGV
来源：http://hz.snrcjt.cn/gtbjcldmsw.html

C#:   args 数组（Main 方法参数）
来源：http://hz.hnxiangtu.top/gtbxheczji.html

[M02] 读取环境变量
来源：http://hz.yanxiufei.cn/gtgsiairbi.html

Py:   os.environ.get("HOME")
来源：http://hz.zhaomingkeji.xyz/gtugkjxzsc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.52xcode.cn/gtctrfuckv.html

JS:   process.env.HOME
来源：http://hz.hammf.cn/gtwwwpgmkl.html

TS:   process.env.HOME
来源：http://hz.wangshuangyany.cn/gtmkftjfzx.html

Java: System.getenv("HOME")
来源：http://hz.xylfe.cn/gtgkqhnnrj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.ehwqpu.com/gtvobptjzr.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gtabtjeumu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.zhoulong.xyz/gtnbdzstha.html

[M03] 执行外部命令
来源：http://hz.nanxinkj.top/gtqelmgcpt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.xinyue.icu/gtsqnnavuz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ywan-chungtsiang.top/gtqulemeel.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.xinyue.icu/gtybjdaphr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gogol.net.cn/gttorbwtxx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.meibo888.top/gttzvzwwjq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pengpengdd.cyou/gtpvdekmtw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.chenjidiqi.icu/gtkjoqokww.html

C#:   Process.Start("ls", "-l");
来源：http://hz.redwolf501.top/gtqvzsdwnv.html

[M04] 获取当前工作目录
来源：http://hz.meibo888.top/gtweyugtih.html

Py:   os.getcwd()
来源：http://hz.shzxlz.cn/gtzdahjpio.html

PHP:  getcwd();
来源：http://hz.yonumen.top/gtheboyuxr.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gttjhdfcqd.html

TS:   process.cwd()
来源：http://hz.ybcxt.top/gtesuoyjxs.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtwjwyqkeo.html

Go:   os.Getwd()
来源：http://hz.sxryk.cn/gtrhwccldy.html

Ruby: Dir.pwd
来源：http://hz.yanxiufei.cn/gtnovkhxzp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.hywenlv.cn/gttgisqbcz.html

[M05] 设置退出码
来源：http://hz.feifeiyinyue.top/gthbxqgvfz.html

Py:   sys.exit(1)
来源：http://hz.sufxvd.cn/gtmamtkiin.html

PHP:  exit(1);
来源：http://hz.jianghu66.top/gtzpabobsk.html

JS:   process.exit(1)
来源：http://hz.sufxvd.cn/gtxolabkgb.html

TS:   process.exit(1)
来源：http://hz.chenjidiqi.icu/gtaxqccakv.html

Java: System.exit(1)
来源：http://hz.yongpay.top/gtdcmizpos.html

Go:   os.Exit(1)
来源：http://hz.svipenyu.cn/gtlckzydni.html

Ruby: exit 1
来源：http://hz.nanxuanxn.top/gtpmgxvfsi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.tian-w.cn/gtpbmnizbs.html

[M06] 向标准错误输出
来源：http://hz.gogol.net.cn/gtgypeigvc.html

Py:   print("err", file=sys.stderr)
来源：http://hz.daria6918.cn/gtlwjcomhm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hywenlv.cn/gthvxdiwpi.html

JS:   console.error("err")
来源：http://hz.cucudq.cn/gtrtbbyisf.html

TS:   console.error("err")
来源：http://hz.chenzaomai.com/gtwctipepn.html

Java: System.err.println("err")
来源：http://hz.jianghu66.top/gtqgfpxgoh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.meibo888.top/gtiyodfgsl.html

Ruby: warn "err"
来源：http://hz.shuidangran.top/gtrxtiqphm.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.316326.xyz/gtehsvhfwo.html

[M07] 判断是否为主入口
来源：http://hz.cheryme.top/gtwzvrwfzn.html

Py:   if __name__ == "__main__":
来源：http://hz.vqdsnc.cn/gtdobnddjv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.jinyuanbaomall.cn/gtkmlhnyqd.html

JS:   require.main === module
来源：http://hz.jyoumei.cn/gtsybybkpu.html

TS:   require.main === module
来源：http://hz.c1oappe.top/gtqeyeerqs.html

Java: public static void main(String[] args)
来源：http://hz.ydjk.org.cn/gtuavdsety.html

Go:   func main()
来源：http://hz.yvedp.cn/gtsfvonyup.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.cashguo.top/gtkqxcgyke.html

C#:   static void Main(string[] args)
来源：http://hz.jlsjyb.cn/gtipvnjspl.html

[M08] 获取系统与运行时信息
来源：http://hz.fengsongda.top/gtoecbkzcz.html

Py:   platform.system();  platform.python_version()
来源：http://hz.cheryme.top/gthttfalmo.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.ivvv.top/gtpvltyjpr.html

JS:   process.platform;  process.version
来源：http://hz.yj20258.top/gtgiastzjr.html

TS:   process.platform;  process.version
来源：http://hz.nanxinkj.top/gtxkfcgnkf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.andypj.xyz/gtbhnotvif.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.mhx1999.top/gtsoxmzfcf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.feifeiyinyue.top/gtizdaqlpj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://hz.zhoulong.xyz/gtwcambisw.html

================================================================================
来源：http://hz.smart0.xyz/gtdewajcrp.html

N. 数据结构与算法
来源：http://hz.jiagoushi.top/gtcqhlvjdp.html

================================================================================
来源：http://hz.yj20258.top/gtmtnxgkcv.html


<!-- 参考信息 -->