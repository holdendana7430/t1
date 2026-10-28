代发 wailian999

J. 日期与时间
来源：http://hz.jinyuanbaomall.cn/gtquhjipvu.html

================================================================================
来源：http://hz.316326.xyz/gtomnkhagd.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtavmkxspi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cheryme.top/gthexanfxt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtmpgrmfpi.html

JS:   new Date();  Date.now()
来源：http://hz.hywenlv.cn/gtpayvojal.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gttdxpcmvw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtisjuhzuz.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtmsyualfi.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtudxxiquh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gticbwbwpf.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtgedlayel.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gthbjabbzk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtkhshfntu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtlhgpuqpc.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtjqovogsh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtbigjihwz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtwkbutpvb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtfopqnycu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gttiyiuxvw.html

[J03] 字符串解析为日期
来源：http://hz.jlsjyb.cn/gttpyewija.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jyoumei.cn/gtfnoqvcvx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pycfn.com/gtpsxxkumy.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtqsfmtsqy.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtckgfttld.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtkudaaaue.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtiugoiqjd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtrfnrxvwe.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gthcylblip.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtmmbdrhvq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xylfe.cn/gtzwohhjmm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtcmiekkix.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtxcnogtxz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.feifeiyinyue.top/gtknaeykiw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtowaqyzke.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtujkwamsj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cashguo.top/gtajvgclci.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gtcpmdrcpb.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gthcrxblaz.html

Py:   now + timedelta(days=7)
来源：http://hz.xuetiantiany.cn/gtbvxcdfbl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtjvshippf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtglntytkl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gticzvudiy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtyjnzhawg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtmqaqpusq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtgrlfvbfv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtruszaivk.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtcdemiglq.html

Py:   (end - start).total_seconds()
来源：http://hz.xuanzx.com/gtnxtmbvtl.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtmlfzjsyx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtekiditqw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gtuizuyurj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gthgvnogit.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gtfsnqbwhp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnqzz.top/gteerngkrw.html

C#:   (end - start).TotalSeconds
来源：http://hz.andypj.xyz/gtwkazlpod.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gtlvgvpxsf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtukzdlmzs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ybcxt.top/gtyifengcj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtmobdgvrv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sysykeji.top/gtqigorzlh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtvanwiqfo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtirijchlm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtcxrxrkjj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtorhyusfg.html

[J08] 提取年月日与星期
来源：http://hz.birdmap.top/gtjjlcngoi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtskritojg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guannengcc.top/gtslwenmpm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtoqxvfaej.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtgqebuqhg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtuhmljjec.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtvrntrnfx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtvilvluqt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtbbdhqkhy.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gtyhmhhfyi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cashguo.top/gtvqphofez.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ehwqpu.com/gttbigfxzd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtdbbutyiw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.c1oappe.top/gtrzvlhfkk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nanxinkj.top/gtwsuazfcd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtdcehdmje.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gtwnvejxtv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhiwuduotai.top/gtpjygpouc.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtdnorhzhg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtwelrswoi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gtijbtwrgo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gterevfvdq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtefkuebnu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtvznqxgdp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtyclgucek.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guannengcc.top/gtsnkhbupq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtnsmkanil.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtoqgohuqh.html

K. JSON 与序列化
来源：http://hz.hammf.cn/gtgxjpiynb.html

================================================================================
来源：http://hz.ydjk.org.cn/gtpzhlsjtm.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhoulong.xyz/gtckbabbns.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gthvzangft.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtnvttktty.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtvizpkfzt.html

TS:   JSON.stringify(obj)
来源：http://hz.ybcxt.top/gtnsoomhdp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtqdjusurf.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gtyvxhnqdi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtlvrmtmrz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtqkghaemd.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gtdjdzkogd.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtmxeobskb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gthksyjpmu.html

