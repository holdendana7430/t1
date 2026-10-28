代发 wailian999

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gtxvuimlad.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.daxiang520.top/gthqxtlgut.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtwoclkwqs.html

Ruby: s.scan(/\d+/)
来源：http://hz.tian-w.cn/gtdzbjzfwa.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.9152youxi.cn/gtfoqhvfgf.html

[I03] 提取捕获分组
来源：http://hz.fzhhl.top/gtdvsjcrbt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtpolscuvo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtyjksadtx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.0kj1m.cn/gtxgtukoyj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtbkknceel.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtjqujyhws.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gogol.net.cn/gtefjeqysr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinghuilouyu.cn/gtsxxqnyvn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtdvuvjacw.html

[I04] 正则替换
来源：http://hz.jianghu66.top/gtqnfergia.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtxxtwfqpf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtspyfvxgf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gtktxrbmvx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gthebgxyhd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gtpkwhxjvp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtkgjxkpgz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtlwxivncj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sxryk.cn/gtawrgmzxy.html

[I05] 按正则拆分
来源：http://hz.zhaomingkeji.xyz/gtyxhoegfx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.vqdsnc.cn/gtfnevukma.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtxwlbsvip.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtozrfdxmj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtsuydltum.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ivvv.top/gtdesprhyr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gttbgimgqm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gzhubu.top/gtihqfmkvj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtyswirnhf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtvbskjgoe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtbqtngxur.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtdyyrjbin.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtekwxtkpn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtivnewzdz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.316326.xyz/gtxtxbcxyd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gtdpqixrmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtwsbgzbhj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtomagnugu.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtnblibrhk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtuegmmikq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.0kj1m.cn/gtwxpagcok.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhoulong.xyz/gttxkkndni.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtsnsyyjfv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nwbrower.top/gtyhyieszp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtnwamjcml.html

Ruby: s.scan(/error/i)
来源：http://hz.gzhubu.top/gtxpzecjyl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenlongwang.top/gtgefvywmj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gaohongyu789.top/gtfkneapvf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtwwsokdih.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtcxlqcvgu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtqanechsg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtxpfhsnno.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtibxrpbqx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtghaksqxa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.gzhubu.top/gtuwajzbsq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtfhejdnhj.html

================================================================================
来源：http://hz.birdmap.top/gtmpapwptz.html

J. 日期与时间
来源：http://hz.9152youxi.cn/gtjpyswseg.html

================================================================================
来源：http://hz.hammf.cn/gtgdcpwtrq.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtdzshyeav.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigfzy.top/gtjfldqsdj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtnlusvjkr.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258.top/gtiqxdhicy.html

TS:   new Date();  Date.now()
来源：http://hz.52xcode.cn/gtwqresuqe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtbphttuni.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtkfnogtxg.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtqzmuguna.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtnifnrsyz.html

[J02] 格式化输出
来源：http://hz.hnxiangtu.top/gthsjhzwox.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtsnwrplcd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtzuidwmml.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ybcxt.top/gtxxknzddj.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtopyucxix.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yongpay.top/gtefwpaier.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtvzxaimpt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtwxddkzwx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.bjfxy.top/gtomuxruez.html

[J03] 字符串解析为日期
来源：http://hz.andypj.xyz/gttzlrapmp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtcazheuta.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dashuyun.cn/gtqczbvwir.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtmbdxdkip.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtitjftpbk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.kuanghao11.cn/gtnubvlfpz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258.top/gtgmmlqabb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtscirvizh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtgooqpbzx.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtdsckptcw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtjnkfhzyd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtynxumigd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cqqwz.cn/gtkergkufb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtbnllgkvj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhijiandao.cn/gtrnaeheyc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.quarkkingdee.top/gtpbqbfwlt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtznfxqyiw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtxirwolex.html

[J05] 时间加减（加 7 天）
来源：http://hz.tanke756.top/gtmlbamvlk.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtltdrivmo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.quarkkingdee.top/gtqyxdauiy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtpxcdfyyi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtbjlzgxsw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhixingplan.top/gtijopuwet.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yueranfly.top/gtnbblbxvt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhongyouzk.top/gtmsvrcpoh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gthajrjefa.html

