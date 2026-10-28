代发 wailian999

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtwcgxfwwf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtlaoaebld.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.bjfxy.top/gtukvbkuxm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtxbtyaazl.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtravfwcbs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtoiasvztz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtpbyarduu.html

Ruby: s.scan(/\d+/)
来源：http://hz.gaohongyu789.top/gtyzunneoo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtctvdinzo.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtthyazkdw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj20258888.top/gtlmmbguag.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgufenzy.top/gtzasxorgg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtgsctstuu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.redwolf501.top/gtjxxardwt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtuqfwtykj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtvcfmekbn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gtcvbbppuj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ppjwa.cn/gtvzugjrdg.html

[I04] 正则替换
来源：http://hz.zhiwuduotai.top/gtutheaxtp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gttfcnicpj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtrrvujjtr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtkjbkpded.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtltmclcom.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtdhimopyk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtnureovdy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yanxiufei.cn/gttjwwonri.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtibhrwlqg.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gtuvjvuzcs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tianlin.xyz/gtuxzadkrq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtkfgnqrmm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gthbdhyfba.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtsecbgnkh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydzc1.top/gtxaqfrzls.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cqqwz.cn/gtxvfianjq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtnxpzxqcm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtiorttibh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hfpthk.cn/gtwaenqblr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtnytlltkh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gtqwnjzbpz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtogjkmnic.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtrbjkxcvo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtqvdfzwuv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtiwzjyhsu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtbnsfzfrw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gttlixsect.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtclnmrvml.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shuidangran.top/gtdgapvnfc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtdpndhghz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gtfrelvcxd.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtexubbjkh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gttfhuwpkj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtitcscbsb.html

Ruby: s.scan(/error/i)
来源：http://hz.zhiwuduotai.top/gtutathslx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sufxvd.cn/gtvkbbibzh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhijiandao.cn/gttkzaygpn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtjsibcrbr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtlbfhyyie.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gttevgnugu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtccgurice.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtcccqtsaq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtndgopxxp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtbvzbzhis.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtkgehbczr.html

================================================================================
来源：http://hz.andypj.xyz/gtdncjuckq.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtvvqmeuyi.html

================================================================================
来源：http://hz.hysaishi.cn/gtzdryrafw.html

[J01] 获取当前时间
来源：http://hz.jinghuilouyu.cn/gtfsulidtq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtngpjxsty.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhongyouzk.top/gtjmuzepnc.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gthnmgugcp.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtxumyecdk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.52xcode.cn/gtuhjvymaa.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtcrkjbdzn.html

Ruby: Time.now
来源：http://hz.sweek.top/gtnfuonksr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.andypj.xyz/gtdnyxapeb.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtdsauoojw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtvqagjvwp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtdzusnhjt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtxgbxsgax.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtqahpaikp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtvnndlgyp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.c1oappe.top/gthrwbxkhh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtxzeukngx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtqxwmcqrt.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gtxzoavibl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtkykkqsly.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtjqyfopwk.html

JS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtcspvsxdt.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxuanxn.top/gtirgpnjre.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtfeglnfhf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dianchejie.cn/gtzgtiztry.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtyokmutqi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtkjlomsde.html

[J04] 时间戳与日期互转
来源：http://hz.316326.xyz/gthjyesesa.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtkqquspys.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtrjfagctx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtwrcnhxwk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuetiantiany.cn/gtofquwgfg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtzdueenas.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tianlin.xyz/gtuoiwwjvd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtytdubtuo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.birdmap.top/gtdninujma.html

[J05] 时间加减（加 7 天）
来源：http://hz.vqdsnc.cn/gtuawgfwes.html

Py:   now + timedelta(days=7)
来源：http://hz.chenjidiqi.icu/gtgilamckq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtzfpgiltb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtokojbapz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtampbtwed.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtjswtsuic.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtoovjyahq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.daria6918.cn/gtqlacwimv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtgbxxyovp.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtoobgfoft.html

Py:   (end - start).total_seconds()
来源：http://hz.xuetiantiany.cn/gtiozrwlha.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtgypnmmjg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtzdhuteqr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtfaapqhar.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gzhubu.top/gtibrqogaw.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtuyxyntyn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.52xcode.cn/gtcgwcdzft.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtghwiamyv.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangkeji.top/gtkdudvgoz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtmetezpol.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jqgufenzy.top/gthizpqlgd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jqgufenzy.top/gtiwepqlzt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtoblptrrz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenjidiqi.icu/gtltjtksqp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtrswwhdbg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtkxmivcrj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtksktsnnw.html

