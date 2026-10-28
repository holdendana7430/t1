代发 wailian999

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gtykadycks.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gtvdwxlevp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.guannengcc.top/gtyrdklmru.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gtlpybsznp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shzxlz.cn/gtvnhjdown.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtedrwvnoh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yueranfly.top/gtqurpasfd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtibyorrbg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gthtzhkvhh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtiovejeyi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yvedp.cn/gtpkjzznav.html

================================================================================
来源：http://hz.guowangkeji.top/gtdopcjzex.html

J. 日期与时间
来源：http://hz.quarkkingdee.top/gtadbptmfi.html

================================================================================
来源：http://hz.iojbl.cn/gtgrsxekqn.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtyzhkiayc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtzfnxitxn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtfzaajnre.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtiirzderq.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtrvyhgcdz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtcqcsannc.html

Go:   time.Now()
来源：http://hz.daxiang520.top/gtrdkwsjce.html

Ruby: Time.now
来源：http://hz.fengsongda.top/gtkfbzlryz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ppjwa.cn/gtcjaxmiqb.html

[J02] 格式化输出
来源：http://hz.xziqi.cn/gtwggiorxr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtwojdyoes.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gttvjhqkys.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangdashe.top/gtxuzbnnlz.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtpmsaxjba.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hongshengwenyu.top/gtqmukupnl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtchukgbii.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtykdafpwg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sxryk.cn/gtiofvzwpn.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gthcyitocm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ybcxt.top/gtnlmehzwm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gttuangixh.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtjdtwuxqd.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtywahwhpb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtpmcizcbk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtxwgecvqh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.aibaodan.cn/gtcvpevktm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gtgosrzcsv.html

[J04] 时间戳与日期互转
来源：http://hz.andypj.xyz/gtwbxjbhkl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.bjfxy.top/gtsmzsergx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtkduapakr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhaomingkeji.xyz/gtdxotspsd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangshuangyany.cn/gtikdkihcp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gttysogpgb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtwxgnnois.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gaohongyu789.top/gtljesvvtl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenzaomai.com/gtnvvjjixc.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtbdlalgxu.html

Py:   now + timedelta(days=7)
来源：http://hz.zhaomingkeji.xyz/gtactzzdcy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hysaishi.cn/gtqyzqksdv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtjoiaiobq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtgrbjurjc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zdqjudy.top/gtjsdkihdq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtxlcyqdfe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.redwolf501.top/gtxbavmovi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hfpthk.cn/gtdldlzzak.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gttcgxecmz.html

Py:   (end - start).total_seconds()
来源：http://hz.hnqzz.top/gtdqnufxqt.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtjkycbmhq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtvuxdgpje.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtcgdvivrk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtziqychop.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtcgwepiyn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.c1oappe.top/gtadtagnjn.html

C#:   (end - start).TotalSeconds
来源：http://hz.nwbrower.top/gtkjrcvuij.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gteumlvhsc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtiajpjjkx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtrvkqatbl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtofxuxqco.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtmesxhrvv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtixpjzpmp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tian-w.cn/gtjmgvyvrc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtbbmpqwfa.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtndrsjskf.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtdwvdtwce.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtntrvuauy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zycfv.cn/gtcagtunly.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhengqikj.top/gtebwhexhv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tianlin.xyz/gtqjbdwoez.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtmlvjhakw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtrwvnlinb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtcvfohokh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtdfbxodki.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gteaskwobq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtczfiadwf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sufxvd.cn/gtkfquuslt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhijiandao.cn/gttygncxiw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.redwolf501.top/gtyugjdicp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtmghpdpyc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtllobimlu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtbqbnxtnz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hfpthk.cn/gtgeotrbtc.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtijamedku.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sweek.top/gtwlmboodf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtvozuhmdq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.guannengcc.top/gtxbynwpgr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtnbbzxgut.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtznuajjzw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtcfipauhl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sxryk.cn/gtilglcdmx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtiziiuuxb.html

================================================================================
来源：http://hz.jlsjyb.cn/gtyrpfvfwx.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gturtakuil.html