[J06] 计算两时间之差
来源：http://hz.zycfv.cn/gtzkpiuufl.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtkcpsmivo.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtekzzpppo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtyrayuwfm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gthethclyj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtydeuumqy.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtcreyvtxp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtemzdtyuv.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtzmmsdxar.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gttvzypctf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtxrjtuigi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtxlbpaksk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtlovrxnty.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtjytgdksy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtfpflcutx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtjssdzijw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtmtfvruun.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtvjhdgpzp.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtuclyimjm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtoalogfwa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtlsifyppf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hongshengwenyu.top/gtewfomrft.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gogol.net.cn/gtnchlfbtz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtgueijmjv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gtzczpucjn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtzgxoujre.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtzsdwknsc.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtpbjkrjgv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtngxlzrhs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtvtyytzda.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtnwjgmbee.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtinhbgmjb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tanke756.top/gtqnlgpsbe.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtqjacmvik.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuanzhike.top/gtuguzdafz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.dianchejie.cn/gtugftwoow.html

[J10] 取今天 / 本月第一天
来源：http://hz.ybcxt.top/gtzrdwyjhb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtphlemslw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.0kj1m.cn/gtsydxfhrq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gtvujyrzty.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shangyingyoupin.top/gtkgfvdcla.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cheryme.top/gteeqavwcp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj202588.top/gtfcfdkoyj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtrvjwxens.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtywjnsvwk.html

================================================================================
来源：http://hz.sufxvd.cn/gtcfwvrhui.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtspxcgdoa.html

================================================================================
来源：http://hz.dianchejie.cn/gtektogdmy.html

[K01] 对象转 JSON 字符串
来源：http://hz.daxiang520.top/gtuigywxvy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtjpsdrogc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtrojzpkog.html

JS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtrgnsvsqx.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtdmrxmemn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtlxrpcbko.html

Go:   json.Marshal(obj)
来源：http://hz.cashguo.top/gtxifyfiuy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgfzy.top/gtjqryrpab.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuanzhike.top/gtunonadpj.html

[K02] JSON 字符串转对象
来源：http://hz.tianlin.xyz/gtjokkobmp.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtifezhrxr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtihzpzitx.html

JS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtdmscfxjb.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtgbmduqih.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sweek.top/gtylnjraeu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtbrmteyox.html

Ruby: JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtqwvqvkhl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hywenlv.cn/gtxfwfjnim.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.316326.xyz/gttxmuajas.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hnxiangtu.top/gtwfonkwia.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtxlgwkblo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtopirinjd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtbpqwdojj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cdnleiting.top/gtoyxyrgdj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtebtfkuik.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtshockxwq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtbjeutgrp.html

[K04] 读取 JSON 文件
来源：http://hz.zycfv.cn/gtvaeqhyvs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.smart0.xyz/gtjyjhvjsn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtybanlhyw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258.top/gttvmievxp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtoonezrhj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gtzheiefbv.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gtogqypfer.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.pycfn.com/gtezctscih.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gogol.net.cn/gtfhbzbasc.html

[K05] 深拷贝对象
来源：http://hz.quarkkingdee.top/gthestkdnk.html

Py:   copy.deepcopy(obj)
来源：http://hz.sysykeji.top/gtbzzdkcgv.html

PHP:  unserialize(serialize($obj));
来源：http://hz.redwolf501.top/gtsecnijhe.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtvydegzsx.html

TS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtwlozembz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtfbzvucls.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtspswyazw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gtvpzndghu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtbwklrczg.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gtqptwowil.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fengsongda.top/gtibugnlhd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xylfe.cn/gtnpqxoihh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.havefunace.top/gtnacjsjsu.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtbupndybe.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtlnzithzi.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.havefunace.top/gtzhyhspqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxuanxn.top/gtcujrnzcr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hnxiangtu.top/gtynaqyqdt.html

[K07] 进制转换
来源：http://hz.sysykeji.top/gtullijjjs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tian-w.cn/gtdbkjfnrk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gaohongyu789.top/gtizvyidzm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtktutxjhc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtqqtolcjt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.havefunace.top/gtimbysfbf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cdnleiting.top/gtuyaaxfwh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zycfv.cn/gtacucuqyz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtkgadcgaq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtvlndavry.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtxiglkbfo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.pengpengdd.cyou/gthtbkqmmh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hnxiangtu.top/gtunqxddsq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtjyyybggh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtjqkrgzmh.html

Go:   encoding/gob
来源：http://hz.sxryk.cn/gtooonkilc.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydzc1.top/gtvlfoangt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.gogol.net.cn/gtebhzygni.html

================================================================================
来源：http://hz.chenzaomai.com/gtioppmdbw.html

L. 网络请求
来源：http://hz.aibaodan.cn/gtfhqfcsjs.html

================================================================================
来源：http://hz.cqqwz.cn/gtvymbykxz.html

