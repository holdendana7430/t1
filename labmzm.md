代发 wailian999

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gteryjenhy.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtamvjpjed.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtystxrtbq.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtwxsmerox.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtdxikexqu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gthuomljql.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtmxnhkvtv.html

TS:   d.toISOString()
来源：http://hz.hnqzz.top/gtaxifovud.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtlytbngwq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtqwmcfbjy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hfpthk.cn/gtuszzitbo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtswjgtalv.html

[J03] 字符串解析为日期
来源：http://hz.0kj1m.cn/gtwluzjagv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtnzhfglfa.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuetiantiany.cn/gtozrineuf.html

JS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtqfmjreqw.html

TS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtcctpogsf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtzskaqkek.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhijiandao.cn/gtlyupbafo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtiseowmaf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtfrcrbwon.html

[J04] 时间戳与日期互转
来源：http://hz.hnqzz.top/gtmfcsxexf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtsvssemot.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtkbzkfgza.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtfhemhxyr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtzflpngma.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtvmijpbja.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtwxshuxya.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtkmntbtwj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gthaxlzfpo.html

[J05] 时间加减（加 7 天）
来源：http://hz.0kj1m.cn/gtucmsiqoz.html

Py:   now + timedelta(days=7)
来源：http://hz.ivvv.top/gtmcjygywh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cqqwz.cn/gtkgafvokg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtmxqpxubo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtagwamefb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtqlzxhkal.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtiprdnohp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtrcsjdbky.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hfpthk.cn/gtifmpmmek.html

[J06] 计算两时间之差
来源：http://hz.haohaochexian.top/gtfgalujqe.html

Py:   (end - start).total_seconds()
来源：http://hz.jinghuilouyu.cn/gtkqwcfuxs.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtpkiatglj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtypbncekg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yuanzhike.top/gtocribigy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtahpisuhp.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtbveykrjp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtyecxfene.html

C#:   (end - start).TotalSeconds
来源：http://hz.sweek.top/gtnrjrvsft.html

[J07] 比较两个日期
来源：http://hz.jinqigfzy.top/gtesiddxgv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gttcnchmfl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtikdggrhi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtyarxyjrx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtuhcdumqf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shangyingyoupin.top/gtmaqzhppw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hongshengwenyu.top/gtpsbtknlq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtevpmqapy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtkshdxxfx.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtzcbfmbei.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ywan-chungtsiang.top/gtatkcqomp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cheryme.top/gtrovayide.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtsoisizyg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtwrzwumco.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gthvlrhppm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.smart0.xyz/gtojuneqft.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gteplsmpdh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtxiumrxhf.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtxhtuwfge.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtexksjjzy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gthjqlvwoi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtitmenfzd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtmaqffmkw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtirwtrnjz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtgemmccog.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtiqpfydhc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xinyue.icu/gtooetjfax.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gtqqeslvuh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ppjwa.cn/gtsvoxzjrz.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.birdmap.top/gtfbgrfeef.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtgrqitamm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gthwqlmqmr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ppjwa.cn/gtkkraydnn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtojctlztt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gttqvrqhdc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gtpbvefhtr.html

================================================================================
来源：http://hz.guowangkeji.top/gtobqmcqck.html

K. JSON 与序列化
来源：http://hz.yj202588.top/gtugcjnlzq.html

================================================================================
来源：http://hz.chenlongwang.top/gtrvhqmqqu.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtmyobtcmo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gogol.net.cn/gtasjhdonx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtoeywqkpq.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtgotvfaoy.html

TS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtugkgkgam.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtttpjuxqk.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtryzjstvv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xinyue.icu/gtzoruljvb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tian-w.cn/gttkczyzoi.html

[K02] JSON 字符串转对象
来源：http://hz.sweek.top/gtqjzltcpi.html

