代发 wailian999

Java: s.split("\\s*,\\s*")
来源：http://hz.yanxiufei.cn/gthzzidlqy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gtrnzuqpsg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtthivdykd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtaynznxoa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtwmnhirrl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtjqmupvht.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtfrfpefue.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.redwolf501.top/gtgjpjbgfd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtmshkneqt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtnmrcskug.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gttxmgybzu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtalletbel.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuanzx.com/gtdnlplfdn.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtepmfymnn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtebyjfoxt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gzhubu.top/gtjbgltgex.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtsoyqqwop.html

TS:   /error/gim
来源：http://hz.zhijiandao.cn/gtsuqdejxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinghuilouyu.cn/gtmasrcppb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtmfuwepuo.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtsdyfdhhd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jyoumei.cn/gtdcrrtbji.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtqyigvgen.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtfghposvi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guowangkeji.top/gtafitfhno.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtkozmlgsj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtwnwmsihe.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtfizchcud.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gteikabbhp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtgrxhypfi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtbevrpmcj.html

================================================================================
来源：http://hz.haohaochexian.top/gtznrpuezo.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtftikilzn.html

================================================================================
来源：http://hz.cucudq.cn/gtmfafogej.html

[J01] 获取当前时间
来源：http://hz.hnqzz.top/gtwlfuukpd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtdybcpilf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtiokasxgh.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtwlrdmirf.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtlvcopbkj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.svipenyu.cn/gtnyzknopr.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gtvhnuwgle.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gtbcvqsnuh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhijiandao.cn/gtlnqypqsr.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtoivojtvv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gttireiwzj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtoarorkqe.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.0kj1m.cn/gtbifcfmwn.html

TS:   d.toISOString()
来源：http://hz.zhiwuduotai.top/gtixwlwyxh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtsjugyark.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtoaxmdwsz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtgshgknyi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj20258888.top/gtxgskowqh.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gtaplhhnkv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtztfbaqpp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtuvhizxqz.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtmmahmwro.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtjslmlavs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtavdufhlj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shangyingyoupin.top/gttlpdkwof.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtgtyedgye.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.dashuyun.cn/gthoxxlrxj.html

[J04] 时间戳与日期互转
来源：http://hz.xingfuxueyuan.xyz/gtxhtytppo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtxgjtrtwx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtnahhklko.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtyajmtuhp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtbzaoujfs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtlkldhwrv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gttdftfiwa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtbxvfjygr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtntavrjxs.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtnnlfceta.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtjowtmwwz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj202588.top/gtyrychfno.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtyxwaayep.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtdcybglqj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtqnroxjjk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtsehtuzvx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zdqjudy.top/gtnifaspac.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtavposuuu.html

[J06] 计算两时间之差
来源：http://hz.sufxvd.cn/gthsjwgxug.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxuanxn.top/gteshkghil.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtlmhojcfw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gttxxtwrtq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shuidangran.top/gtkjalpbzy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtshltmdbm.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtcxgtfkpe.html

Ruby: end - start                 # 返回秒数
来源：http://hz.snrcjt.cn/gtxqzijumo.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhoulong.xyz/gtcdlgspnd.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtlsgevvln.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gthdkewyyj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.snrcjt.cn/gtlmikgdfp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtbdwwjqid.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtembvkknp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cucudq.cn/gtwjdtqztc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtdauwbshq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtxqaktcnf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gthkhbjftv.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtslrmdrxq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guannengcc.top/gtzkvruxyt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.aizwys.cn/gtntuhfbzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtffiekimy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shangyingyoupin.top/gtmedwhcgd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtrkyhcnfz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtruutukcl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtubezoqyn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtrgpicrwn.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtbcetvpfe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.birdmap.top/gttlmbijyg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtxotwjclo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtmdrlxgit.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtbklfedel.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtyskryjkq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtcspsxwdm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtvefzgzoo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtfyopnkxi.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gteojoyffx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtnteknkyt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtabjwckvh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sufxvd.cn/gtoanjgomy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtnlpdvgxy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.kuanghao11.cn/gtlyxtuznt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.dianchejie.cn/gtktonysgr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtbttrtylm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nwbrower.top/gtoapqgdpx.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkgbwgwqq.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gttvriqbal.html

================================================================================
来源：http://hz.chenlongwang.top/gtrumvmsyo.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtgbrbworz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtuuzwqopz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtsbrotrmr.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtbkoyhnfx.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtnqqyvlut.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.havefunace.top/gtrqatlyih.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gtnegqchbo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuxming.cn/gtizaugnyg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gotoacloud.top/gtfluodqbh.html

[K02] JSON 字符串转对象
来源：http://hz.yongpay.top/gtlsbivhgv.html

