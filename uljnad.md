代发 wailian999

J. 日期与时间
来源：http://hz.xuetiantiany.cn/gtimyccdmk.html

================================================================================
来源：http://hz.daxiang520.top/gtraevvokr.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtwfqtcsyu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtahqbyiix.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtguplwwaa.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtrnwzqivr.html

TS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtgjtozidk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuanzhike.top/gtbddnmklj.html

Go:   time.Now()
来源：http://hz.hammf.cn/gtocwiyfqq.html

Ruby: Time.now
来源：http://hz.tanke756.top/gtbyampiqe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jiagoushi.top/gtfizefhoj.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtcutjjryt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtqyywzres.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtozbcbldr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gttqzoatle.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtbmxggjsf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtpufzftss.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtqgstujba.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtbyzxsxxf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtrveymgvn.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtwmlrdiuh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtzsmpdjmf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigfzy.top/gttwdwdwyx.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gttmrwdane.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtcreczeqz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtabyrgywo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxuanxn.top/gtpirvmaoz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtlwgzncao.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gthfncztyv.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtgmwwmciq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtlricibgn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daxiang520.top/gtkfxltvns.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gtjwiljjon.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtjirmntao.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cucudq.cn/gtzbdfmken.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtwnoynimj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gtaaqhjpxn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtcbnrrgzy.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangtech.top/gteapjlhig.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtqunhpgpr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hywenlv.cn/gtivwdhgln.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtzgcuugep.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtmnoodkie.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtukmsgtqt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtppchmyxx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258.top/gtzegmgnqc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtywsuiwjt.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gtmpwjwldw.html

Py:   (end - start).total_seconds()
来源：http://hz.zhiwuduotai.top/gtgtdvuzaq.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtumlasnqb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenjidiqi.icu/gtmgvhzmyb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangdashe.top/gttnlhzdmi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtrurandbt.html

Go:   end.Sub(start).Hours()
来源：http://hz.gogol.net.cn/gtckrkszml.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yvedp.cn/gtkivsyfsv.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtdcdejxel.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gttqbqjdkk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtrxzrfzsq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gternoklwa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtcterpvtb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtzvkmhpnu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtwutjaszn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtycxvbika.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtsppxbzic.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtkpcmmziv.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtacwyrzwk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydjk.org.cn/gtlmamvise.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gtdiamkgqr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daria6918.cn/gtmdeqycos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtmwiaxxjt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hysaishi.cn/gtaqmykhhs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hfpthk.cn/gtpzjohqwb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtkopffkow.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258.top/gtgbxfvydf.html

[J09] 时区处理
来源：http://hz.yj20258.top/gtsmxulqss.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtvfphvxcm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gthixmdbjy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daria6918.cn/gtrqhdywfz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xylfe.cn/gtacqubrco.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gttexjhcki.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gtbsoeqbpu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jlsjyb.cn/gtfdsmfmxv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gteqxmtmmt.html

[J10] 取今天 / 本月第一天
来源：http://hz.cucudq.cn/gtmyesczus.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtnlzsixao.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtfsekqwyz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sysykeji.top/gtsjxhdnem.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtnhtauaci.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fzhhl.top/gtshceksvo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgfzy.top/gtuejdndmm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daxiang520.top/gtelvkkryw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.pycfn.com/gtncbnqgae.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrfaazyja.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtbhhjexfq.html

================================================================================
来源：http://hz.hammf.cn/gtgvojbuba.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtemmdpwkx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtjpbmmghu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtaaymlefx.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtdoqcsdbb.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtoytixvbp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gttttnfyya.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtkgnzbhen.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtswbkfjae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtozfogoto.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtycyelysc.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtzgkqxzfe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtvsppgrsn.html

JS:   JSON.parse(s)
来源：http://hz.jianghu66.top/gthbtfeslj.html

