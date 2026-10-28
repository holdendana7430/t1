代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtjefltszd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtuqhskdtz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtbetmlpom.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtyumnsmdb.html

[J03] 字符串解析为日期
来源：http://hz.yj20258.top/gteqjogvlj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tanke756.top/gtkvzinxqa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtluvmabno.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtfnfvjowj.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtorxqhqgk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtsthpoxxa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cashguo.top/gtnohbzdky.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtvubhijcg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gttkobsbze.html

[J04] 时间戳与日期互转
来源：http://hz.hfpthk.cn/gtnfyikqhg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cashguo.top/gtfzyufafs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtlwdvxixd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gtuaffkbaw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtdctkhyne.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtiwweenrl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jianghu66.top/gtjxheyizm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtjygyhplt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtikxxpixp.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtkthmkroj.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gtosjsrmho.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtsyuwdgel.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtfnbmninm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtuqpdexrd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.c1oappe.top/gtwgiuvvww.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtenwscmjy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtwgcytthy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtociomejb.html

[J06] 计算两时间之差
来源：http://hz.iojbl.cn/gtufcetpgw.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtjbjjvudv.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtqmprlxmy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtukyyfinb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtbnhdigpt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnxiangtu.top/gtsucvnbjc.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtwelfdcbn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hywenlv.cn/gtfcjjrrnk.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gthyckxkec.html

[J07] 比较两个日期
来源：http://hz.jinqigufen.top/gtcnjgmkho.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtqckhxenz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtcxkdjaim.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtubxlhsnj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtxwnrifqv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gthtqeefyu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtworpqyuv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtlibkrwir.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtboiasgye.html

[J08] 提取年月日与星期
来源：http://hz.jinqigufen.top/gttqkdhxrf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.vqdsnc.cn/gthaanjlrd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtghozywkh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtvarohsho.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtxqjbsglm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dashuyun.cn/gtucyilcxu.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gthaklohwj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shuidangran.top/gtamvmpuxi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gtrntfoltv.html

[J09] 时区处理
来源：http://hz.shanyushiyangkeji.top/gtwegtpqat.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtgjmqvpmv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cdnleiting.top/gtejxnctgy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtktuqwsox.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtrzhwyosp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gtpqcthrwz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtsommoahy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtliehyeir.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuxming.cn/gtdvklfocc.html

[J10] 取今天 / 本月第一天
来源：http://hz.hysaishi.cn/gtzyhmbcpo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtvjeocqss.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtzbspwewd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtasgddhiy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gtpdureaxx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtcadnqymo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gtwxnupeou.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtktjapvrp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtsetgdrvt.html

================================================================================
来源：http://hz.iojbl.cn/gtwpwwitvi.html

K. JSON 与序列化
来源：http://hz.daxiang520.top/gtpcipygjj.html

================================================================================
来源：http://hz.cqqwz.cn/gtukwmoizz.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtazjhirpq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.feifeiyinyue.top/gtsppdggxc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.feifeiyinyue.top/gtqfnyhkfc.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtoacqzvby.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtzctrzqrl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.birdmap.top/gtxpvhajoa.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtjkgzujlp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhoulong.xyz/gthatosttp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtkutcsghc.html

[K02] JSON 字符串转对象
来源：http://hz.fzhhl.top/gtreqipqkd.html

Py:   json.loads(s)
来源：http://hz.guannengcc.top/gtmmrqvimm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxinkj.top/gtqaaugnmz.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtwsxqxeav.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtdclymmmu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinqigufen.top/gtalsdruiv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zdqjudy.top/gteyxwwoso.html

Ruby: JSON.parse(s)
来源：http://hz.xziqi.cn/gtjnspgbvd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhoulong.xyz/gtzeijtyiw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtyrpzfqvv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtllmhoccr.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtwukomotd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtbahxhqco.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.quarkkingdee.top/gtyceisldg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daxiang520.top/gtfvdibofo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtmtebqjxt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtjjlrxmod.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hongshengwenyu.top/gtvilbleir.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtunaqmntg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zdqjudy.top/gtppvuvbhb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hfpthk.cn/gtweuuscep.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtgxsgehzw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sxryk.cn/gtjtizwhhm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.birdmap.top/gtplpllpfn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtojkityic.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtosypqafj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj202588.top/gtplkfxbnx.html

