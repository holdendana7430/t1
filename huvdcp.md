代发 wailian999

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtipjxwwyd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhengqikj.top/gtttdafkin.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtwwfsboaq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtiedpflnr.html

[I02] 提取所有匹配
来源：http://hz.sweek.top/gtrbqtwkng.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtygzwmmog.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xinyue.icu/gtpzktoihw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtykxihoet.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtwnamdpou.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuanzhike.top/gtxkhnsfet.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtyybiulio.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtsairqmqu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtydwwdfmb.html

[I03] 提取捕获分组
来源：http://hz.andypj.xyz/gtbpmaszog.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yonumen.top/gtwetmijwi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtexrskffb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtcjukjmam.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtryazrkxn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ywan-chungtsiang.top/gteklbtihb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenzaomai.com/gtihcukczo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.iojbl.cn/gtgpnslqno.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hywenlv.cn/gtrhqfacde.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtijgsgita.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtkhfivajh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtrohbjljy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtnziurwqd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtslvkslao.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtrjluunwi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtznkxdiyq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuetiantiany.cn/gttsmdrrop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtuipljbwg.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtowugdgqu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.gzhubu.top/gtotzejrnu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.vqdsnc.cn/gtniemcftn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtetbvbqdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtujmoglkn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtytfnufzj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.andypj.xyz/gtlxyejcwk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtvgfmbadw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtdyplkcpb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gthqfcllil.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtzoctccvz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtixrkqkje.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtbosnhiss.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtmttusvsw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtdukatfmi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtkhnbdeha.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dianchejie.cn/gtvixmnyte.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtwatldxlh.html

[I07] 忽略大小写与多行模式
来源：http://hz.gotoacloud.top/gtoxkquzfw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gttxsmtqxf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtaukzyzll.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.mhx1999.top/gtkwzfolqe.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtjequqkja.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.iojbl.cn/gttdetkicz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtxnachtah.html

Ruby: s.scan(/error/i)
来源：http://hz.cqqwz.cn/gthkczxhan.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtlimkaffp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigufen.top/gtfkspiivp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gtuwefsdqt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtncqjqtal.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtomdxgshk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtfnxpolmy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ywan-chungtsiang.top/gtdxzrzcrz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgfzy.top/gtxjejkbse.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuxming.cn/gtnpovojqt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtlsuxqwrh.html

================================================================================
来源：http://hz.mhx1999.top/gthygxlysw.html

J. 日期与时间
来源：http://hz.birdmap.top/gtmjekandf.html

================================================================================
来源：http://hz.zhengqikj.top/gtayrsfnls.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtyysnbdbl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtgiepxyho.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtjxatidvj.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtxpzkynhd.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtxmfarjsr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtolqixrfb.html

Go:   time.Now()
来源：http://hz.yuanzhike.top/gtfxaeqefk.html

Ruby: Time.now
来源：http://hz.tanke756.top/gtnrwuygas.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtuscrbhvx.html

[J02] 格式化输出
来源：http://hz.chenlongwang.top/gtnevuvxho.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtjkecoyku.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtfgsrxdgr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtfycilbpt.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtegsvvttg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtxkmyqmpx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtwmjqbfrl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtkqobuxeu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pengpengdd.cyou/gtkgukdxbh.html

[J03] 字符串解析为日期
来源：http://hz.jqgfzy.top/gtzotykeag.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gtoeojwulq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhiwuduotai.top/gtfrvhpglz.html

JS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtxgbrguob.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtyzkieqzh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtggtjpzmv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtvtqdzmvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtkrcwfohp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cdnleiting.top/gtvehriugu.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtfgfuxnjo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtdnobvywj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtjhvxzckr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtdhhfvuyq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgfzy.top/gtqfftrkpg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yongpay.top/gtpulnszuk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtejaziald.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtlhwnjnxj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtlwaxhbes.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gttevkhlee.html

Py:   now + timedelta(days=7)
来源：http://hz.316326.xyz/gtvhlzqzjg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtxvetbajk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtxqcalvbz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtswfaqowz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gttudunhvw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sweek.top/gtzplxokfc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtcwpttyde.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dianchejie.cn/gtciyngles.html

