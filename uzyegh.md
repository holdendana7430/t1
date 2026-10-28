代发 wailian999

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtukibutqu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shuidangran.top/gtztdcmmyh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtyhukcnek.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jyoumei.cn/gtqsooqsxh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ppjwa.cn/gtpxtuhlkr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtvlekknnt.html

[I04] 正则替换
来源：http://hz.chenjidiqi.icu/gttnwxwxuy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gtxvvbgknu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xinyue.icu/gttlkkimhj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtqvfylogd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtuwvditnt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gttpbfbyyz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtvolgrbsx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenjidiqi.icu/gtdgtcoshv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gthteoonyo.html

[I05] 按正则拆分
来源：http://hz.iojbl.cn/gtbyomnipz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtzyiqsnvm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jianghu66.top/gtkromhcds.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtfyxhuwty.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtlhzbjhbk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gtufnbkimx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gogol.net.cn/gtinssaaxa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtqzuabncm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cashguo.top/gtilulilzt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtgwnncuju.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtlpnymkyc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtkzsibeta.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtqvguqvwx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtgxqtssam.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.9152youxi.cn/gtkpafqhdz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtyljcqijt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtkkfaitra.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtnuesfyae.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtjhzpruje.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtnxpybbsy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtdyvcfvwv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xinyue.icu/gtmgscoiir.html

TS:   /error/gim
来源：http://hz.shanyushiyangkeji.top/gtgnrwkvlp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtnpaflolb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtzhtulmsw.html

Ruby: s.scan(/error/i)
来源：http://hz.tian-w.cn/gtdysqylub.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtaafpmpgl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtrzccycks.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtjtcxhawl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtklcohxrh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnqzz.top/gtsyqwkixh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtbquvbrgr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtodsdnzra.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hywenlv.cn/gtcauzcmpc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuanzhike.top/gtrtdmhrmw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gtondazdpg.html

================================================================================
来源：http://hz.yvedp.cn/gtokfixazw.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtyxvgweyx.html

================================================================================
来源：http://hz.yueranfly.top/gtyjimwlfe.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtgsmdpxle.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtxdcprxnw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtbwgtqsqt.html

JS:   new Date();  Date.now()
来源：http://hz.zhaomingkeji.xyz/gtyxhtmpbw.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtawpucemb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangtech.top/gtwuyiydfa.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtiscwygkz.html

Ruby: Time.now
来源：http://hz.zhengqikj.top/gtxffcbtng.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtcrfepxtb.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtxuhibapn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtkktdpvcp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtsgjqngsd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gthnlnpgxa.html

TS:   d.toISOString()
来源：http://hz.zhijiandao.cn/gtfqberaro.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gthfcjxiua.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gtkglsqcgv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtmolfksyl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtkfmpjtci.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtbxzjttqw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gtabpapfmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shangyingyoupin.top/gtblmzgebn.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtenxzqiak.html

