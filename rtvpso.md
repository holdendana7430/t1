代发 wailian999

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtkkphnswb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtbgqonvob.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtxeoixzur.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhiwuduotai.top/gtsmqwxpus.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtrtfwzzap.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtehidoarj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtdoivczpg.html

JS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtjulwudbj.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtbsuaucat.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtykjterkd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gtbxpecdcg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtoqudfbpp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtscrzcqjb.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtnsgnlevz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258888.top/gtggehoqot.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yanxiufei.cn/gtyrpeiibq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtucpujpnl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtxchusybh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtzvhoryyk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gtltixiyqp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shuidangran.top/gtmmmukhwz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtpsuhuvlg.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gttjaigxdt.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtgmrjqeal.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gthclvuqkd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtdowuhedp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtenbuqmrg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gtbhnuqahv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guowangkeji.top/gtkvxxvhba.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenlongwang.top/gtbpomcwrp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sxryk.cn/gtfktoyiwd.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtmmhucyen.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtinwpzhep.html

PHP:  $end->diff($start)->days;
来源：http://hz.pengpengdd.cyou/gtfowbcrlm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtkyqoqcoo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhoulong.xyz/gtzehodrdm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtjbhjjvdl.html

Go:   end.Sub(start).Hours()
来源：http://hz.gzhubu.top/gtealzkcmb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtcnlhwjdx.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtginxhexg.html

[J07] 比较两个日期
来源：http://hz.hongshengwenyu.top/gtmupgopke.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtihbdwtwb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinqigfzy.top/gtsdogguml.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtacsmossr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gteboqrquj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtpkhqxyay.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xuetiantiany.cn/gtwmraadow.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtobcbephg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtwxtphhrq.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtfczohmen.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtinxpnuwn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtikksfsmt.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinghuilouyu.cn/gtmphkejup.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtvunaoapv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gttfzaptpr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtauyuasus.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daxiang520.top/gthxwvuiwp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtrcmwlavm.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtkqechqjw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtxxhswwai.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.guannengcc.top/gtkiqxvgss.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtmpwryfmz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtvjwlcopz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gthcxxzmjf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtuneexekj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gogol.net.cn/gtkzuogoxx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuanzx.com/gtljocaalc.html

[J10] 取今天 / 本月第一天
来源：http://hz.zycfv.cn/gtdlzfitqm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgfzy.top/gtbyxfyzur.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.mhx1999.top/gtgpefldgl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtssccpmtg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtpnbjvfps.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtnamenalo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtjfqqacbe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtxoshyzti.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gthadgsoyg.html

================================================================================
来源：http://hz.hfpthk.cn/gtsapombdj.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtspfbgntc.html

================================================================================
来源：http://hz.daria6918.cn/gtummdbqaj.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtpuvbitjg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtmnglvbkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtbkwwaroa.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtopcxspcf.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtlucosfmh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dianchejie.cn/gtmsntjzhn.html

Go:   json.Marshal(obj)
来源：http://hz.wangdashe.top/gtinfkrgiv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxinkj.top/gtcmfupflg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gtvbavzduu.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtaobfwgjh.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtotidptvi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtnzwqivge.html

JS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtxatrvezm.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtcacabegn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shuidangran.top/gtncutnndf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhiwuduotai.top/gthaosykug.html

Ruby: JSON.parse(s)
来源：http://hz.sufxvd.cn/gtfldlqdlo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtmgdyhmjq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtndfhphel.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tanke756.top/gtdrfhwtxk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgufenzy.top/gtojyulryf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cucudq.cn/gttyfmvspr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtewkzjbud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtjktrvfhq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtrtozhtab.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xinyue.icu/gtbrmstybu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtaeuiqjwh.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtyzmmhrlj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtgaegmsfy.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtiaegdkuy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.snrcjt.cn/gturfbxcbi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gttjlqvkaa.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtpfyojfzg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtjhgzpcou.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtglesfyhh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtjzorvcgu.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtljbmczcc.html

Py:   copy.deepcopy(obj)
来源：http://hz.mhx1999.top/gtkicwtleh.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtmkhfiqvj.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtberiddlu.html