[J08] 提取年月日与星期
来源：http://hz.aibaodan.cn/gtjtslutji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtjrbhnfih.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtbwkdfyzb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtpyjqsdwz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtaxtszvpe.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ywan-chungtsiang.top/gtlvryjxbd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.redwolf501.top/gthnkqvuid.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinyuanbaomall.cn/gtqsombkth.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xingfuxueyuan.xyz/gtlspiitul.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtrngoprxm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gttqkluzhk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtotqqvact.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtendemlnm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gthumpqzvi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtyfremesp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtzjcftxzr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtcelecqkr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nanxinkj.top/gthrwhmsfx.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gttnqkorib.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gtvrrwdbae.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gttfshrqra.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtldbtcjnr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtzmqhpten.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gtzodhawok.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtqjmedfjr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtitoikojx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.vqdsnc.cn/gtxaabiaud.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtunobzeal.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtlpmaoahh.html

================================================================================
来源：http://hz.316326.xyz/gtnsijygvl.html

[K01] 对象转 JSON 字符串
来源：http://hz.yuanzhike.top/gtsvggxprs.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gthyzpkmxf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtmatulzko.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtcjknlscr.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtwtoeoroe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtzmzkkdby.html

Go:   json.Marshal(obj)
来源：http://hz.sufxvd.cn/gtfvcecmta.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuetiantiany.cn/gtqryyspvp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtvpxmdlro.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtpgejroil.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtfvlzvecz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtaumzfcka.html

JS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtchzdssap.html

TS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtrmkcfyal.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtlzmghchc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guowangkeji.top/gtpruuqbev.html

Ruby: JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtwkcfvfmm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xinyue.icu/gtwppjdbif.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gtmwcykgzw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtcaavwrfn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtbtskyjxz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hammf.cn/gtjkgqhqvn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yangfankeji.com/gtucsrgbww.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shzxlz.cn/gtinwbcebw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jyoumei.cn/gtwhwopsrv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtxexkidcq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tian-w.cn/gtrauaemco.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtuodiwflo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuetiantiany.cn/gtaizqxngd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.9152youxi.cn/gtrsnfiltn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtloouohnb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tian-w.cn/gtkxfcpqus.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gtsqwbiolz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtuugqgehh.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtvbnuswvo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtrqndznqv.html

[K05] 深拷贝对象
来源：http://hz.chenlongwang.top/gtbuhqnpvg.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtzqehqlji.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gtcqbhwydx.html

JS:   structuredClone(obj)
来源：http://hz.52xcode.cn/gtirtejwpa.html

TS:   structuredClone(obj)
来源：http://hz.ehwqpu.com/gtsglqfkdx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yonumen.top/gthudyiasf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gttgiectmd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gogol.net.cn/gtfdckgtzz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtonuffqch.html

[K06] 解析 URL 查询串
来源：http://hz.zycfv.cn/gtornjrsgw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.nanxinkj.top/gtcxzrodiw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gtcocabcme.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.wangdashe.top/gtwfmzkuqg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhengqikj.top/gtpwyurvat.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.andypj.xyz/gtxeumgoyn.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zdqjudy.top/gtnysxvpvw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinqigufen.top/gtwqcyifac.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtbtqeuefk.html

[K07] 进制转换
来源：http://hz.snrcjt.cn/gtuxbnncgm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cashguo.top/gtvzwzorle.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtvpcffacd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtfzjmoogh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtzclmhwag.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.c1oappe.top/gtyxuxyldk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtppecwfji.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtjlldzhki.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinyuanbaomall.cn/gtlfzmygou.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinqigfzy.top/gtcwhvsnuw.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gttonsqndb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jyoumei.cn/gtiuqhrtvs.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtexxwlznh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtpjahxgcn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuxming.cn/gtsmrodefi.html

Go:   encoding/gob
来源：http://hz.svipenyu.cn/gtepliguyz.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtbwdibath.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtfjaizacp.html

================================================================================
来源：http://hz.cqqwz.cn/gtetuvkfqo.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtqaigcsva.html

================================================================================
来源：http://hz.yj20258888.top/gtyenbogkn.html

[L01] 发送 GET 请求
来源：http://hz.yuxming.cn/gthqttjymr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuetiantiany.cn/gtotmufczo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.yongpay.top/gtvkycwitn.html