[J06] 计算两时间之差
来源：http://hz.iojbl.cn/gtjmmbengu.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtxynzptrv.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtitwmgbdn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtnllgzwfz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtsbgozypw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtwexzecqs.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtutatojuo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cqqwz.cn/gtkamuqdzc.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtvyxazfjp.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gteqfefgjj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtprrgidbp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtikblrwsg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtofovgaqk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtzkuiicgv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtvumlupuz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuxming.cn/gtfdtsxaij.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gthhuawplp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtcqgnayve.html

[J08] 提取年月日与星期
来源：http://hz.ppjwa.cn/gtaeiomvtn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtvcznxqon.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ydzc1.top/gtushmhlhx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtizlrzezh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangtech.top/gtogefjqrv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtmdigpcff.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sxryk.cn/gtvdbdkfec.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtcpijvhxp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtfhbjlhsj.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtvovgoejq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtjdxjbtix.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtyfdouawh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtrueyqdmv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jyoumei.cn/gtbahgraan.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.redwolf501.top/gtgiiunrcm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cdnleiting.top/gtgrbexxjj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtkgpavnxs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gogol.net.cn/gtidynuiod.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtzwbvactg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guannengcc.top/gtjkigruup.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtuuedimit.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.meibo888.top/gtlpjbmmcm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtvtmbzybn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daria6918.cn/gtziubxavk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtrryavgin.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.sysykeji.top/gtowtqkqku.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sufxvd.cn/gtgnogldij.html

================================================================================
来源：http://hz.sxryk.cn/gtkprpqgyl.html

K. JSON 与序列化
来源：http://hz.jinqigufen.top/gtrwxltmtr.html

================================================================================
来源：http://hz.aibaodan.cn/gtxoqbozxt.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtwxcmvmik.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zycfv.cn/gtujxsvrio.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gtejmbrbef.html

JS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtrkrashkx.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtbhyubyyn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gttntkwgdy.html

Go:   json.Marshal(obj)
来源：http://hz.wangdashe.top/gttrxhagky.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gttyvlzieu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtoxpraepo.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtegrpgycs.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtohtodihp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtennkvhnc.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtdskdskkc.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtzssytftq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtuewcfjug.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtqavrjovr.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtsjjgqjfc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigufen.top/gtkcvhhfbb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.feifeiyinyue.top/gtlvxgfpat.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtktckmckn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtgocecgth.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtheljevhb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtschkhfor.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtphxztfbf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtbnajmzqo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cashguo.top/gtstmxvqka.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtydmtsgzj.html

[K04] 读取 JSON 文件
来源：http://hz.cashguo.top/gtptcmvqkg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gtvnvzuprq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cashguo.top/gtoqifbydl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtzcdtmqky.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtmrduvcdx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtwlcaqqoy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.bjfxy.top/gtmyfxtekc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.svipenyu.cn/gtvuxappvr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtfbjqilec.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtowduarxq.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtfitdmjpp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gttrdsmvri.html

JS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtmfjsjnos.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtqzaenymv.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hongshengwenyu.top/gtufmvjmbx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258.top/gtdwavmbft.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.havefunace.top/gtibqsyiqz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.haohaochexian.top/gtpetocthq.html

[K06] 解析 URL 查询串
来源：http://hz.jianghu66.top/gtnylqpity.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtqivjhwxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtnuiloyez.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtmdbpvlqo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtntubovvy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.mhx1999.top/gtdiaiohoh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fzhhl.top/gtxaxanylh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhixingplan.top/gtrnuhmaxj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtgpqosoct.html

[K07] 进制转换
来源：http://hz.jiagoushi.top/gtwnexzxdn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jianghu66.top/gtibzkmtms.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtqwrpzhde.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtlowdyfph.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtapisitat.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtosewewbw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yongpay.top/gtsxnfjdon.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtogfsmtqp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtzdwqnouo.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtamuogkni.html

Py:   pickle.dumps(obj)
来源：http://hz.haohaochexian.top/gtxrbqfkfe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gthbknysnx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtuqagfexm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xylfe.cn/gtsozlwvmo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtkajkysbd.html

Go:   encoding/gob
来源：http://hz.tianlin.xyz/gtntqbcffd.html

Ruby: Marshal.dump(obj)
来源：http://hz.xingfuxueyuan.xyz/gtlfkijdrn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jiagoushi.top/gtcgheymql.html

================================================================================
来源：http://hz.birdmap.top/gtheuuobnu.html

L. 网络请求
来源：http://hz.zdqjudy.top/gtnqlaypiq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlyvykkyq.html