[K05] 深拷贝对象
来源：http://hz.jinghuilouyu.cn/gtmwfropca.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gthjqrmnos.html

PHP:  unserialize(serialize($obj));
来源：http://hz.kuanghao11.cn/gtapnjbeqq.html

JS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtdsohgmvu.html

TS:   structuredClone(obj)
来源：http://hz.birdmap.top/gtqsaspvwn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cdnleiting.top/gtmdjcfzac.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nanxinkj.top/gtcquakjtq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtrrhifzel.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtyvfosoym.html

[K06] 解析 URL 查询串
来源：http://hz.yongpay.top/gtdhckrrjd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shangyingyoupin.top/gtouunjpou.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtimtkgatv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ivvv.top/gtwppmpvbp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gogol.net.cn/gtoqmhmhsf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtyfhhwjlc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtsvabnesx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtnngrjjct.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sufxvd.cn/gtejqfnljw.html

[K07] 进制转换
来源：http://hz.jinghuilouyu.cn/gtvxicjzsm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gttaosyslj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.xylfe.cn/gtuuuleoed.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtggwbxrbs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.svipenyu.cn/gtbcydfhjp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtxzurcgkv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hammf.cn/gthejhctty.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtuyzicann.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.haohaochexian.top/gtjzpxdrwf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtkqkuepac.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtmlhegmgx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ywan-chungtsiang.top/gtxjmthzwn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtshnxhhxc.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yvedp.cn/gtiptspjne.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtnbycqpal.html

Go:   encoding/gob
来源：http://hz.cqqwz.cn/gthwhlaeuh.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtskiyxepd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.aibaodan.cn/gtsvkfydvt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtoceaoigw.html

L. 网络请求
来源：http://hz.daxiang520.top/gtzocznbau.html

================================================================================
来源：http://hz.gogol.net.cn/gtsbzlekly.html

[L01] 发送 GET 请求
来源：http://hz.tanke756.top/gtzrnumhkb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhiwuduotai.top/gtqrliaoyx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtnssgnstx.html

JS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtevggsqqj.html

TS:   await fetch(url)
来源：http://hz.nwbrower.top/gtuvbtwkcz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.havefunace.top/gtwintdbok.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtcryhavyq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtctsgpcoh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hysaishi.cn/gtsobngdiz.html

[L02] 发送 POST JSON
来源：http://hz.hnqzz.top/gtgzapftqy.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.havefunace.top/gtlaxkmwgw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ehwqpu.com/gtpymoomkc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ydjk.org.cn/gtvwdmouxg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtxreyqeij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zdqjudy.top/gtuifvwlhb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtiaqsqifq.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gogol.net.cn/gtgwmhxegw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hammf.cn/gtcsbjdeih.html

[L03] 设置自定义请求头
来源：http://hz.yvedp.cn/gthmiikbjn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cucudq.cn/gttluchstw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.haohaochexian.top/gtbcvqvgrb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtvnhzqexc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gthvjlmmqh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtzyfqvkvq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgfzy.top/gtghmglkfu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.birdmap.top/gtahxpkjiv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.fzhhl.top/gtfncuxfwj.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtubyzigkz.html

Py:   requests.get(url, timeout=5)
来源：http://hz.nanxuanxn.top/gticuetrfy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.nanxuanxn.top/gtayrrcokk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.chenjidiqi.icu/gtrikpeqys.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.quarkkingdee.top/gtnaulclsw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yangfankeji.com/gtekqnwibl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.bjfxy.top/gtralndvgb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.xuanzx.com/gttmvndken.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shzxlz.cn/gtovxswuiw.html

[L05] 上传文件（multipart）
来源：http://hz.cdnleiting.top/gtugfwqezt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shanyushiyangtech.top/gthqpolsix.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.yanxiufei.cn/gtozutisjf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.zhijiandao.cn/gtjtvtwndk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.snrcjt.cn/gtqblbdxhs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yangfankeji.com/gtrrkbcfaq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.ywan-chungtsiang.top/gtehcbmqlm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.redwolf501.top/gtbddooxkz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtzeshbysg.html

