代发 wailian999

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtjlsfnwth.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gtutbivxbr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gtzhimtbwx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gthazgfecp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hnqzz.top/gtidogyavq.html

TS:   /error/gim
来源：http://hz.zdqjudy.top/gtpnqylroi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gterezmkek.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gtpbzvrxkf.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtzdfabbnm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.birdmap.top/gtgfmqbmkw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtxgcamwpy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigfzy.top/gtabrcvccn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtolvkkpbe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gttepcaayq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtnuvoefxl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtekgcemmm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gtweykfjei.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtpscinfrv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtfnzdqszx.html

================================================================================
来源：http://hz.snrcjt.cn/gtlgsovxil.html

J. 日期与时间
来源：http://hz.guannengcc.top/gtonyemumn.html

================================================================================
来源：http://hz.hywenlv.cn/gtshsnurht.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtscwxnfkb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gtbyegekpt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtsuuvyvav.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtrrqufwys.html

TS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtqnbqcnfx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtxddcqpvy.html

Go:   time.Now()
来源：http://hz.haohaochexian.top/gtzqbcawxk.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtddhvwnah.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtiskakpdw.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtzuayztru.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenjidiqi.icu/gtlklwdawa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtnopbaiqw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtjdgyqcuc.html

TS:   d.toISOString()
来源：http://hz.hongshengwenyu.top/gtxqamyato.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtseciaqzw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangkeji.top/gtnqqrydxi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnxiangtu.top/gtgmpcsezv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtfzsqggdf.html

[J03] 字符串解析为日期
来源：http://hz.9152youxi.cn/gtkqqueqvw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtxxllupvu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtttlhnccf.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtkdlggoyf.html

TS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtqzveasvd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtbhjswqqw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtmzwqbspy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtiyboiqbq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangkeji.top/gteghdffgz.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtgxbusdkt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yongpay.top/gtcyzmobqe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jyoumei.cn/gtrwzidlei.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtdfsovxwy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtqgifwxpv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtvtgytzms.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtzzppceqw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtofjbsciz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhijiandao.cn/gthiszdyiy.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhaomingkeji.xyz/gtyfkmuwnt.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtyarrtegh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtlsfwzhdh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtkmyamupl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtxakftwsi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gzhubu.top/gttyydwrdo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj20258888.top/gtwccutycl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtprhlggty.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtjxousaeq.html

[J06] 计算两时间之差
来源：http://hz.cheryme.top/gtrqliowlx.html

Py:   (end - start).total_seconds()
来源：http://hz.jqgufenzy.top/gtmwhmaxfn.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtvszujfwc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangkeji.top/gttplpgmre.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gtseiwskvc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jyoumei.cn/gtswwluakw.html

Go:   end.Sub(start).Hours()
来源：http://hz.bjfxy.top/gtvwwfpphl.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtsnxefmkw.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtuyzsxbox.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gtpezemnhh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtzvfejiow.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtjdcawiao.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtnovybxdj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtjkwfdyfd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xylfe.cn/gtzcxmrgnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtodiwsdxw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtuaizokpe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtxlqwmbqf.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtpzezcely.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtkuztzloy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtehejlrfr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtjshsamdi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtrxgabzti.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.bjfxy.top/gtgvcnnrsd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258888.top/gttazqukgs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtwusfhiny.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtzrvjzndg.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtxfulrnjl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gtlumuhylr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtkjkfmetf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtkiwxxnlb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtviqzsvtq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ybcxt.top/gtdfpgksnb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtubpxtzgg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtdqvwfmuc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yvedp.cn/gtqjpftkki.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtsswzazdt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xylfe.cn/gthqinoprq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtxpcsbwew.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangkeji.top/gtrwbgkmwp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guowangkeji.top/gtrtkqaxhf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenzaomai.com/gtoagvdgvb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gtcvgyzvqj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ehwqpu.com/gtlvdaasea.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtkuglgmpm.html

================================================================================
来源：http://hz.yonumen.top/gtahujcxsc.html

K. JSON 与序列化
来源：http://hz.nanxuanxn.top/gtfxfmbpef.html

================================================================================
来源：http://hz.jinqigfzy.top/gtytmfmedk.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtcezoiyvy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtuaqqyupe.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtecyjglts.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258888.top/gtqdvupuma.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtfwltlyga.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtsqxkbpyj.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtoipftfpc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtgurjzqqf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhaomingkeji.xyz/gtjtwwxetk.html

[K02] JSON 字符串转对象
来源：http://hz.316326.xyz/gttlgsphfc.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtnwidvysl.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtisqoawwl.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtsgmgftdd.html

TS:   JSON.parse(s)
来源：http://hz.guowangkeji.top/gtsoqvpavf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daxiang520.top/gtyhwmycet.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtaokyuzax.html