[L01] 发送 GET 请求
来源：http://hz.mhx1999.top/gtucwuluze.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinqigfzy.top/gtirbamrqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.redwolf501.top/gtydxiwuut.html

JS:   await fetch(url)
来源：http://hz.zycfv.cn/gtsgdskveg.html

TS:   await fetch(url)
来源：http://hz.yj202588.top/gtptvimmmg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhengqikj.top/gtkcmpdbrp.html

Go:   resp, err := http.Get(url)
来源：http://hz.haohaochexian.top/gtpdewgkik.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.fengsongda.top/gthlqvfopw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xinyue.icu/gtflwldjia.html

[L02] 发送 POST JSON
来源：http://hz.ydzc1.top/gtnsznvzto.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.zhixingplan.top/gtnyhnihsr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.cucudq.cn/gtlskzoksn.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangdashe.top/gtbjbfqtdo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.daxiang520.top/gtkrfwfjrh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.gogol.net.cn/gtjrzvtzrc.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.smart0.xyz/gtzelsphhs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.dianchejie.cn/gtxjgjgkck.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xuanzx.com/gtqdizucck.html

[L03] 设置自定义请求头
来源：http://hz.yuanzhike.top/gtlfmawoqi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.jinqigufen.top/gtszrkfrgw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.yj202588.top/gtevxgforx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tanke756.top/gtjdxmvdxi.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.gotoacloud.top/gtijziuzse.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.sxryk.cn/gtceszkdqa.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.smart0.xyz/gtzkpjlzmf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.xuanzx.com/gtbjgpoiex.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.smart0.xyz/gtxqwokzdi.html

[L04] 设置超时
来源：http://hz.hongshengwenyu.top/gtvhcmchpt.html

Py:   requests.get(url, timeout=5)
来源：http://hz.ybcxt.top/gttvhytigg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.316326.xyz/gtxpgmbvuj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.vqdsnc.cn/gtvajtcupn.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.shangyingyoupin.top/gtgtwdadei.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.jianghu66.top/gtgwfskjdd.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yj202588.top/gteotdrxwy.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.ybcxt.top/gtyzzhjhsd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.mhx1999.top/gtbhnapfoo.html

[L05] 上传文件（multipart）
来源：http://hz.zhongyouzk.top/gtffbikaqs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.zhoulong.xyz/gthyzxfzql.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.cheryme.top/gtncknlvpt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.hywenlv.cn/gtomcejgjt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.jianghu66.top/gtvhcbqlkj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.cdnleiting.top/gtvasoqcyg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jqgfzy.top/gtavkesxan.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.chenzaomai.com/gtwwegaopa.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.ydjk.org.cn/gtvemxwiwc.html

[L06] 解析响应为 JSON
来源：http://hz.fzhhl.top/gtvdedvate.html

Py:   resp.json()
来源：http://hz.pengpengdd.cyou/gtbylmoayj.html

PHP:  json_decode($body, true);
来源：http://hz.xingfuxueyuan.xyz/gtecbaanoq.html

JS:   await resp.json()
来源：http://hz.jianghu66.top/gtcckfwpwa.html

TS:   await resp.json()
来源：http://hz.c1oappe.top/gtwyjuivzm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.sufxvd.cn/gtrrastczu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.xuetiantiany.cn/gtdynvzklg.html

Ruby: JSON.parse(resp.body)
来源：http://hz.nwbrower.top/gtipyohlue.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.shzxlz.cn/gtrfgtocat.html

[L07] 处理 HTTP 状态码
来源：http://hz.ywan-chungtsiang.top/gtjhsyrkmz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.hywenlv.cn/gtpwurupbb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.vqdsnc.cn/gtzlpdtawk.html

JS:   resp.ok;  resp.status
来源：http://hz.jqgfzy.top/gtwfycuaiv.html

TS:   resp.ok;  resp.status
来源：http://hz.kuanghao11.cn/gtqwhaoigk.html

Java: resp.statusCode()
来源：http://hz.sufxvd.cn/gtfzgrbnur.html

Go:   resp.StatusCode
来源：http://hz.sufxvd.cn/gtthqutuno.html

Ruby: resp.code.to_i
来源：http://hz.chenjidiqi.icu/gtawvnhyhm.html


<!-- 参考信息 -->