================================================================================
来源：http://hz.gaohongyu789.top/gtifoyrcrt.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtethyorms.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtvvrhnesb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtpltwhrwu.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtmbnlegrp.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtbvsubbng.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.vqdsnc.cn/gtszpqqbzi.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gthshxmbyi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tanke756.top/gtujcnebrn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtvethprzc.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtgwrpvkqy.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtqqhfvjtm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtagnmrlbk.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtziiaejrj.html

TS:   JSON.parse(s)
来源：http://hz.pycfn.com/gtibgpwvbe.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gtsfxevoft.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gthenrtzvw.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtbaagntcq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.316326.xyz/gtmpfhyird.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgufenzy.top/gthllvvcbl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hammf.cn/gtemclyfst.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtnkwdhqfj.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhijiandao.cn/gtlgrlowtf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtgwgdrhih.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gttlppeyqp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtdsuolbaa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtnhldiqwn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangshuangyany.cn/gtwvusbpah.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtyajmhnem.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuetiantiany.cn/gtdaphyemi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtddjlfekd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtyjulvhmj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtaausnvoy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shangyingyoupin.top/gtjqneejlg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtweosbltf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gtrqmjkjol.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhengqikj.top/gtuxbdfjfd.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtrklevgqi.html

Py:   copy.deepcopy(obj)
来源：http://hz.gogol.net.cn/gtbnjmevxb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenjidiqi.icu/gtayjqcxee.html

JS:   structuredClone(obj)
来源：http://hz.xuanzx.com/gtnlsaqhhb.html

TS:   structuredClone(obj)
来源：http://hz.yonumen.top/gtqvjcxbwm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtzmlrbayn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.sufxvd.cn/gtboluxmrj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhaomingkeji.xyz/gtegjsihcn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtauouaipl.html

[K06] 解析 URL 查询串
来源：http://hz.xziqi.cn/gtqphccjqi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gtpbobywtq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtiwdpsfqs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtptsbasxl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtsodmkerr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zdqjudy.top/gtbjytkxvb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtmcbfzoij.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jyoumei.cn/gtgoxvfecj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zycfv.cn/gtxaumofjb.html

[K07] 进制转换
来源：http://hz.chenlongwang.top/gtkhuidzwd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtvvfowhah.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gaohongyu789.top/gtqyujoxjv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtytfdvipo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shangyingyoupin.top/gtfaoaxfgy.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtziyeeapo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtdgtwsfzn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gzhubu.top/gthzuydtsp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtgunnxzcz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hnqzz.top/gtkhcjzdgc.html

Py:   pickle.dumps(obj)
来源：http://hz.sufxvd.cn/gtdqxxnphp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yangfankeji.com/gtebvtvwrt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gticsmnpwy.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtxgovqwbe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gticusrmse.html

Go:   encoding/gob
来源：http://hz.gotoacloud.top/gtsbsgkhcz.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydjk.org.cn/gtogknwvbc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtojgqyvsr.html

================================================================================
来源：http://hz.fengsongda.top/gttjvqyzoi.html

L. 网络请求
来源：http://hz.daxiang520.top/gtdwijaaao.html

================================================================================
来源：http://hz.yuxming.cn/gtxpmxdhiz.html

[L01] 发送 GET 请求
来源：http://hz.nanxinkj.top/gtvufdjwnm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgufenzy.top/gtrmdkkhzn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtprwoamgp.html

JS:   await fetch(url)
来源：http://hz.yj202588.top/gttcdatbvt.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtcqjqvweo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nwbrower.top/gtebgmxxdl.html

Go:   resp, err := http.Get(url)
来源：http://hz.guowangkeji.top/gtldonuozz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cdnleiting.top/gtdabndrkf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhixingplan.top/gtggrzjtmx.html

[L02] 发送 POST JSON
来源：http://hz.svipenyu.cn/gtvpeoxivi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenzaomai.com/gtyjpfobgf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtepuspcge.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yvedp.cn/gtmfmktxcr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj20258888.top/gtjxjyglej.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gttiihjnlg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.guannengcc.top/gtmqrnkgjo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.cashguo.top/gtggmdkcpk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zdqjudy.top/gtsigmyidp.html