JS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtzkukvykk.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtqddcvsbn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.svipenyu.cn/gtpffvlmdw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtxnuslgfg.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtgyqhyrhg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gthozsndjq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtsubymbkj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtvmxnoref.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.quarkkingdee.top/gtyywqprqx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtwmlxngoa.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtqiykhvyj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtghlenusl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hfpthk.cn/gtsxcypsfm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.iojbl.cn/gtutbiould.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gtatpxovwb.html

[K04] 读取 JSON 文件
来源：http://hz.redwolf501.top/gtmtynxyfm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtzepdaqyt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sufxvd.cn/gtgdbopuxf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gttqbckhrf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtlkrltmtx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yanxiufei.cn/gttoqeekpw.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtyoktywtg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtsbumcpfz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sufxvd.cn/gtawwbmzsr.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtehrwntgt.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtxxkcfoxi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtxujseorh.html

JS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtqtkilbnh.html

TS:   structuredClone(obj)
来源：http://hz.smart0.xyz/gtredwzxth.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xziqi.cn/gtonqmomzx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtqksyzvcz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daxiang520.top/gtcnkfwdya.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtrnfmfzmp.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtlmfrfrod.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.shzxlz.cn/gtkndnggdd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtrclfkdgx.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtjozpayqy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gzhubu.top/gtqdleuqpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtttthbksk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.svipenyu.cn/gtqgbpivpu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtukrmurgo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gtqgiftfwj.html

[K07] 进制转换
来源：http://hz.c1oappe.top/gtpvfttfks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydjk.org.cn/gtmuqqxddf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.zhoulong.xyz/gtgzuljnys.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtoqqtiorw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtofldkgnl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtzkqglzoo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jqgfzy.top/gtrbhoszav.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtqtifashc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sxryk.cn/gtcuencmfo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhaomingkeji.xyz/gthhfsugto.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtjckekjdc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.snrcjt.cn/gtdoqgdspx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtinucxbcf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yuanzhike.top/gteewwodom.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.snrcjt.cn/gtpbdgryrv.html

Go:   encoding/gob
来源：http://hz.yj20258888.top/gtxbjpaxsk.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gtgtyyakhn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnxiangtu.top/gtyiunjqpi.html

================================================================================
来源：http://hz.ppjwa.cn/gtrywsusdy.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtxfvufcqx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtozwkspll.html

[L01] 发送 GET 请求
来源：http://hz.ehwqpu.com/gtdibrvptm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtiyqflspd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenzaomai.com/gttyfegyil.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtsukxxwzu.html

TS:   await fetch(url)
来源：http://hz.jqgufenzy.top/gtzzpwhcew.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yongpay.top/gtcvzqcbtu.html

Go:   resp, err := http.Get(url)
来源：http://hz.jianghu66.top/gtlhsmpzzd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ywan-chungtsiang.top/gtmyexbgzk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.pengpengdd.cyou/gthymlopmj.html

[L02] 发送 POST JSON
来源：http://hz.smart0.xyz/gtxszbujlf.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.0kj1m.cn/gtoxjdqynn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gtbbjvqylu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtnxtrlcgk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtevbdhgzq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jiagoushi.top/gtojchtjoz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.zhijiandao.cn/gtpmacjdtd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.wangdashe.top/gtigwonzml.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.pycfn.com/gtfpnthuug.html

[L03] 设置自定义请求头
来源：http://hz.52xcode.cn/gtvenbntrn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuanzx.com/gtqodslofl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.hongshengwenyu.top/gtarygqaep.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jlsjyb.cn/gttmzdfxgt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhoulong.xyz/gtykcxynug.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.shanyushiyangtech.top/gtmkjxonhn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.aizwys.cn/gtaggjtdgx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.316326.xyz/gtcvieevwo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.tianlin.xyz/gtpzaxozsq.html