Py:   json.loads(s)
来源：http://hz.ydjk.org.cn/gtjlnzyzyw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cheryme.top/gtmsynxdxo.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtfzpmzadc.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtvbidgwxd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gteyoyclrd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tianlin.xyz/gtegghtwyo.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtjshmesod.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangshuangyany.cn/gtvftrdacp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cqqwz.cn/gtxepowage.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtsctizenh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtrrafjdet.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xylfe.cn/gtojsfyary.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtrilcdtsr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhixingplan.top/gtfqxlmkve.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guowangkeji.top/gtksuwueej.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtcsgcnciz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gtuigbyrok.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtgxvuqldw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.316326.xyz/gtielbujsr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtwoileora.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtsyzlpmno.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtladsjggw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cashguo.top/gtljxmzdtn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hywenlv.cn/gtssqltpwj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtkeepxfzx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhongyouzk.top/gtyaeynhgd.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gtcykupgvy.html

Py:   copy.deepcopy(obj)
来源：http://hz.yonumen.top/gtwxmfpach.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtezqflqoy.html

JS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtjbigyums.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtzpanscom.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtgjwqvyft.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj202588.top/gttwyghdrj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtqxyfqswc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtuyuhsgsd.html

[K06] 解析 URL 查询串
来源：http://hz.mhx1999.top/gthtarcsut.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtcbwtlcel.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gtzyanikyw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258888.top/gtwbjhuiio.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.vqdsnc.cn/gtjwyvpein.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guowangkeji.top/gtlmmgtnej.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shuidangran.top/gtrjrpiaca.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.bjfxy.top/gtbwzhluwd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gtzdwrdfxg.html

[K07] 进制转换
来源：http://hz.sufxvd.cn/gtblyignvz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yvedp.cn/gtmvskorxg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtvyricnaz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jlsjyb.cn/gtdmocadrl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sysykeji.top/gtmqclfwcv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gttgspsrqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtserwqift.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yonumen.top/gtfsucbwax.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yueranfly.top/gtldxjdcij.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ybcxt.top/gtxjwuwitf.html

Py:   pickle.dumps(obj)
来源：http://hz.sxryk.cn/gtpzxvckcn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtaxmfklpw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinyuanbaomall.cn/gtfxpbgabd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtdibshjim.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gttmqwmmdx.html

Go:   encoding/gob
来源：http://hz.yj202588.top/gtiokdmkcl.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gttsttaork.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtatufoqnl.html

================================================================================
来源：http://hz.zhixingplan.top/gtjooomnkn.html

L. 网络请求
来源：http://hz.yonumen.top/gthhjmdzjx.html

================================================================================
来源：http://hz.yj20258.top/gtrybztkfp.html

[L01] 发送 GET 请求
来源：http://hz.hongshengwenyu.top/gtdjbgmnak.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtdhsluuoa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtgtkrntlj.html

JS:   await fetch(url)
来源：http://hz.chenzaomai.com/gtumjvargf.html

TS:   await fetch(url)
来源：http://hz.zhongyouzk.top/gtmndssuxt.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.daxiang520.top/gtgodfcxqu.html

Go:   resp, err := http.Get(url)
来源：http://hz.hfpthk.cn/gtlmjudzei.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtomuzpnte.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnxiangtu.top/gttmestjlu.html

[L02] 发送 POST JSON
来源：http://hz.52xcode.cn/gtfaykgvfm.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.kuanghao11.cn/gtdawsnyzi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.jiagoushi.top/gtotishhqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.haohaochexian.top/gthqjlagfa.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtnooajadl.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.pengpengdd.cyou/gtdhfurune.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.aibaodan.cn/gtbhqjsszd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tianlin.xyz/gtmuhqndbq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.tanke756.top/gtkdtwdgqg.html

[L03] 设置自定义请求头
来源：http://hz.ivvv.top/gtmmluzptn.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinghuilouyu.cn/gtgrwdprgf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.fengsongda.top/gtpwtazgdf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.redwolf501.top/gtcadgtfgr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtmfjrwfiw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.smart0.xyz/gtedtzzcdl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.nanxuanxn.top/gtmwrxpndq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hysaishi.cn/gtovlqqrmr.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xylfe.cn/gtvnnnkbat.html

[L04] 设置超时
来源：http://hz.chenjidiqi.icu/gtswfilnec.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gtandaeiyu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yj202588.top/gtmfkxwgnz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.guannengcc.top/gteplbirar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tianlin.xyz/gtgadgfkon.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fengsongda.top/gtepyarwnj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.shuidangran.top/gthsaanria.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jinqigfzy.top/gtwozkhttm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tianlin.xyz/gtxkkeprgi.html