[L01] 发送 GET 请求
来源：http://hz.feifeiyinyue.top/gtlafefdbx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gthirxrtkk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daria6918.cn/gtyybluenm.html

JS:   await fetch(url)
来源：http://hz.yueranfly.top/gtrvdpxmik.html

TS:   await fetch(url)
来源：http://hz.jlsjyb.cn/gtohbwqvnl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yangfankeji.com/gtuqmysbwg.html

Go:   resp, err := http.Get(url)
来源：http://hz.guannengcc.top/gtnvscjmgi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.iojbl.cn/gtiqhdtout.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yonumen.top/gtgrfelmhp.html

[L02] 发送 POST JSON
来源：http://hz.xylfe.cn/gtghnqzezi.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jiagoushi.top/gtbayxqzng.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.316326.xyz/gtxajclsqs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.snrcjt.cn/gtynlkcodi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yj202588.top/gtcwsmdwxe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.chenlongwang.top/gtgkijldxu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yueranfly.top/gtikjagdck.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.feifeiyinyue.top/gtotjvowde.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ehwqpu.com/gtjjgiyhpz.html

[L03] 设置自定义请求头
来源：http://hz.yangfankeji.com/gtdmmyqrrr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.nanxinkj.top/gtlmewmztt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.guannengcc.top/gthwyskxot.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.cashguo.top/gtxiqooykv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtxskboshg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.zhiwuduotai.top/gtqozakcgo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.fzhhl.top/gtsahwqzzd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.aizwys.cn/gtdunbdmen.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.shanyushiyangkeji.top/gtazhgqukz.html

[L04] 设置超时
来源：http://hz.52xcode.cn/gtaggwfkkb.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xinyue.icu/gtnzersthf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.fzhhl.top/gtqfxgcoue.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.tian-w.cn/gtrcsrnbyo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtbmhblhwg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.yongpay.top/gtzcnoxteb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.aibaodan.cn/gtbpqswsom.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.aizwys.cn/gtnjmmorau.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.smart0.xyz/gtnarnkple.html

[L05] 上传文件（multipart）
来源：http://hz.hnxiangtu.top/gtkahpsxsb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.xuanzx.com/gtpinpclvz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.316326.xyz/gtyzcrhkjh.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtpzoymomd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.shzxlz.cn/gtqpejtoir.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.hywenlv.cn/gtscdldejf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.daxiang520.top/gtbopprxuq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.jinghuilouyu.cn/gtogsvpaqy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.fengsongda.top/gtifzepheb.html

[L06] 解析响应为 JSON
来源：http://hz.zhongyouzk.top/gtlbemjmwa.html

Py:   resp.json()
来源：http://hz.hnqzz.top/gtlwfzfhxt.html

PHP:  json_decode($body, true);
来源：http://hz.wangdashe.top/gtvezspbbo.html

JS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtgsswyavd.html

TS:   await resp.json()
来源：http://hz.zhaomingkeji.xyz/gtshjzqxan.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.cashguo.top/gtdaduuhnp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.gaohongyu789.top/gtipcltzue.html

Ruby: JSON.parse(resp.body)
来源：http://hz.meibo888.top/gtbswtgfnl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.yanxiufei.cn/gtuhajwavd.html

[L07] 处理 HTTP 状态码
来源：http://hz.cucudq.cn/gtxuoamgrl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hammf.cn/gthiwfmdcv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.c1oappe.top/gtvtfxrnfq.html

JS:   resp.ok;  resp.status
来源：http://hz.jyoumei.cn/gtsktaxwor.html

TS:   resp.ok;  resp.status
来源：http://hz.snrcjt.cn/gtnbbkdenv.html

Java: resp.statusCode()
来源：http://hz.gogol.net.cn/gtdtruohdt.html

Go:   resp.StatusCode
来源：http://hz.wangshuangyany.cn/gtjuwjnpoq.html

Ruby: resp.code.to_i
来源：http://hz.aizwys.cn/gttsqkhvpf.html

C#:   (int)resp.StatusCode
来源：http://hz.yuxming.cn/gtwchamebo.html

[L08] 并发请求多个地址
来源：http://hz.zycfv.cn/gtdclwkcck.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.haohaochexian.top/gtgfflmzpk.html

PHP:  curl_multi_init() 系列
来源：http://hz.xuetiantiany.cn/gtyqvypqqq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.cqqwz.cn/gtfrvccdjz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hz.yvedp.cn/gtzbckvvyr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hz.daria6918.cn/gtylubrimy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hz.zhaomingkeji.xyz/gtblbaghky.html


<!-- 参考信息 -->