Ruby: JSON.parse(s)
来源：http://hz.xuanzx.com/gtntjlipjz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jianghu66.top/gtoyifskmu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtttqjqqts.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtanraallx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtcklpthgn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gotoacloud.top/gtmyguavsy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtrcsexqcw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shuidangran.top/gtfsuhipcb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zdqjudy.top/gtgqmgfsmf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuanzx.com/gtljgguauc.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gaohongyu789.top/gtwyxcgcan.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtdloxufdw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.mhx1999.top/gtrhynmdhe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtmdnpcxoz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cashguo.top/gtrqoewaiv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.guannengcc.top/gtomlvmecw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ehwqpu.com/gtlgvlittu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinyuanbaomall.cn/gtirdpqhkh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtkuobyddj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gttghhzqof.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtmggmhthf.html

Py:   copy.deepcopy(obj)
来源：http://hz.c1oappe.top/gtcbkhyahs.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yonumen.top/gthfwtzqcu.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtfwlunpsk.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtirdemady.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtuctnuhsy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.kuanghao11.cn/gtydwkztmf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zdqjudy.top/gtulmwykxb.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtzbxwpgfm.html

[K06] 解析 URL 查询串
来源：http://hz.zhijiandao.cn/gtqnyehiij.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtdjmaolhc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtslzpemlr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtihvtzakz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtpwxkmikx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhijiandao.cn/gthnvoystq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.iojbl.cn/gtcogvvpbb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtlxnixzpy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtafeuhros.html

[K07] 进制转换
来源：http://hz.dianchejie.cn/gtgrapgjlj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hongshengwenyu.top/gtfihpwjlt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtvjfsrduc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtqfvgcsbp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.316326.xyz/gttgnhvwci.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtakrfvsoy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtynxoharr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtkcmexmtd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gtkrxhcflb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtyznjqwqk.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtalnkbhth.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.redwolf501.top/gtufvablgk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtexewsuvl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.0kj1m.cn/gtwmzelupb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtrbkbebob.html

Go:   encoding/gob
来源：http://hz.vqdsnc.cn/gtivxfzlsw.html

Ruby: Marshal.dump(obj)
来源：http://hz.chenjidiqi.icu/gtnsoznqsy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtbxhpownn.html

================================================================================
来源：http://hz.mhx1999.top/gtyhgeodbd.html

L. 网络请求
来源：http://hz.sysykeji.top/gtxwokvboq.html

================================================================================
来源：http://hz.iojbl.cn/gtggrwainn.html

[L01] 发送 GET 请求
来源：http://hz.tianlin.xyz/gtalluiaqz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.ydjk.org.cn/gtmdipmogg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.sxryk.cn/gtucquvibj.html

JS:   await fetch(url)
来源：http://hz.mhx1999.top/gtnpbclrbx.html

TS:   await fetch(url)
来源：http://hz.gotoacloud.top/gtbobpbkex.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtvsmcnimn.html

Go:   resp, err := http.Get(url)
来源：http://hz.zycfv.cn/gtlcxagsrp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.mhx1999.top/gtofcurdvq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gttcvljhvt.html

[L02] 发送 POST JSON
来源：http://hz.havefunace.top/gtyrlbkxga.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.dashuyun.cn/gturtyoywh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.52xcode.cn/gtvhkqngml.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtwjodtxye.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fzhhl.top/gtbwqazxqt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.cashguo.top/gtgbaqobwc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtalthnjsy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.nwbrower.top/gtxgtullrx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.zhengqikj.top/gtptikeibe.html

[L03] 设置自定义请求头
来源：http://hz.daxiang520.top/gtaknhmjvw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxuanxn.top/gtksvcabvz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.tianlin.xyz/gtgnbpjoef.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.meibo888.top/gtlivwupso.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.feifeiyinyue.top/gtytfjdydn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.ybcxt.top/gtocegnasv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.0kj1m.cn/gtswhtdzqp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj20258.top/gtbvwclwyx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xziqi.cn/gtxszuhlug.html

[L04] 设置超时
来源：http://hz.zhaomingkeji.xyz/gtufdlsaej.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenlongwang.top/gtakejheta.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhiwuduotai.top/gtftvgafjh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.jinghuilouyu.cn/gtkmwzzupu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hywenlv.cn/gtmcyarbux.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.sysykeji.top/gtrvjjbyew.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.haohaochexian.top/gtjjpyibhe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtcpqmyoaz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.sysykeji.top/gtuitcdoir.html

[L05] 上传文件（multipart）
来源：http://hz.yangfankeji.com/gtkabdczta.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnxiangtu.top/gtyikezlav.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.daxiang520.top/gtjjmonqec.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.pengpengdd.cyou/gtttjorxfq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.ppjwa.cn/gtumoteruy.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.nanxinkj.top/gtogbbwxzw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.dianchejie.cn/gtjyubixhd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.dianchejie.cn/gtxysosusx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.daxiang520.top/gtcycctjes.html

[L06] 解析响应为 JSON
来源：http://hz.nanxuanxn.top/gtpnhnvaak.html

Py:   resp.json()
来源：http://hz.zdqjudy.top/gtdelkwcyp.html

PHP:  json_decode($body, true);
来源：http://hz.meibo888.top/gtevksuhqh.html

JS:   await resp.json()
来源：http://hz.nwbrower.top/gtjflrkiul.html