JS:   await fetch(url)
来源：http://hz.hywenlv.cn/gthopdxjpw.html

TS:   await fetch(url)
来源：http://hz.xinyue.icu/gtxetbslos.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gteffwhxxv.html

Go:   resp, err := http.Get(url)
来源：http://hz.yj20258.top/gtayaolvvm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hysaishi.cn/gtomrcnvzj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zhiwuduotai.top/gtaqjytkmq.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtvelkrgbj.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtvvcryryn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.haohaochexian.top/gtdyslmitm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.9152youxi.cn/gtuhmsaeyg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ywan-chungtsiang.top/gtrtnwbnjh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.svipenyu.cn/gtvnhxgulp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.ivvv.top/gtjaqwnvpu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.jiagoushi.top/gtuigwncyt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtshprjibg.html

[L03] 设置自定义请求头
来源：http://hz.sweek.top/gtbnmcfazu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.cashguo.top/gtkunkmvrw.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jianghu66.top/gtsuhuneyp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.iojbl.cn/gtcqggevle.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ydjk.org.cn/gtioucsmfa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.jiagoushi.top/gtljugxgha.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jqgufenzy.top/gtcstsyopm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.hammf.cn/gtizpkwvqj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yj202588.top/gtmgeoorhf.html

[L04] 设置超时
来源：http://hz.xziqi.cn/gtydgovwra.html

Py:   requests.get(url, timeout=5)
来源：http://hz.bjfxy.top/gtgiwvguny.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.yanxiufei.cn/gtomlzcsga.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.hnqzz.top/gtyfdkupnv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.haohaochexian.top/gtcwgbjopt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.gaohongyu789.top/gtfltxmigw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.kuanghao11.cn/gtyvwhkqay.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.yuanzhike.top/gthsjwkrhj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.guannengcc.top/gtcvidodio.html

[L05] 上传文件（multipart）
来源：http://hz.sysykeji.top/gtalavjodf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.jinqigfzy.top/gtxvrtuqpp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.0kj1m.cn/gtbnadqhcu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.ywan-chungtsiang.top/gtuhsngwhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.9152youxi.cn/gtplqgggks.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.jinghuilouyu.cn/gttggynbvp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.gotoacloud.top/gtokbpnchk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangshuangyany.cn/gtqbvootyi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.yj20258.top/gtoqfjuusa.html

[L06] 解析响应为 JSON
来源：http://hz.cqqwz.cn/gttxqsqfyi.html

Py:   resp.json()
来源：http://hz.hfpthk.cn/gttdrauewe.html

PHP:  json_decode($body, true);
来源：http://hz.cashguo.top/gtsplfxpag.html

JS:   await resp.json()
来源：http://hz.chenjidiqi.icu/gtapypzfvo.html

TS:   await resp.json()
来源：http://hz.shangyingyoupin.top/gtshkmnqmk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hz.zdqjudy.top/gtbasqpjqt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hz.cheryme.top/gtvdzhczwi.html

Ruby: JSON.parse(resp.body)
来源：http://hz.jyoumei.cn/gtkfpfubpi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://hz.zhoulong.xyz/gtzpeufxdc.html

[L07] 处理 HTTP 状态码
来源：http://hz.ppjwa.cn/gtymiijhld.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hz.havefunace.top/gthyqwppxo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hz.zhoulong.xyz/gtkfnqwsma.html

JS:   resp.ok;  resp.status
来源：http://hz.gotoacloud.top/gtzaiihnbp.html

TS:   resp.ok;  resp.status
来源：http://hz.wangshuangyany.cn/gtnguvhmib.html

Java: resp.statusCode()
来源：http://hz.ybcxt.top/gtcscaugfl.html

Go:   resp.StatusCode
来源：http://hz.yvedp.cn/gtsiujzkrf.html

Ruby: resp.code.to_i
来源：http://hz.zhongyouzk.top/gtwrrgkmss.html

C#:   (int)resp.StatusCode
来源：http://hz.dianchejie.cn/gtwwfulcjv.html

[L08] 并发请求多个地址
来源：http://hz.yuanzhike.top/gtjfqzvuey.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://hz.daria6918.cn/gthriqzvnp.html

PHP:  curl_multi_init() 系列
来源：http://hz.jinqigfzy.top/gtnyrnekll.html


<!-- 参考信息 -->