[L04] 设置超时
来源：http://hz.tian-w.cn/gtxaxwuyhv.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gzhubu.top/gtqelczskq.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhengqikj.top/gteylsbobb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtfwuuvqhl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jlsjyb.cn/gtyzywrnig.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.tianlin.xyz/gtlvltmqxw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.jinqigufen.top/gtlegblsyb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.iojbl.cn/gteexifgoz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.shanyushiyangtech.top/gtexybpglu.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtslrdzhtr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nwbrower.top/gtyadmrfyt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.hammf.cn/gtromhowzo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.316326.xyz/gtowxxrxkg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gthraffwlx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.9152youxi.cn/gtelpmilxr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.shangyingyoupin.top/gtjgpwvemp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.aizwys.cn/gtabpreeab.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.zhijiandao.cn/gtrkrbmhez.html

[L06] 解析响应为 JSON
来源：http://hz.guannengcc.top/gtqtxfoqab.html

Py:   resp.json()
来源：http://hz.redwolf501.top/gtpegsjuxp.html

PHP:  json_decode($body, true);
来源：http://hz.aibaodan.cn/gtcqdzqgnn.html

JS:   await resp.json()
来源：http://hz.jinqigufen.top/gtxlcloycb.html

TS:   await resp.json()
来源：http://hz.gogol.net.cn/gtukxbujcg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtgypymjhr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.guannengcc.top/gtnzlejgto.html

Ruby: JSON.parse(resp.body)
来源：http://hz.zhengqikj.top/gtammolfws.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.wangshuangyany.cn/gtjuhfdazb.html

[L07] 处理 HTTP 状态码
来源：http://hz.nanxuanxn.top/gtteqrvzja.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.jinqigfzy.top/gtmcwzfubc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.wangdashe.top/gtzrgfzwpa.html

JS:   resp.ok;  resp.status
来源：http://hz.haohaochexian.top/gtugwqfhfj.html

TS:   resp.ok;  resp.status
来源：http://hz.hongshengwenyu.top/gtaimiqokv.html

Java: resp.statusCode()
来源：http://hz.nanxuanxn.top/gtpjavdpia.html

Go:   resp.StatusCode
来源：http://hz.tanke756.top/gtbomdjymg.html

Ruby: resp.code.to_i
来源：http://hz.shanyushiyangkeji.top/gtrtggguhf.html

C#:   (int)resp.StatusCode
来源：http://hz.redwolf501.top/gtqquuzwnt.html

[L08] 并发请求多个地址
来源：http://hz.ybcxt.top/gtxlynzypf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dashuyun.cn/gtusbfwdhs.html

PHP:  curl_multi_init() 系列
来源：http://hz.zhijiandao.cn/gtctvrxnte.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.fzhhl.top/gtbqvdzziw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtnhhyzzdi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.pengpengdd.cyou/gtuxcnqqed.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.ivvv.top/gtfunfblzt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.hywenlv.cn/gtxdnxxnyb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.gogol.net.cn/gtudfbiqst.html

================================================================================
来源：http://hz.jinqigfzy.top/gtpnklcnjg.html

M. 命令行 / 进程 / 环境
来源：http://hz.shanyushiyangkeji.top/gtdzvnbspv.html

================================================================================
来源：http://hz.jinqigfzy.top/gtosvvslci.html

[M01] 读取命令行参数
来源：http://hz.shanyushiyangtech.top/gtxtingrld.html

Py:   sys.argv[1:]
来源：http://hz.gogol.net.cn/gtbzilsttj.html

PHP:  $argv;  $argc;
来源：http://hz.mhx1999.top/gtbowmpfzu.html

JS:   process.argv.slice(2)
来源：http://hz.zycfv.cn/gtdtrqlslm.html

TS:   process.argv.slice(2)
来源：http://hz.sweek.top/gtgvbnjnrg.html

Java: args 数组（main 方法参数）
来源：http://hz.zhixingplan.top/gtvvfvqzdi.html

Go:   os.Args[1:]
来源：http://hz.yongpay.top/gthmlapfeg.html

Ruby: ARGV
来源：http://hz.dashuyun.cn/gtjqydbszy.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtdrshwrxh.html