[L05] 上传文件（multipart）
来源：http://hz.gaohongyu789.top/gtlubozvab.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.yj202588.top/gtpiecxkbz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtfcvtbljr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.quarkkingdee.top/gtvsnayyag.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtwmcwbzkc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yuxming.cn/gtuogziiix.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jlsjyb.cn/gteneavtzy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.sysykeji.top/gtwgehesml.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtwevwdoum.html

[L06] 解析响应为 JSON
来源：http://hz.chenjidiqi.icu/gtmedumdjp.html

Py:   resp.json()
来源：http://hz.zhongyouzk.top/gtvscfhsbr.html

PHP:  json_decode($body, true);
来源：http://hz.jqgufenzy.top/gtsowcpmud.html

JS:   await resp.json()
来源：http://hz.zhongyouzk.top/gtpgfwgatu.html

TS:   await resp.json()
来源：http://hz.zhiwuduotai.top/gtfcqufmks.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dianchejie.cn/gtxojzngdk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.yuxming.cn/gtkokxfzcw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.cucudq.cn/gtbasaulls.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.dianchejie.cn/gtchophmjn.html

[L07] 处理 HTTP 状态码
来源：http://hz.shuidangran.top/gtvqwxlwtc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.shangyingyoupin.top/gtpurtpkfd.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtxfatpvdx.html

JS:   resp.ok;  resp.status
来源：http://hz.xuetiantiany.cn/gtprkwkvlp.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtuqpdykdd.html

Java: resp.statusCode()
来源：http://hz.chenzaomai.com/gttbhywokc.html

Go:   resp.StatusCode
来源：http://hz.zycfv.cn/gtgcfylylf.html

Ruby: resp.code.to_i
来源：http://hz.sxryk.cn/gtsbeunima.html

C#:   (int)resp.StatusCode
来源：http://hz.mhx1999.top/gtayrzlmbr.html

[L08] 并发请求多个地址
来源：http://hz.nanxinkj.top/gthgdaxbda.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.dianchejie.cn/gtljbqusty.html

PHP:  curl_multi_init() 系列
来源：http://hz.gogol.net.cn/gthnrckvuc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yanxiufei.cn/gtblzconsy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.xziqi.cn/gtieijfpvn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.hywenlv.cn/gtgfigslos.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.cashguo.top/gtywebjlfh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gtfuxyaxwi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.jianghu66.top/gtmncodbtk.html

================================================================================
来源：http://hz.sweek.top/gtdghlhalg.html

M. 命令行 / 进程 / 环境
来源：http://hz.hongshengwenyu.top/gtbjoadyni.html

================================================================================
来源：http://hz.gogol.net.cn/gtaqvjvtfs.html

[M01] 读取命令行参数
来源：http://hz.c1oappe.top/gttjnuwluo.html

Py:   sys.argv[1:]
来源：http://hz.shzxlz.cn/gtxwmxhgsr.html

PHP:  $argv;  $argc;
来源：http://hz.shzxlz.cn/gtslntxhcx.html

JS:   process.argv.slice(2)
来源：http://hz.zhixingplan.top/gtyqtarazz.html

TS:   process.argv.slice(2)
来源：http://hz.daxiang520.top/gtipqhnvwm.html

Java: args 数组（main 方法参数）
来源：http://hz.jinqigfzy.top/gtseqmwmvz.html

Go:   os.Args[1:]
来源：http://hz.0kj1m.cn/gteypsfheo.html

Ruby: ARGV
来源：http://hz.xuetiantiany.cn/gtnljuqoki.html

C#:   args 数组（Main 方法参数）
来源：http://hz.jinghuilouyu.cn/gtgxvezfkz.html

[M02] 读取环境变量
来源：http://hz.quarkkingdee.top/gthkqyickt.html

Py:   os.environ.get("HOME")
来源：http://hz.kuanghao11.cn/gtaygnwqya.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.hongshengwenyu.top/gtzyuebokm.html

JS:   process.env.HOME
来源：http://hz.jianghu66.top/gtsgwvuczo.html

TS:   process.env.HOME
来源：http://hz.yvedp.cn/gtnpayxmoi.html