Py:   json.loads(s)
来源：http://hz.daxiang520.top/gtlgrfocyz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangtech.top/gtwglqqxmi.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtksjnyvrc.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtpylhqjwz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtxtfxstjo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtcukpakse.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtipdoedao.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtenhkusrg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtqpcavzjo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtohvtkddc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtcjfujrbb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinghuilouyu.cn/gtivnqmtgd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhongyouzk.top/gtyghhrxsr.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gtbrzsbpcv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.bjfxy.top/gtsrsbccgf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.52xcode.cn/gtsxxuzaog.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtiswfwsbc.html

[K04] 读取 JSON 文件
来源：http://hz.zhaomingkeji.xyz/gtpheyekgo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtshcztvku.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtylyxlnuu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtxncfhqxk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gthzwgwtmz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tianlin.xyz/gtjimvflfa.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtpjzpvytg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtohtdprtl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hongshengwenyu.top/gtmmsdfeuj.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtmqxemcac.html

Py:   copy.deepcopy(obj)
来源：http://hz.sweek.top/gtyaijogqz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtuwjtujno.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtkihsjwjk.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gthhhqghhq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtiigbcsae.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gthqmdlest.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtgpilolqo.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.kuanghao11.cn/gtfiklepvz.html

[K06] 解析 URL 查询串
来源：http://hz.iojbl.cn/gtemtaaycn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gotoacloud.top/gtbsxmayxl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gaohongyu789.top/gtavwplyzg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nwbrower.top/gtibjyvnmg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtgomjgzdl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenlongwang.top/gttnrjiczw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jyoumei.cn/gtleoqjzdh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xuanzx.com/gthpvtqbui.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtxfapzugm.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtvwlzrrrw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhongyouzk.top/gtikrihvsy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cheryme.top/gtklphyfkk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtohiveazv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jianghu66.top/gtpmetcjik.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtowckgink.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtptukrtiy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtyfhnrlgy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj202588.top/gtqivbkbeo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigufen.top/gtukbfntci.html

Py:   pickle.dumps(obj)
来源：http://hz.ehwqpu.com/gtnrnothxu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtfedmvbuh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.svipenyu.cn/gtekqpntbw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtijphylim.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj20258.top/gtulywirda.html

Go:   encoding/gob
来源：http://hz.cucudq.cn/gtbxnwimms.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhijiandao.cn/gtphiytsxh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtsnwldglz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtsamuouqj.html

L. 网络请求
来源：http://hz.sweek.top/gtoyofzebx.html

================================================================================
来源：http://hz.c1oappe.top/gtfplrxfjb.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtmqbueapy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.guowangkeji.top/gtpploqgvj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yj20258888.top/gtorxfpazu.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtgicbstif.html

TS:   await fetch(url)
来源：http://hz.andypj.xyz/gtmohqoyyh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.0kj1m.cn/gtqsmhcyec.html

Go:   resp, err := http.Get(url)
来源：http://hz.hnxiangtu.top/gtdohbbqpq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.c1oappe.top/gtpnrbysku.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.kuanghao11.cn/gtvbcovurd.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtudlnaghu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ybcxt.top/gtphsiuvjt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.ydzc1.top/gtdquzejvn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtkrjhvumm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.fengsongda.top/gtekqviwwj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ybcxt.top/gtyjybqgeg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.chenzaomai.com/gtctvvxfvp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtcqgeqtil.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yuxming.cn/gtmfjxukfn.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtocemjgdd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.xinyue.icu/gtfvljnfou.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.cqqwz.cn/gtjjrvwekp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ppjwa.cn/gtthizclic.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sysykeji.top/gtrvmfimiw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yanxiufei.cn/gtgjbgjusb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.sysykeji.top/gtmzbiivpc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.daria6918.cn/gtzlsdzpof.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.jinqigfzy.top/gtuorxhosz.html

[L04] 设置超时
来源：http://hz.ppjwa.cn/gtqggjgpxa.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenjidiqi.icu/gttqyvbaur.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.aizwys.cn/gtpbrjqgpn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.52xcode.cn/gtundarirh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gthizdkahg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.chenjidiqi.icu/gtwlfoaspn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.redwolf501.top/gtbubfmcmr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tianlin.xyz/gtcbxsshsd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.tanke756.top/gtoslsxgcz.html

[L05] 上传文件（multipart）
来源：http://hz.nwbrower.top/gtswegjdjc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.shzxlz.cn/gtwevgbrqq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zhaomingkeji.xyz/gtfhdwafdz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gttfwzxlvb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.wangdashe.top/gtzbdsbqlh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinqigfzy.top/gtfkrasqyv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.feifeiyinyue.top/gttlroyxtr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.yangfankeji.com/gtyndcavxa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fzhhl.top/gtdfbatmam.html