[L06] 解析响应为 JSON
来源：http://hz.9152youxi.cn/gtdardngvy.html

Py:   resp.json()
来源：http://hz.dashuyun.cn/gtyixmlcyz.html

PHP:  json_decode($body, true);
来源：http://hz.haohaochexian.top/gthltadipt.html

JS:   await resp.json()
来源：http://hz.bjfxy.top/gtecivuizh.html

TS:   await resp.json()
来源：http://hz.aizwys.cn/gtjxoujfim.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.bjfxy.top/gtnqhvilry.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jinqigufen.top/gtfmxsorjk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.guowangkeji.top/gtkvliqewu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.cashguo.top/gtfzyxmqar.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtuujcvqnl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.zhixingplan.top/gtzmubecye.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.gzhubu.top/gtukhasnpe.html

JS:   resp.ok;  resp.status
来源：http://hz.jinghuilouyu.cn/gtchrtndur.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtgtdnfgun.html

Java: resp.statusCode()
来源：http://hz.hnxiangtu.top/gtlaqxouxm.html

Go:   resp.StatusCode
来源：http://hz.cheryme.top/gtavokvqih.html

Ruby: resp.code.to_i
来源：http://hz.c1oappe.top/gtadheakya.html

C#:   (int)resp.StatusCode
来源：http://hz.gotoacloud.top/gtwuqqwbbq.html

[L08] 并发请求多个地址
来源：http://hz.shzxlz.cn/gtwrvgqtxj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.fzhhl.top/gtkmcaunho.html

PHP:  curl_multi_init() 系列
来源：http://hz.tian-w.cn/gtvujtewpe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.mhx1999.top/gtropiqrfx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangshuangyany.cn/gthpvsckms.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.yangfankeji.com/gthfwsteeq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.chenlongwang.top/gtkdhtblbp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.iojbl.cn/gtywnotbyg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.guannengcc.top/gtfdvtsxit.html

================================================================================
来源：http://hz.jinqigfzy.top/gthcswzhhc.html

M. 命令行 / 进程 / 环境
来源：http://hz.hfpthk.cn/gthhbiogpu.html

================================================================================
来源：http://hz.c1oappe.top/gtekwixdko.html

[M01] 读取命令行参数
来源：http://hz.jqgufenzy.top/gtfzldeevg.html

Py:   sys.argv[1:]
来源：http://hz.wangshuangyany.cn/gtbuxuoyhz.html

PHP:  $argv;  $argc;
来源：http://hz.dashuyun.cn/gtjrufesnd.html

JS:   process.argv.slice(2)
来源：http://hz.9152youxi.cn/gtbmrpgtus.html

TS:   process.argv.slice(2)
来源：http://hz.ivvv.top/gtnqymczno.html

Java: args 数组（main 方法参数）
来源：http://hz.hfpthk.cn/gtwldghsdw.html

Go:   os.Args[1:]
来源：http://hz.sufxvd.cn/gtttwfokkj.html

Ruby: ARGV
来源：http://hz.mhx1999.top/gtsvcrpxci.html

C#:   args 数组（Main 方法参数）
来源：http://hz.aizwys.cn/gtfrrqdubn.html

[M02] 读取环境变量
来源：http://hz.yangfankeji.com/gtxdeytmqp.html

Py:   os.environ.get("HOME")
来源：http://hz.sysykeji.top/gtzufoqrzh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtkahuhnfl.html

JS:   process.env.HOME
来源：http://hz.pengpengdd.cyou/gtkmksvyqk.html

TS:   process.env.HOME
来源：http://hz.pycfn.com/gtdxpjadln.html

Java: System.getenv("HOME")
来源：http://hz.cdnleiting.top/gtgzdugczk.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.9152youxi.cn/gtdqbbmyxw.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtoffyepjz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gtbypgapse.html