TS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtdxldzvka.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydzc1.top/gtbeheycvu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ivvv.top/gtwbdptowi.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtpxkgkeqe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtfblqrqby.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtcnwcbluj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtaigjqljp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtwfapdxun.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shangyingyoupin.top/gtxftbglxm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtetwimkjn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guannengcc.top/gtisfsmhvb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.9152youxi.cn/gtkishfrfp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jianghu66.top/gtfgnhmvdn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtotlyoxfv.html

[K04] 读取 JSON 文件
来源：http://hz.nanxuanxn.top/gttrlshdft.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.dashuyun.cn/gtxlfpaecr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtydlnltnd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtdbnwpwxu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jianghu66.top/gttkwpubim.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jyoumei.cn/gtargmwvry.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aibaodan.cn/gtmpwxmdgd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtpttqfyho.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtsfwxbexg.html

[K05] 深拷贝对象
来源：http://hz.jyoumei.cn/gtmaymrxgm.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtbgtltjrx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtrhglrpyo.html

JS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gteotudqcz.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtffaatekd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.snrcjt.cn/gtqxnobhoc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gteorccvqm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.9152youxi.cn/gtehnyigic.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.316326.xyz/gtxzhzgqmd.html

[K06] 解析 URL 查询串
来源：http://hz.kuanghao11.cn/gtotknyfoh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtowfkdobk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dianchejie.cn/gtvdbbeaqz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtmpihqnjw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtqswcvbuo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yuxming.cn/gtwazrcqwo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigufen.top/gtikwyulgc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtqbqwrwkf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yueranfly.top/gtwmvnprwu.html

[K07] 进制转换
来源：http://hz.hysaishi.cn/gtrqbkkzni.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtzkeuqowq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hongshengwenyu.top/gtgjwcdbci.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtiezmfeeb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtcvajbnrc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtxxqbcfco.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.316326.xyz/gtqwvrwqzj.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sweek.top/gtywmyzthu.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.meibo888.top/gtknowpntn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtcltzhsyp.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtvtkqrogb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnxiangtu.top/gttweqdlfg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guannengcc.top/gtnpdqarms.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.52xcode.cn/gttyzofpvw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.vqdsnc.cn/gtfmiizvfs.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtprnirvty.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtpzywbszi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jlsjyb.cn/gtrxvgbzbt.html

================================================================================
来源：http://hz.svipenyu.cn/gtdjhxqgip.html

L. 网络请求
来源：http://hz.jyoumei.cn/gtpjgkgdgy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlueydikv.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtiuvdlrhi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gotoacloud.top/gtaujyelfy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangshuangyany.cn/gthonfllay.html

JS:   await fetch(url)
来源：http://hz.shzxlz.cn/gtpfkaemsl.html

TS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtcywizdub.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.andypj.xyz/gtretgnqkj.html

Go:   resp, err := http.Get(url)
来源：http://hz.yuanzhike.top/gtpzqctaoa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.jyoumei.cn/gtcheknbrk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ivvv.top/gtdejiosmp.html

[L02] 发送 POST JSON
来源：http://hz.guannengcc.top/gtfmrvvbim.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jinqigfzy.top/gtqmyvjywl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jinyuanbaomall.cn/gtfkosiagv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtkwjxwsry.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daria6918.cn/gttoaxggyy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.andypj.xyz/gtscxmcaqm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yongpay.top/gtosnscepl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.shuidangran.top/gtkafclroa.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zycfv.cn/gtwznnlshw.html

[L03] 设置自定义请求头
来源：http://hz.dianchejie.cn/gtlhxhnazx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gtgzmsprlc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.andypj.xyz/gtqctwuqpk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtfqoyvpnq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.nanxuanxn.top/gtzuegpbjr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.xinyue.icu/gtkbdnrjdy.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.yj202588.top/gtaohhdguz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.zhoulong.xyz/gtqccodpkm.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.kuanghao11.cn/gtwuhgldyb.html

[L04] 设置超时
来源：http://hz.vqdsnc.cn/gtmoshcbys.html