TS:   structuredClone(obj)
来源：http://hz.bjfxy.top/gtpigkjquv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jianghu66.top/gtxihxlecr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gttrytxjjk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtxkulqglx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtqwfqczzw.html

[K06] 解析 URL 查询串
来源：http://hz.nanxinkj.top/gtfcnrgvfq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.snrcjt.cn/gtftefhekp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jyoumei.cn/gticdrbobg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtmncdvnxj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.kuanghao11.cn/gtgtyafqvt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtgvhpexyo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hnqzz.top/gtxpyijuml.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gtiovbqoet.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtwsjqnykn.html

[K07] 进制转换
来源：http://hz.iojbl.cn/gtcvqmcidl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.gzhubu.top/gtggudoaqa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sysykeji.top/gtvbkobgxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtguvyxjte.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtbzcznpaw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cashguo.top/gttpxcidxr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.quarkkingdee.top/gtwppzvvzy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtprdbwcgd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgufenzy.top/gthcjmrmdw.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.haohaochexian.top/gtqgrmspgu.html

Py:   pickle.dumps(obj)
来源：http://hz.yuanzhike.top/gtbevdcatl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jiagoushi.top/gtcwgrhvmn.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtvvjrsdbi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtdkybhogs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtlofletqg.html

Go:   encoding/gob
来源：http://hz.iojbl.cn/gtxgybnhli.html

Ruby: Marshal.dump(obj)
来源：http://hz.havefunace.top/gteqivvzgq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtjtmmskcg.html

================================================================================
来源：http://hz.iojbl.cn/gtajmychsh.html

L. 网络请求
来源：http://hz.yonumen.top/gtgdvugisl.html

================================================================================
来源：http://hz.yj202588.top/gtnprmfved.html

[L01] 发送 GET 请求
来源：http://hz.jqgfzy.top/gtpqfllyod.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhongyouzk.top/gtczdcukig.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hammf.cn/gthikzeyyb.html

JS:   await fetch(url)
来源：http://hz.birdmap.top/gtbgjpkvac.html

TS:   await fetch(url)
来源：http://hz.sufxvd.cn/gtqmcizrhi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gtptmjzwfq.html

Go:   resp, err := http.Get(url)
来源：http://hz.c1oappe.top/gtbithcdyo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtnpvrpczf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.0kj1m.cn/gtiblqoxjk.html

[L02] 发送 POST JSON
来源：http://hz.jyoumei.cn/gtkndpykva.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shuidangran.top/gtutzlroyf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gttkofgtig.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.xylfe.cn/gtudlqywlf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.havefunace.top/gtmbjbfjyb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yuanzhike.top/gtdairvavq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.shangyingyoupin.top/gtzuhhhljf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.0kj1m.cn/gtkhdnvxdd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jqgufenzy.top/gtdxokoavh.html

[L03] 设置自定义请求头
来源：http://hz.snrcjt.cn/gtuurcfsly.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtredqdciy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.chenzaomai.com/gtnrlurlwc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtuhijovdv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yonumen.top/gtwufgcnwe.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gzhubu.top/gtxkiwqtmx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.pycfn.com/gtdkyrqclg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuetiantiany.cn/gthytkijvz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yuxming.cn/gtpgxxvgeb.html

[L04] 设置超时
来源：http://hz.tianlin.xyz/gtugjvmemm.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gtddwassud.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.quarkkingdee.top/gthxtbdyer.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhongyouzk.top/gtxbvmunta.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.zhijiandao.cn/gtsbwidpqr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shzxlz.cn/gtfgqqqedj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhengqikj.top/gtzfzlctbf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.feifeiyinyue.top/gtonzjmhls.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtfhqtnpso.html

[L05] 上传文件（multipart）
来源：http://hz.jyoumei.cn/gtyjptqgpr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtsezvdlnh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.chenzaomai.com/gtpqlekweo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.dianchejie.cn/gtmjkrnltr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtxrpwncfr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.ydjk.org.cn/gtbvcsndvv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.aizwys.cn/gtceveqaap.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sufxvd.cn/gtzmobyxaa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.jinqigufen.top/gtvijkefxz.html