[L06] 解析响应为 JSON
来源：http://hz.andypj.xyz/gtxrfkopjv.html

Py:   resp.json()
来源：http://hz.jlsjyb.cn/gtxizzddct.html

PHP:  json_decode($body, true);
来源：http://hz.sysykeji.top/gtxwhxzcto.html

JS:   await resp.json()
来源：http://hz.fengsongda.top/gtimvjtxgf.html

TS:   await resp.json()
来源：http://hz.tianlin.xyz/gtenypxhuj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.yongpay.top/gtrqyhwenw.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.9152youxi.cn/gtjvkmiikw.html

Ruby: JSON.parse(resp.body)
来源：http://hz.52xcode.cn/gtxaihttxn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.jinghuilouyu.cn/gttiirsdnc.html

[L07] 处理 HTTP 状态码
来源：http://hz.yj20258.top/gtrwlkjfth.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hfpthk.cn/gtltsaendi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.jqgufenzy.top/gtfbrreapv.html

JS:   resp.ok;  resp.status
来源：http://hz.yj202588.top/gtsnikcpff.html

TS:   resp.ok;  resp.status
来源：http://hz.quarkkingdee.top/gtdlawfvku.html

Java: resp.statusCode()
来源：http://hz.guowangkeji.top/gtcvdqiisr.html

Go:   resp.StatusCode
来源：http://hz.zdqjudy.top/gtkckyphvp.html

Ruby: resp.code.to_i
来源：http://hz.hongshengwenyu.top/gtlbkucstf.html

C#:   (int)resp.StatusCode
来源：http://hz.chenzaomai.com/gttrimsxud.html

[L08] 并发请求多个地址
来源：http://hz.cashguo.top/gtmubegkxq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.wangdashe.top/gtkwzkofdi.html

PHP:  curl_multi_init() 系列
来源：http://hz.xziqi.cn/gtryflytcm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.birdmap.top/gtpwcfkcwg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.ydzc1.top/gtpatwfqxz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.xziqi.cn/gtwqaywcww.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.aibaodan.cn/gtzentstea.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.jinyuanbaomall.cn/gtzmljgztk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shangyingyoupin.top/gtbggozjad.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpsykwnna.html

M. 命令行 / 进程 / 环境
来源：http://hz.316326.xyz/gtulgrpfhn.html

================================================================================
来源：http://hz.meibo888.top/gtbwsrijos.html

[M01] 读取命令行参数
来源：http://hz.xinyue.icu/gtsqjwcywg.html

Py:   sys.argv[1:]
来源：http://hz.gotoacloud.top/gtcsphwvoj.html

PHP:  $argv;  $argc;
来源：http://hz.zycfv.cn/gtuzfevzci.html

JS:   process.argv.slice(2)
来源：http://hz.ybcxt.top/gtxhmdjhop.html

TS:   process.argv.slice(2)
来源：http://hz.cashguo.top/gtrhiwwled.html

Java: args 数组（main 方法参数）
来源：http://hz.hammf.cn/gthkykbbeb.html

Go:   os.Args[1:]
来源：http://hz.jqgufenzy.top/gtnlgpcdxj.html

Ruby: ARGV
来源：http://hz.quarkkingdee.top/gtawzmbvzc.html

C#:   args 数组（Main 方法参数）
来源：http://hz.0kj1m.cn/gtwsluwwsl.html

[M02] 读取环境变量
来源：http://hz.tian-w.cn/gtpqururuc.html

Py:   os.environ.get("HOME")
来源：http://hz.tanke756.top/gtajqgtyez.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://hz.ivvv.top/gtouaqsymd.html

JS:   process.env.HOME
来源：http://hz.snrcjt.cn/gtumclryah.html

TS:   process.env.HOME
来源：http://hz.fengsongda.top/gtzdvtebql.html

Java: System.getenv("HOME")
来源：http://hz.gaohongyu789.top/gtmxbxsfdp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hz.yj20258.top/gtzdaczgzv.html

Ruby: ENV["HOME"]
来源：http://hz.0kj1m.cn/gtekpefbpv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hz.jinqigfzy.top/gtzjjgpwud.html

[M03] 执行外部命令
来源：http://hz.smart0.xyz/gtafanttde.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hz.aizwys.cn/gtsnjgokfn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://hz.hammf.cn/gtehnhfjag.html

JS:   child_process.execSync("ls -l").toString()
来源：http://hz.cashguo.top/gtatarbtfs.html

TS:   child_process.execSync("ls -l").toString()
来源：http://hz.gzhubu.top/gtxfwubmli.html


<!-- 参考信息 -->