[M03] 执行外部命令
来源：http://hz.gotoacloud.top/gtcozwjsbs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.shuidangran.top/gtwygmriys.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ivvv.top/gtjytkctxk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yonumen.top/gtivgwuksz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.zhiwuduotai.top/gtsajzxgox.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jinghuilouyu.cn/gtsdkambmw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ehwqpu.com/gtiymnszar.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.xinyue.icu/gtaowefswo.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jqgfzy.top/gtrggaewbi.html

[M04] 获取当前工作目录
来源：http://hz.yonumen.top/gtnkomkbrb.html

Py:   os.getcwd()
来源：http://hz.gzhubu.top/gtwhvjdlin.html

PHP:  getcwd();
来源：http://hz.sweek.top/gtqndzjaya.html

JS:   process.cwd()
来源：http://hz.hfpthk.cn/gtfrxtayea.html

TS:   process.cwd()
来源：http://hz.havefunace.top/gtbxkjwqgd.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.snrcjt.cn/gttuteccew.html

Go:   os.Getwd()
来源：http://hz.cdnleiting.top/gtbgarqazl.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gthgivvxzp.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.kuanghao11.cn/gtvgrvfmig.html

[M05] 设置退出码
来源：http://hz.smart0.xyz/gtwwcxykvz.html

Py:   sys.exit(1)
来源：http://hz.zhongyouzk.top/gtdhquqrmo.html

PHP:  exit(1);
来源：http://hz.sxryk.cn/gtbcfagjzv.html

JS:   process.exit(1)
来源：http://hz.cdnleiting.top/gtozurupqe.html

TS:   process.exit(1)
来源：http://hz.zhengqikj.top/gtytzcfqmn.html

Java: System.exit(1)
来源：http://hz.chenzaomai.com/gtpjydrpea.html

Go:   os.Exit(1)
来源：http://hz.zhaomingkeji.xyz/gtruinkxwd.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtpjfcbhds.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nwbrower.top/gtirbnwzap.html

[M06] 向标准错误输出
来源：http://hz.wangdashe.top/gtzjnmwnrt.html

Py:   print("err", file=sys.stderr)
来源：http://hz.wangdashe.top/gtpfqotcfj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.yj202588.top/gturtnivyb.html

JS:   console.error("err")
来源：http://hz.jianghu66.top/gtxjtojsft.html

TS:   console.error("err")
来源：http://hz.iojbl.cn/gtgjqocgoj.html

Java: System.err.println("err")
来源：http://hz.wangshuangyany.cn/gtksdfwgaj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gtiyhnpyev.html

Ruby: warn "err"
来源：http://hz.gogol.net.cn/gtqghbeyot.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhijiandao.cn/gtpaebtdbb.html

[M07] 判断是否为主入口
来源：http://hz.zhoulong.xyz/gtfulbvaqv.html

Py:   if __name__ == "__main__":
来源：http://hz.wangshuangyany.cn/gtkryzyrrh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.cdnleiting.top/gtdzpqhwbf.html

JS:   require.main === module
来源：http://hz.xingfuxueyuan.xyz/gtztsatrcl.html

TS:   require.main === module
来源：http://hz.cdnleiting.top/gtezljocrj.html

Java: public static void main(String[] args)
来源：http://hz.tanke756.top/gtnqusfceq.html

Go:   func main()
来源：http://hz.zhijiandao.cn/gtsbwlohlr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.xziqi.cn/gtysnobbcy.html

C#:   static void Main(string[] args)
来源：http://hz.cheryme.top/gtzscdbahi.html

[M08] 获取系统与运行时信息
来源：http://hz.tian-w.cn/gthsomkzfj.html

Py:   platform.system();  platform.python_version()
来源：http://hz.fzhhl.top/gthtjvafux.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.xziqi.cn/gtxezethll.html

JS:   process.platform;  process.version
来源：http://hz.hywenlv.cn/gtscvknfln.html

TS:   process.platform;  process.version
来源：http://hz.daria6918.cn/gtgssjizqz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.jinyuanbaomall.cn/gtavicnccd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.haohaochexian.top/gtgkxltkxl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.jqgfzy.top/gttjgskhir.html


<!-- 参考信息 -->