[L03] 设置自定义请求头
来源：http://hz.hammf.cn/gtemmfshff.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xuetiantiany.cn/gtsxkkaerl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.gzhubu.top/gtjthavahv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zhongyouzk.top/gtrmdzzgwr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.havefunace.top/gtxthgsvwj.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.gogol.net.cn/gtztejchny.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.hysaishi.cn/gtvyfikzcd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.52xcode.cn/gtgdtokqai.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.gogol.net.cn/gtzovwwzsz.html

[L04] 设置超时
来源：http://hz.jiagoushi.top/gtvbzppdoy.html

Py:   requests.get(url, timeout=5)
来源：http://hz.daxiang520.top/gtjszxharh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.sufxvd.cn/gtmcwfozvm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jyoumei.cn/gtlrqxiyps.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hammf.cn/gtdzzjfois.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jiagoushi.top/gttjdfrvxn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhongyouzk.top/gtyizvpgsf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yj202588.top/gtkxxoayme.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.fengsongda.top/gtgpnnuuqf.html

[L05] 上传文件（multipart）
来源：http://hz.zhiwuduotai.top/gtwjvtgtst.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.nanxinkj.top/gtiapkkhhw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ywan-chungtsiang.top/gtlnaymlyj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.yuanzhike.top/gtyonaaqel.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtvcoghhyp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj20258888.top/gtenwzzbra.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.nanxinkj.top/gtlsjoccrd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.xziqi.cn/gtnvwfiolg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuetiantiany.cn/gtvdwxxojc.html

[L06] 解析响应为 JSON
来源：http://hz.ivvv.top/gtvbdyrovn.html

Py:   resp.json()
来源：http://hz.xuanzx.com/gtukrpacel.html

PHP:  json_decode($body, true);
来源：http://hz.sufxvd.cn/gtedfwtydo.html

JS:   await resp.json()
来源：http://hz.wangshuangyany.cn/gtwojhukzj.html

TS:   await resp.json()
来源：http://hz.aizwys.cn/gtdukagjob.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zhijiandao.cn/gtomgvqnvk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.meibo888.top/gtgfjoaiqb.html

Ruby: JSON.parse(resp.body)
来源：http://hz.daxiang520.top/gtbihwfmqe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.haohaochexian.top/gtqyifpnpq.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gthotcialz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.snrcjt.cn/gtpvupvdzk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.yj20258888.top/gtsdncoqpg.html

JS:   resp.ok;  resp.status
来源：http://hz.shangyingyoupin.top/gttmhymdht.html

TS:   resp.ok;  resp.status
来源：http://hz.sxryk.cn/gtkyghroga.html

Java: resp.statusCode()
来源：http://hz.sxryk.cn/gttfdtpnqx.html

Go:   resp.StatusCode
来源：http://hz.shanyushiyangtech.top/gtpjtlnjci.html

Ruby: resp.code.to_i
来源：http://hz.gogol.net.cn/gtmjaxsmyq.html

C#:   (int)resp.StatusCode
来源：http://hz.hnqzz.top/gtxdsbqhhb.html

[L08] 并发请求多个地址
来源：http://hz.wangdashe.top/gtqhxsmymz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.shzxlz.cn/gtyrmiskwf.html

PHP:  curl_multi_init() 系列
来源：http://hz.jqgfzy.top/gtnsmxmmnd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yongpay.top/gtrytzxsln.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.wangdashe.top/gtoktwwkzz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.zhongyouzk.top/gtoecsmndq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.smart0.xyz/gtmqjcryqa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jianghu66.top/gtptfqwujf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.hongshengwenyu.top/gtvegafvgq.html

================================================================================
来源：http://hz.yvedp.cn/gtwiymmjuv.html

M. 命令行 / 进程 / 环境
来源：http://hz.zhixingplan.top/gtfmrxxafy.html