Py:   requests.get(url, timeout=5)
来源：http://hz.yvedp.cn/gttkavtlun.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.bjfxy.top/gtytyqxzfk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.mhx1999.top/gtzmhybgtq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.wangshuangyany.cn/gtpfpmzhbx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.vqdsnc.cn/gtkhgcucll.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.gogol.net.cn/gtufmzwrqg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.cucudq.cn/gtkrlapjse.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nwbrower.top/gtkcxrlwft.html

[L05] 上传文件（multipart）
来源：http://hz.ppjwa.cn/gtcpochndk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.wangshuangyany.cn/gtupnckuhe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.shanyushiyangkeji.top/gtmbqyjhok.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.jyoumei.cn/gtoksrghyl.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.chenjidiqi.icu/gtbwqkpjuv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.shanyushiyangtech.top/gtrbsnzugc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.fzhhl.top/gtrodfymvb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenjidiqi.icu/gtcufymfjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shanyushiyangkeji.top/gtziloihca.html

[L06] 解析响应为 JSON
来源：http://hz.aizwys.cn/gtvdgxolyi.html

Py:   resp.json()
来源：http://hz.zycfv.cn/gttvqgikwn.html

PHP:  json_decode($body, true);
来源：http://hz.chenlongwang.top/gtfgmqdywr.html

JS:   await resp.json()
来源：http://hz.aizwys.cn/gtwgxcleun.html

TS:   await resp.json()
来源：http://hz.snrcjt.cn/gtygmozfff.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.pengpengdd.cyou/gtpabjmzlb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.smart0.xyz/gtafjdeugk.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jqgufenzy.top/gtfhxizqpk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.316326.xyz/gtnrjrlmdh.html

[L07] 处理 HTTP 状态码
来源：http://hz.shzxlz.cn/gtmbbshwkq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.quarkkingdee.top/gtjeugishk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.tian-w.cn/gtfnsgzzko.html

JS:   resp.ok;  resp.status
来源：http://hz.yonumen.top/gtlawchguc.html

TS:   resp.ok;  resp.status
来源：http://hz.nanxuanxn.top/gtbcafxdsx.html

Java: resp.statusCode()
来源：http://hz.hysaishi.cn/gtjcbgsses.html

Go:   resp.StatusCode
来源：http://hz.yongpay.top/gtapfumnco.html

Ruby: resp.code.to_i
来源：http://hz.yj202588.top/gtofcnwgwq.html

C#:   (int)resp.StatusCode
来源：http://hz.birdmap.top/gtermwxihj.html

[L08] 并发请求多个地址
来源：http://hz.ydjk.org.cn/gtwcktyzkv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.hnxiangtu.top/gttwrxvcpv.html

PHP:  curl_multi_init() 系列
来源：http://hz.haohaochexian.top/gtduiuiqlu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.andypj.xyz/gtrwvnvfyi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.iojbl.cn/gtxklzyncd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.tianlin.xyz/gtalbtlxhm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.jyoumei.cn/gtrhyiilqm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtdobztusv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zycfv.cn/gtorycdivt.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrlbofqtv.html

M. 命令行 / 进程 / 环境
来源：http://hz.hnxiangtu.top/gtzeqgqwey.html

================================================================================
来源：http://hz.zhongyouzk.top/gtaosmldad.html

[M01] 读取命令行参数
来源：http://hz.guannengcc.top/gtemjychaj.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtmtohcvaw.html

PHP:  $argv;  $argc;
来源：http://hz.aibaodan.cn/gttthzdahc.html

JS:   process.argv.slice(2)
来源：http://hz.zhoulong.xyz/gtednpjbxu.html

TS:   process.argv.slice(2)
来源：http://hz.c1oappe.top/gtdpatdtla.html

Java: args 数组（main 方法参数）
来源：http://hz.bjfxy.top/gtftazqtcj.html

Go:   os.Args[1:]
来源：http://hz.xinyue.icu/gtcdprxvuq.html