[M02] 读取环境变量
来源：http://hz.yj20258888.top/gtktzhjunx.html

Py:   os.environ.get("HOME")
来源：http://hz.gzhubu.top/gtqsjgypws.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.zhixingplan.top/gttwfwoteb.html

JS:   process.env.HOME
来源：http://hz.jyoumei.cn/gtfhwvjpsm.html

TS:   process.env.HOME
来源：http://hz.tanke756.top/gtidzgwbxy.html

Java: System.getenv("HOME")
来源：http://hz.yj202588.top/gtdtwytjvr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.meibo888.top/gtprkwyjpx.html

Ruby: ENV["HOME"]
来源：http://hz.zhijiandao.cn/gtgsjausjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenjidiqi.icu/gtoizpsxur.html

[M03] 执行外部命令
来源：http://hz.jinqigfzy.top/gtmfmxouix.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.gaohongyu789.top/gtbvlfdmxv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.ybcxt.top/gtbfpjuknn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yanxiufei.cn/gtxprjbubn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.guannengcc.top/gtjorifsbx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.daria6918.cn/gtwazgfvkq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.pycfn.com/gtsqsgndpw.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.jlsjyb.cn/gthyvpmipz.html

C#:   Process.Start("ls", "-l");
来源：http://hz.haohaochexian.top/gtoniwznsx.html

[M04] 获取当前工作目录
来源：http://hz.ywan-chungtsiang.top/gtdkamgutc.html

Py:   os.getcwd()
来源：http://hz.yuxming.cn/gtzfogyrdn.html

PHP:  getcwd();
来源：http://hz.yanxiufei.cn/gtmtzfsynb.html

JS:   process.cwd()
来源：http://hz.sysykeji.top/gttkxeygle.html

TS:   process.cwd()
来源：http://hz.daria6918.cn/gtojjwjgya.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.aibaodan.cn/gtvlncphjb.html

Go:   os.Getwd()
来源：http://hz.jinqigfzy.top/gthqoiytfk.html

Ruby: Dir.pwd
来源：http://hz.fzhhl.top/gtflfyhnwt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.jyoumei.cn/gtkutkwnbh.html

[M05] 设置退出码
来源：http://hz.xylfe.cn/gtjwztodgu.html

Py:   sys.exit(1)
来源：http://hz.daria6918.cn/gtmzkewlqy.html

PHP:  exit(1);
来源：http://hz.yj202588.top/gtxundilzx.html

JS:   process.exit(1)
来源：http://hz.jianghu66.top/gtpxmczxuv.html

TS:   process.exit(1)
来源：http://hz.gaohongyu789.top/gtlehpdxzs.html

Java: System.exit(1)
来源：http://hz.wangdashe.top/gtvhbamamw.html

Go:   os.Exit(1)
来源：http://hz.yonumen.top/gtuwcytscw.html

Ruby: exit 1
来源：http://hz.zhijiandao.cn/gtzwekrici.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.kuanghao11.cn/gtcseewgso.html

[M06] 向标准错误输出
来源：http://hz.zhongyouzk.top/gtjlkgbuea.html

Py:   print("err", file=sys.stderr)
来源：http://hz.svipenyu.cn/gtycmwdhkc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.chenjidiqi.icu/gtecrqpkzp.html

JS:   console.error("err")
来源：http://hz.cqqwz.cn/gtcjarzdwm.html

TS:   console.error("err")
来源：http://hz.hnxiangtu.top/gtcbqxwfxn.html

Java: System.err.println("err")
来源：http://hz.pengpengdd.cyou/gthdvwbkhf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.zhoulong.xyz/gtjuimpzcd.html

Ruby: warn "err"
来源：http://hz.xuetiantiany.cn/gtgndpobys.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.yongpay.top/gtoppjbtpy.html

[M07] 判断是否为主入口
来源：http://hz.hammf.cn/gtrqocgwmu.html


<!-- 参考信息 -->