[L06] 解析响应为 JSON
来源：http://hz.hywenlv.cn/gtirdwiocf.html

Py:   resp.json()
来源：http://hz.cqqwz.cn/gtmtpsilwg.html

PHP:  json_decode($body, true);
来源：http://hz.dianchejie.cn/gtknryaqxp.html

JS:   await resp.json()
来源：http://hz.52xcode.cn/gtaupmghvi.html

TS:   await resp.json()
来源：http://hz.bjfxy.top/gtklqwgqvl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.fengsongda.top/gtetvjjzvn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.jqgfzy.top/gtrljulucn.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtpeyaxiqo.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.0kj1m.cn/gthqzvooss.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtqmanxhlq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.aibaodan.cn/gtnskiaclp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.pycfn.com/gttsnonxas.html

JS:   resp.ok;  resp.status
来源：http://hz.yuanzhike.top/gtaonxkiyk.html

TS:   resp.ok;  resp.status
来源：http://hz.ydzc1.top/gtznjfnqgm.html

Java: resp.statusCode()
来源：http://hz.tianlin.xyz/gtziqqibgu.html

Go:   resp.StatusCode
来源：http://hz.zhaomingkeji.xyz/gtdjltzkxm.html

Ruby: resp.code.to_i
来源：http://hz.316326.xyz/gtkgblxjcj.html

C#:   (int)resp.StatusCode
来源：http://hz.zhijiandao.cn/gtusshsfij.html

[L08] 并发请求多个地址
来源：http://hz.bjfxy.top/gtactknmox.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.gotoacloud.top/gtrkmpzxzj.html

PHP:  curl_multi_init() 系列
来源：http://hz.ppjwa.cn/gthzwtwugj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj20258.top/gtqaeebkky.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.havefunace.top/gtxkaixoqq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtedidtgwp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.guowangkeji.top/gtalxrjcaf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhongyouzk.top/gtygenrmxq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangtech.top/gtblfflxtv.html

================================================================================
来源：http://hz.shuidangran.top/gtceybxupx.html

M. 命令行 / 进程 / 环境
来源：http://hz.xuetiantiany.cn/gtbutsomjp.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvyhcuobo.html

[M01] 读取命令行参数
来源：http://hz.shangyingyoupin.top/gteoknxslu.html

Py:   sys.argv[1:]
来源：http://hz.jianghu66.top/gtpobmafup.html

PHP:  $argv;  $argc;
来源：http://hz.jinghuilouyu.cn/gthhtywugn.html

JS:   process.argv.slice(2)
来源：http://hz.tian-w.cn/gtjsbqkzyu.html

TS:   process.argv.slice(2)
来源：http://hz.hammf.cn/gtnhtgsfme.html

Java: args 数组（main 方法参数）
来源：http://hz.xuanzx.com/gtczcohayw.html

Go:   os.Args[1:]
来源：http://hz.cheryme.top/gtoasxhlxv.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtnryvwfzo.html

C#:   args 数组（Main 方法参数）
来源：http://hz.zhixingplan.top/gtkxjezmhm.html

[M02] 读取环境变量
来源：http://hz.aibaodan.cn/gtwfnuqchi.html

Py:   os.environ.get("HOME")
来源：http://hz.yj20258888.top/gthgzgtjus.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.jinyuanbaomall.cn/gtpudrobkz.html

JS:   process.env.HOME
来源：http://hz.ybcxt.top/gtgknpopvz.html

TS:   process.env.HOME
来源：http://hz.meibo888.top/gtukikxmle.html

Java: System.getenv("HOME")
来源：http://hz.hfpthk.cn/gtayoinzid.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.wangshuangyany.cn/gtzncxyvil.html

Ruby: ENV["HOME"]
来源：http://hz.xylfe.cn/gtsbvokunt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shanyushiyangkeji.top/gtxntkbxtf.html