Ruby: ARGV
来源：http://hz.chenlongwang.top/gtyfqpthym.html

C#:   args 数组（Main 方法参数）
来源：http://hz.svipenyu.cn/gtklwfofrs.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gtsundyswn.html

Py:   os.environ.get("HOME")
来源：http://hz.shanyushiyangkeji.top/gteqgcncwt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.cashguo.top/gtkcdfqttu.html

JS:   process.env.HOME
来源：http://hz.zhengqikj.top/gtzfyjdiai.html

TS:   process.env.HOME
来源：http://hz.cheryme.top/gtvwezgkch.html

Java: System.getenv("HOME")
来源：http://hz.jyoumei.cn/gthkbqmiew.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yuxming.cn/gtxmdxkkqs.html

Ruby: ENV["HOME"]
来源：http://hz.redwolf501.top/gtkhrqbshg.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.kuanghao11.cn/gtwnebnctd.html

[M03] 执行外部命令
来源：http://hz.tianlin.xyz/gtwclxhaah.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.zhaomingkeji.xyz/gtzofnehhx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.pengpengdd.cyou/gtscreaswa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.tanke756.top/gtcgwdwswh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.nanxinkj.top/gthlgybpik.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.yvedp.cn/gtxhyinecm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ydzc1.top/gtcanysngp.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yueranfly.top/gtjtepwmjr.html

C#:   Process.Start("ls", "-l");
来源：http://hz.wangshuangyany.cn/gtvldcsxdl.html

[M04] 获取当前工作目录
来源：http://hz.jiagoushi.top/gtgnpfjcwk.html

Py:   os.getcwd()
来源：http://hz.sufxvd.cn/gtyajqnulh.html

PHP:  getcwd();
来源：http://hz.tanke756.top/gtazybparw.html

JS:   process.cwd()
来源：http://hz.smart0.xyz/gtojecoead.html

TS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtjgivxxvl.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.dianchejie.cn/gtylykjndh.html

Go:   os.Getwd()
来源：http://hz.zhengqikj.top/gtqdbvmshg.html

Ruby: Dir.pwd
来源：http://hz.snrcjt.cn/gtzjdhqkms.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.52xcode.cn/gtnsfsmxhh.html

[M05] 设置退出码
来源：http://hz.dianchejie.cn/gtryhzuvok.html

Py:   sys.exit(1)
来源：http://hz.zhiwuduotai.top/gtttdgmoed.html

PHP:  exit(1);
来源：http://hz.yongpay.top/gttemrrbrw.html

JS:   process.exit(1)
来源：http://hz.jlsjyb.cn/gtyhvesuzj.html

TS:   process.exit(1)
来源：http://hz.sweek.top/gtzuklluxh.html

Java: System.exit(1)
来源：http://hz.cucudq.cn/gtwmpjdspz.html

Go:   os.Exit(1)
来源：http://hz.andypj.xyz/gtdtefhlnb.html

Ruby: exit 1
来源：http://hz.pycfn.com/gtksfpolfi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.nanxinkj.top/gtkdkysqqn.html

[M06] 向标准错误输出
来源：http://hz.yj20258.top/gthtqpevnm.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtjsnaiguf.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sxryk.cn/gtqqcpotag.html

JS:   console.error("err")
来源：http://hz.jinqigfzy.top/gtjcoienne.html

TS:   console.error("err")
来源：http://hz.cashguo.top/gtsgqzoyxl.html

Java: System.err.println("err")
来源：http://hz.xziqi.cn/gtkmfkzvsa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.xziqi.cn/gtuxygxqib.html

Ruby: warn "err"
来源：http://hz.shzxlz.cn/gtlbqfgfjs.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.zhoulong.xyz/gtvvvvsvug.html

[M07] 判断是否为主入口
来源：http://hz.kuanghao11.cn/gtqwczsdtt.html


<!-- 参考信息 -->