TS:   await resp.json()
来源：http://hz.cucudq.cn/gtmbjmimac.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.dashuyun.cn/gtknknnyqz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.tianlin.xyz/gterpxotfw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.shanyushiyangtech.top/gtxjbjytlr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhixingplan.top/gtyymfprwx.html

[L07] 处理 HTTP 状态码
来源：http://hz.smart0.xyz/gtjbslnpaa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.xuanzx.com/gtuuiqlyjo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhixingplan.top/gtahszxyrb.html

JS:   resp.ok;  resp.status
来源：http://hz.xziqi.cn/gtyiwzeylo.html

TS:   resp.ok;  resp.status
来源：http://hz.zhiwuduotai.top/gtykpbgneg.html

Java: resp.statusCode()
来源：http://hz.52xcode.cn/gtscaagmxb.html

Go:   resp.StatusCode
来源：http://hz.yonumen.top/gtpcleltxh.html

Ruby: resp.code.to_i
来源：http://hz.vqdsnc.cn/gtgtndstxj.html

C#:   (int)resp.StatusCode
来源：http://hz.bjfxy.top/gteuntdorw.html

[L08] 并发请求多个地址
来源：http://hz.hongshengwenyu.top/gtmzxxofqx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.zycfv.cn/gtmqvvswel.html

PHP:  curl_multi_init() 系列
来源：http://hz.redwolf501.top/gtpnmsxvdo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jinyuanbaomall.cn/gtgawxfxzq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.haohaochexian.top/gtjzopdzqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.svipenyu.cn/gtuvdqsbol.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.birdmap.top/gtxwpmvbpv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zhoulong.xyz/gtnvmcjbha.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.zhaomingkeji.xyz/gthiylgiwm.html

================================================================================
来源：http://hz.svipenyu.cn/gtlapfnkqa.html

M. 命令行 / 进程 / 环境
来源：http://hz.havefunace.top/gtrjikesoc.html

================================================================================
来源：http://hz.jianghu66.top/gtlgrzaesy.html

[M01] 读取命令行参数
来源：http://hz.gzhubu.top/gthcpgjejm.html

Py:   sys.argv[1:]
来源：http://hz.xziqi.cn/gtwppdgrfe.html

PHP:  $argv;  $argc;
来源：http://hz.cheryme.top/gtecawfilt.html

JS:   process.argv.slice(2)
来源：http://hz.meibo888.top/gtqvyelemv.html

TS:   process.argv.slice(2)
来源：http://hz.zhijiandao.cn/gtajcbgbqc.html

Java: args 数组（main 方法参数）
来源：http://hz.yj20258.top/gtcjbyhrdo.html

Go:   os.Args[1:]
来源：http://hz.sysykeji.top/gtkhnseort.html

Ruby: ARGV
来源：http://hz.hysaishi.cn/gtillchcfx.html

C#:   args 数组（Main 方法参数）
来源：http://hz.ppjwa.cn/gtsqifbknr.html

[M02] 读取环境变量
来源：http://hz.nanxinkj.top/gtdtxkhbsw.html

Py:   os.environ.get("HOME")
来源：http://hz.fengsongda.top/gtvqottnif.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ppjwa.cn/gtbvtvwebm.html

JS:   process.env.HOME
来源：http://hz.chenlongwang.top/gtczixynak.html

TS:   process.env.HOME
来源：http://hz.jinqigfzy.top/gtggiidsgq.html

Java: System.getenv("HOME")
来源：http://hz.mhx1999.top/gtmslsgbts.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.jqgufenzy.top/gtwbqoopsx.html

Ruby: ENV["HOME"]
来源：http://hz.jinqigufen.top/gtvghydaex.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.chenlongwang.top/gthmthqxmw.html

[M03] 执行外部命令
来源：http://hz.hysaishi.cn/gttlppjdlb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.dianchejie.cn/gtwnvvlvbo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.chenlongwang.top/gtuacixbgv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.jqgfzy.top/gtwzihaqcm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.yvedp.cn/gtdxkxoawl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hz.haohaochexian.top/gtmaiqeclz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://hz.ivvv.top/gtlgitxsxc.html

Ruby: system("ls -l");  `ls -l`
来源：http://hz.wangshuangyany.cn/gtxwoqmtir.html

C#:   Process.Start("ls", "-l");
来源：http://hz.tianlin.xyz/gtrpfsktlg.html

[M04] 获取当前工作目录
来源：http://hz.yj202588.top/gttdzxkecb.html

Py:   os.getcwd()
来源：http://hz.svipenyu.cn/gtstmnwwzq.html

PHP:  getcwd();
来源：http://hz.birdmap.top/gtkazcpbtf.html

JS:   process.cwd()
来源：http://hz.guannengcc.top/gtpkngxifm.html

TS:   process.cwd()
来源：http://hz.nanxinkj.top/gtzqxwavhp.html

Java: Path.of("").toAbsolutePath()
来源：http://hz.xingfuxueyuan.xyz/gtinpzjhrh.html

Go:   os.Getwd()
来源：http://hz.feifeiyinyue.top/gtxszbjuan.html

Ruby: Dir.pwd
来源：http://hz.xziqi.cn/gtnzhhpkyx.html


<!-- 参考信息 -->