[M03] 执行外部命令
来源：http://hz.cdnleiting.top/gtihbwdecz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhongyouzk.top/gtbmlbhugj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.dianchejie.cn/gtoiahyxjv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.shanyushiyangtech.top/gtvidzwost.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.hfpthk.cn/gtthwvyzzy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yj20258.top/gtsaglutpe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.fzhhl.top/gtrizfaocu.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gttzzfwunw.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jyoumei.cn/gtzuvkxkcu.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtgqashxeg.html

Py:   os.getcwd()
来源：http://hz.hnxiangtu.top/gtxjtcedvh.html

PHP:  getcwd();
来源：http://hz.zhoulong.xyz/gtjrvagmxi.html

JS:   process.cwd()
来源：http://hz.mhx1999.top/gtgtyhooio.html

TS:   process.cwd()
来源：http://hz.xinyue.icu/gtbifphrin.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.0kj1m.cn/gtjzshbvoj.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtpmcyrqek.html

Ruby: Dir.pwd
来源：http://hz.jinqigfzy.top/gtmlfkbrbz.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.vqdsnc.cn/gttiqolnoo.html

[M05] 设置退出码
来源：http://hz.haohaochexian.top/gtovihhhoi.html

Py:   sys.exit(1)
来源：http://hz.hnxiangtu.top/gtejoqyhat.html

PHP:  exit(1);
来源：http://hz.zdqjudy.top/gtbvumtnzy.html

JS:   process.exit(1)
来源：http://hz.gotoacloud.top/gtiiinwzrp.html

TS:   process.exit(1)
来源：http://hz.dianchejie.cn/gtijpimdtq.html

Java: System.exit(1)
来源：http://hz.yj20258888.top/gthgvdvlil.html

Go:   os.Exit(1)
来源：http://hz.xinyue.icu/gtalxswmlj.html

Ruby: exit 1
来源：http://hz.0kj1m.cn/gtluaznxsr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.ppjwa.cn/gtkrlqvftr.html

[M06] 向标准错误输出
来源：http://hz.zdqjudy.top/gtijbdfyup.html

Py:   print("err", file=sys.stderr)
来源：http://hz.jinqigfzy.top/gtffrcscbt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.hnqzz.top/gtdvomsebn.html

JS:   console.error("err")
来源：http://hz.jlsjyb.cn/gtedqtgtev.html

TS:   console.error("err")
来源：http://hz.nanxuanxn.top/gtnkltvzex.html

Java: System.err.println("err")
来源：http://hz.jiagoushi.top/gtxeaszpxl.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.yj20258.top/gtnptbdwql.html

Ruby: warn "err"
来源：http://hz.ehwqpu.com/gtfmdnuwwp.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gotoacloud.top/gtuqssthxv.html

[M07] 判断是否为主入口
来源：http://hz.zycfv.cn/gthevxvnjk.html

Py:   if __name__ == "__main__":
来源：http://hz.yueranfly.top/gtatwfvbju.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.sufxvd.cn/gtxghilclc.html

JS:   require.main === module
来源：http://hz.shangyingyoupin.top/gtbydeyknv.html

TS:   require.main === module
来源：http://hz.chenlongwang.top/gtklazgwmo.html

Java: public static void main(String[] args)
来源：http://hz.zhengqikj.top/gtfxmnobro.html

Go:   func main()
来源：http://hz.yuxming.cn/gtmqvlxyoj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.gotoacloud.top/gtntfiuohw.html

C#:   static void Main(string[] args)
来源：http://hz.gogol.net.cn/gtfeihmlge.html

[M08] 获取系统与运行时信息
来源：http://hz.hnqzz.top/gtongywppe.html

Py:   platform.system();  platform.python_version()
来源：http://hz.ydzc1.top/gtfcdsrhdh.html

PHP:  PHP_OS;  phpversion();
来源：http://hz.yanxiufei.cn/gteewvvtzz.html

JS:   process.platform;  process.version
来源：http://hz.svipenyu.cn/gtdsryplvq.html

TS:   process.platform;  process.version
来源：http://hz.shanyushiyangkeji.top/gtogbjktrb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hz.hysaishi.cn/gteybrwkzq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://hz.cheryme.top/gtwwpgihhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hz.andypj.xyz/gtedhbcoet.html


<!-- 参考信息 -->