Java: System.getenv("HOME")
来源：http://hz.sweek.top/gtjzrilibg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yangfankeji.com/gtgyhtoegy.html

Ruby: ENV["HOME"]
来源：http://hz.cashguo.top/gtnmguccfl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.shzxlz.cn/gtusaktboo.html

[M03] 执行外部命令
来源：http://hz.xuanzx.com/gtdconlyps.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.redwolf501.top/gtvymkuzkv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.yonumen.top/gtedxxhafw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.svipenyu.cn/gtmqmeedxd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.ywan-chungtsiang.top/gtizcoxuxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.jiagoushi.top/gtrfxolrfe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gtkdapwkux.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.sufxvd.cn/gtpkhcrhfm.html

C#:   Process.Start("ls", "-l");
来源：http://hz.jinyuanbaomall.cn/gthsfgakgi.html

[M04] 获取当前工作目录
来源：http://hz.cheryme.top/gtajrisqub.html

Py:   os.getcwd()
来源：http://hz.iojbl.cn/gtaeohxrkt.html

PHP:  getcwd();
来源：http://hz.nanxinkj.top/gtizbytvdb.html

JS:   process.cwd()
来源：http://hz.shanyushiyangkeji.top/gtximzhaxn.html

TS:   process.cwd()
来源：http://hz.zdqjudy.top/gtoixqowum.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.bjfxy.top/gtqsjtbnjw.html

Go:   os.Getwd()
来源：http://hz.fzhhl.top/gtaqrtlaij.html

Ruby: Dir.pwd
来源：http://hz.wangdashe.top/gtdhhahwvt.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.yuanzhike.top/gtgjcdvbie.html

[M05] 设置退出码
来源：http://hz.fengsongda.top/gtihhliwlh.html

Py:   sys.exit(1)
来源：http://hz.jlsjyb.cn/gtywxmziam.html

PHP:  exit(1);
来源：http://hz.jinqigufen.top/gtnhnspdqk.html

JS:   process.exit(1)
来源：http://hz.xinyue.icu/gtmuovukzj.html

TS:   process.exit(1)
来源：http://hz.gogol.net.cn/gtcqlsdeih.html

Java: System.exit(1)
来源：http://hz.jinyuanbaomall.cn/gtohvbpsjk.html

Go:   os.Exit(1)
来源：http://hz.quarkkingdee.top/gthfjtajqu.html

Ruby: exit 1
来源：http://hz.havefunace.top/gtaoamhrea.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hz.shanyushiyangtech.top/gtnjseuycl.html

[M06] 向标准错误输出
来源：http://hz.yongpay.top/gtvcdprtvj.html

Py:   print("err", file=sys.stderr)
来源：http://hz.ppjwa.cn/gtuqvaictj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://hz.sweek.top/gtvijmxakr.html

JS:   console.error("err")
来源：http://hz.hammf.cn/gtwzveyctx.html

TS:   console.error("err")
来源：http://hz.52xcode.cn/gteipbdmgy.html

Java: System.err.println("err")
来源：http://hz.haohaochexian.top/gtbpgstvlb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hz.chenjidiqi.icu/gtliqdcvwu.html

Ruby: warn "err"
来源：http://hz.tianlin.xyz/gtpcqylmwy.html

C#:   Console.Error.WriteLine("err")
来源：http://hz.gaohongyu789.top/gtsgyvabyh.html

[M07] 判断是否为主入口
来源：http://hz.guowangkeji.top/gtcuhtqphn.html

Py:   if __name__ == "__main__":
来源：http://hz.jlsjyb.cn/gttphawqkd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hz.chenjidiqi.icu/gtapbdquid.html

JS:   require.main === module
来源：http://hz.bjfxy.top/gthzznjsxz.html

TS:   require.main === module
来源：http://hz.iojbl.cn/gtcrzuewgv.html

Java: public static void main(String[] args)
来源：http://hz.pycfn.com/gttuprgusp.html

Go:   func main()
来源：http://hz.ehwqpu.com/gtkxkcgtvm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hz.vqdsnc.cn/gtctxfwbcv.html

C#:   static void Main(string[] args)
来源：http://hz.shangyingyoupin.top/gtpktopqbo.html


<!-- 参考信息 -->