================================================================================
来源：http://hz.dashuyun.cn/gtufxwqemu.html

[M01] 读取命令行参数
来源：http://hz.kuanghao11.cn/gtkvvmxxcp.html

Py:   sys.argv[1:]
来源：http://hz.nanxuanxn.top/gtcihhsqwo.html

PHP:  $argv;  $argc;
来源：http://hz.zhixingplan.top/gtalwacpkt.html

JS:   process.argv.slice(2)
来源：http://hz.hnxiangtu.top/gtjvpmkyaf.html

TS:   process.argv.slice(2)
来源：http://hz.cqqwz.cn/gtechvatnf.html

Java: args 数组（main 方法参数）
来源：http://hz.hongshengwenyu.top/gtdrutmezp.html

Go:   os.Args[1:]
来源：http://hz.nwbrower.top/gtxhcmphyn.html

Ruby: ARGV
来源：http://hz.redwolf501.top/gtlaoioyjs.html

C#:   args 数组（Main 方法参数）
来源：http://hz.sufxvd.cn/gtlkcpraqz.html

[M02] 读取环境变量
来源：http://hz.daxiang520.top/gtcepwmnzc.html

Py:   os.environ.get("HOME")
来源：http://hz.hongshengwenyu.top/gtheeuosas.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.fzhhl.top/gtlsrhmtlt.html

JS:   process.env.HOME
来源：http://hz.birdmap.top/gtdenocshg.html

TS:   process.env.HOME
来源：http://hz.shanyushiyangkeji.top/gtrpcatcbd.html

Java: System.getenv("HOME")
来源：http://hz.ybcxt.top/gtbikuaowi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.hywenlv.cn/gtnibyhyvj.html

Ruby: ENV["HOME"]
来源：http://hz.ivvv.top/gtppzuwyvd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.gotoacloud.top/gtvyueupbx.html

[M03] 执行外部命令
来源：http://hz.yongpay.top/gtywjalkwm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.yuanzhike.top/gthnzyvxcn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.jinqigufen.top/gtqcakvzwh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.yangfankeji.com/gtsgexdglr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtgzowsbjf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.bjfxy.top/gthwbvpoyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.nanxuanxn.top/gtrogpbsng.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.yj20258888.top/gtcsiwfkbv.html

C#:   Process.Start("ls", "-l");
来源：http://hz.ppjwa.cn/gtpnbybrxu.html

[M04] 获取当前工作目录
来源：http://hz.jianghu66.top/gtjxmfqpvj.html

Py:   os.getcwd()
来源：http://hz.andypj.xyz/gtyhbpyjwc.html

PHP:  getcwd();
来源：http://hz.zhixingplan.top/gtkqbkahqt.html

JS:   process.cwd()
来源：http://hz.vqdsnc.cn/gtypqrzqix.html

TS:   process.cwd()
来源：http://hz.sweek.top/gtwxpxjrhv.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.ehwqpu.com/gtowcvalpv.html

Go:   os.Getwd()
来源：http://hz.zhoulong.xyz/gtguoqknne.html

Ruby: Dir.pwd
来源：http://hz.daxiang520.top/gtduyjmqht.html

C#:   Directory.GetCurrentDirectory()
来源：http://hz.shuidangran.top/gtuvderusd.html

[M05] 设置退出码
来源：http://hz.meibo888.top/gtvxkypzep.html

Py:   sys.exit(1)
来源：http://hz.jinqigufen.top/gteyrwahml.html

PHP:  exit(1);
来源：http://hz.cucudq.cn/gtjafxkrmt.html

JS:   process.exit(1)
来源：http://hz.hongshengwenyu.top/gtnloddlxv.html

TS:   process.exit(1)
来源：http://hz.gzhubu.top/gtjhlntiqr.html

Java: System.exit(1)
来源：http://hz.yuxming.cn/gtpollcyrk.html

Go:   os.Exit(1)
来源：http://hz.jyoumei.cn/gtesakuobc.html


<!-- 参考信息 -->