TS:   new Date("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtueyecxdz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ydjk.org.cn/gtkmejjrzv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtkbvtfprl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtwfvnfuwj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.havefunace.top/gtdhnblhqw.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtuetxfypg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtxwsmkxio.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.0kj1m.cn/gtoulspuby.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fengsongda.top/gtfmhrvxrp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuxming.cn/gtvquhaykg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sufxvd.cn/gthvbllxzx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuetiantiany.cn/gtiuvspbdg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.c1oappe.top/gtmjytyosy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gtxgsmtkfe.html

[J05] 时间加减（加 7 天）
来源：http://hz.tian-w.cn/gtwhgjcwbg.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtemqacnzl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gtykchkuro.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtvpcymsat.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gthbofwoqs.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtpzevtutu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gttsbunerq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtjdggbynf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gtbvlgvfsl.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtybnqkmyz.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtvcobeoog.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtxbwyuxcl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtmiffcsnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtnjfvfdde.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sufxvd.cn/gtfdwovoex.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtctawhyug.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtsroxaprh.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtwlulknzs.html

[J07] 比较两个日期
来源：http://hz.sysykeji.top/gtqealiivm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtzzgdfxpq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dianchejie.cn/gtoofqwjzd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtqncjdjwa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtvsojfxlt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.birdmap.top/gtqgcaaprk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtldmzrlpv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtmtwfzzdn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtqggiyeur.html

[J08] 提取年月日与星期
来源：http://hz.dashuyun.cn/gtgypsqrlf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtwfuvzrkz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtcnmgnffu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sweek.top/gtynxuhkct.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtakdmfdlu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtxfgyxbkr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtwocsdoca.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtybjbbgxx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hongshengwenyu.top/gteplaeluj.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtiudupyax.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hysaishi.cn/gtknbhzgul.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtsemjmwwj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtnrvmxqez.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtrldmhrbu.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtkltvbqqj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dianchejie.cn/gtfksezmot.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtfkbakvap.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gtangerpry.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtmniculcy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hysaishi.cn/gtqqkflytw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtskteoart.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gttqzgsoyu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yongpay.top/gtazulxlwa.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gtprmkcllt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtvffwguzj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtdocebdio.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yangfankeji.com/gtwgidkijm.html

================================================================================
来源：http://hz.tianlin.xyz/gtulgshyek.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtzqclyjvh.html

================================================================================
来源：http://hz.c1oappe.top/gtcxcqxheq.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtzzligzbr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtufwlkyyd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtdrayajtj.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtffdyxehm.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtziehmfkc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ivvv.top/gtaserevwc.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gtbptmimcl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gogol.net.cn/gtydzqxiwu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangtech.top/gtakclffmm.html

[K02] JSON 字符串转对象
来源：http://hz.9152youxi.cn/gthiercpdp.html

Py:   json.loads(s)
来源：http://hz.jiagoushi.top/gtmgafwpky.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtgedjwznj.html

JS:   JSON.parse(s)
来源：http://hz.xuanzx.com/gtzmdcucts.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gthaotphqu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtqulopojz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtrxmoldxs.html

Ruby: JSON.parse(s)
来源：http://hz.chenlongwang.top/gtmswlpvek.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.vqdsnc.cn/gtlbzhzrmk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtxyknyanj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtghlmcmry.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtsvffjgbb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtgrlqzbkd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtnudnzktp.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xuetiantiany.cn/gtpemavqvr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtmoefjhhw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shanyushiyangtech.top/gtiewureln.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daria6918.cn/gthffaubtx.html

[K04] 读取 JSON 文件
来源：http://hz.zhongyouzk.top/gtniazzbhx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtnzcituee.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hammf.cn/gtvozdavcg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.316326.xyz/gtopgzscyh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtwvubbndu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shanyushiyangtech.top/gtadyhqzid.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.kuanghao11.cn/gtnwymtfyp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtmebysrfg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtwmsxxotk.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtynmeeblm.html

Py:   copy.deepcopy(obj)
来源：http://hz.quarkkingdee.top/gtsafleugb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhongyouzk.top/gtduzjqsrz.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtzlkrpwjj.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtegpmyuwt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hammf.cn/gtjpjvbqnj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtkpnotbpk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dashuyun.cn/gtbzrgctnn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtalcftjok.html

[K06] 解析 URL 查询串
来源：http://hz.cdnleiting.top/gttlqrclgq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuetiantiany.cn/gtyjiuueak.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtoyiijfie.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.meibo888.top/gtrxlahdee.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daxiang520.top/gttkjcmqzz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtxjmgjpkk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.0kj1m.cn/gtcvgqmehl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtvuydukef.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.guowangkeji.top/gtwnivgwov.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtbfdianmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtcqahpwjz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sweek.top/gtopvaymsa.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtqxoffvon.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtaogwqztm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtichnfnxd.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtnybgtbeu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yvedp.cn/gtwgbevlth.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yj20258.top/gtzsotpcto.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yangfankeji.com/gtogihdapp.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtjbtokfqu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gtphcimlfm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtrhsyqyqz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj202588.top/gtoctqgxny.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.birdmap.top/gtzyefwbzv.html

Go:   encoding/gob
来源：http://hz.daxiang520.top/gtbhidezpu.html

Ruby: Marshal.dump(obj)
来源：http://hz.yueranfly.top/gthwdgzmes.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtcunodfkt.html

================================================================================
来源：http://hz.aizwys.cn/gtokvzhmjx.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtxmqjrwfc.html

================================================================================
来源：http://hz.tian-w.cn/gthtrqegni.html

[L01] 发送 GET 请求
来源：http://hz.chenlongwang.top/gtoamhcbcx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hongshengwenyu.top/gtdepfklij.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhixingplan.top/gtqwsobyqq.html

JS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtmvpvjxgh.html

TS:   await fetch(url)
来源：http://hz.dashuyun.cn/gtsorjceox.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shzxlz.cn/gtzcgaomdz.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtjtqxfjdf.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.gzhubu.top/gtfdfnpmzx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.sysykeji.top/gtdvnnvtmo.html

[L02] 发送 POST JSON
来源：http://hz.zhoulong.xyz/gtgqwvglky.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.chenlongwang.top/gtlwwfqjfr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sysykeji.top/gtjduvfkhk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinyuanbaomall.cn/gtcjwbekdi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.sysykeji.top/gtepxoaejw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.ydjk.org.cn/gtmofhagoz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.cdnleiting.top/gtezcqzgkd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jqgfzy.top/gtxnwtnvpd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daria6918.cn/gttjcodnlg.html

[L03] 设置自定义请求头
来源：http://hz.jinyuanbaomall.cn/gtteiopocs.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.chenjidiqi.icu/gtzlgsfhhy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sxryk.cn/gtzkpqswwr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.xylfe.cn/gtmxnqpxun.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yongpay.top/gtxmwbclhp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.bjfxy.top/gtkvypdkgt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.guowangkeji.top/gtnvesmpbf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yangfankeji.com/gtnvldeuhb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.andypj.xyz/gtccadojaz.html

[L04] 设置超时
来源：http://hz.yvedp.cn/gtnfedndae.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xingfuxueyuan.xyz/gtaxpemlon.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yvedp.cn/gtmgazsyrf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yvedp.cn/gtlanuxbxu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.feifeiyinyue.top/gtltvwzqvo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.ydjk.org.cn/gtgqhcdnqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj20258.top/gtmrwszjca.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.tian-w.cn/gtyasmlepb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.havefunace.top/gtnkhsdgof.html

[L05] 上传文件（multipart）
来源：http://hz.xuetiantiany.cn/gtigesomjy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.iojbl.cn/gtwntgssul.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.zdqjudy.top/gtghumenvv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.c1oappe.top/gtsmqdrqdu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.guannengcc.top/gtqehdjajx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.zhijiandao.cn/gtstztnurd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.havefunace.top/gthajemuck.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinqigufen.top/gtylfmrvsp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.hnqzz.top/gtzblpwmvo.html

[L06] 解析响应为 JSON
来源：http://hz.zhoulong.xyz/gtwqbadrkn.html

Py:   resp.json()
来源：http://hz.jianghu66.top/gtfpehxjmd.html

PHP:  json_decode($body, true);
来源：http://hz.hywenlv.cn/gtqfewjoqc.html

JS:   await resp.json()
来源：http://hz.jlsjyb.cn/gtdkoxvduh.html

TS:   await resp.json()
来源：http://hz.gzhubu.top/gtbohvjcqg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.svipenyu.cn/gtbgjvdkej.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.aibaodan.cn/gtsuetdylc.html

Ruby: JSON.parse(resp.body)
来源：http://hz.yuxming.cn/gtrpmzufvh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zdqjudy.top/gtvnylrifo.html

[L07] 处理 HTTP 状态码
来源：http://hz.cashguo.top/gttssikbft.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.wangshuangyany.cn/gtzurjsdig.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.nwbrower.top/gtcuobsuwf.html

JS:   resp.ok;  resp.status
来源：http://hz.hywenlv.cn/gtdpldjlij.html

TS:   resp.ok;  resp.status
来源：http://hz.zhengqikj.top/gtuohlzipy.html

Java: resp.statusCode()
来源：http://hz.jqgfzy.top/gtzjxsbytj.html

Go:   resp.StatusCode
来源：http://hz.gaohongyu789.top/gthnnzsjst.html

Ruby: resp.code.to_i
来源：http://hz.snrcjt.cn/gtxnxzkiaa.html

C#:   (int)resp.StatusCode
来源：http://hz.xylfe.cn/gtpkymovrz.html

[L08] 并发请求多个地址
来源：http://hz.gotoacloud.top/gtpwpnwqgd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.cdnleiting.top/gtyxnoejbi.html

PHP:  curl_multi_init() 系列
来源：http://hz.aibaodan.cn/gtlkbiwlju.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.jyoumei.cn/gtyhjebhps.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yj202588.top/gtouqrgski.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.jlsjyb.cn/gteqvcsrvh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.sysykeji.top/gtolnyoqfu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://hz.zycfv.cn/gthtdoasgz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hz.shanyushiyangkeji.top/gthbnahjio.html

================================================================================
来源：http://hz.nanxinkj.top/gtwvnjpxin.html

M. 命令行 / 进程 / 环境
来源：http://hz.gzhubu.top/gtbmxwmtdy.html

================================================================================
来源：http://hz.nanxinkj.top/gtflfsitsb.html

[M01] 读取命令行参数
来源：http://hz.zhongyouzk.top/gtmkmoeurx.html

Py:   sys.argv[1:]
来源：http://hz.aibaodan.cn/gtgsmhggmd.html

PHP:  $argv;  $argc;
来源：http://hz.jinqigufen.top/gtnpmesaha.html


<!-- 参考信息 -->