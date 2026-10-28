代发 wailian999

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtmdhvsrvq.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtkcdzogvf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtgqgoeuab.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtvyqojzvd.html

================================================================================
来源：http://hz.ehwqpu.com/gtitkouren.html

I. 正则表达式
来源：http://hz.cheryme.top/gtazovoqke.html

================================================================================
来源：http://hz.aizwys.cn/gtkzoxmwiz.html

[I01] 判断是否匹配
来源：http://hz.jyoumei.cn/gtydomorcm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtpjtizbpc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtupurytov.html

JS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtcfwdbefw.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtetvngans.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtvmxxxdgk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.52xcode.cn/gtdtvhdsta.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtqeabqnti.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtglvvzxyw.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gtoqigbkbb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fzhhl.top/gtwjnhkmwr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gthuqqedlz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtibshovbl.html

TS:   s.match(/\d+/g)
来源：http://hz.dianchejie.cn/gtixnxjrao.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtdwrjnbqu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ehwqpu.com/gtiqggbmuh.html

Ruby: s.scan(/\d+/)
来源：http://hz.guannengcc.top/gtcnlrteik.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhixingplan.top/gtavphdudk.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtvjhszgac.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xingfuxueyuan.xyz/gtqupqsijw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yj202588.top/gtcixusurm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtghfwngqq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtrzzlbgot.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aibaodan.cn/gtamilsgga.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtxgsjdpvl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtfevejgsb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtigtzisad.html

[I04] 正则替换
来源：http://hz.xuanzx.com/gtnfhbvaif.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258888.top/gtgtjfgzzi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtskkptbnt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtfltmvypo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtiseudjio.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.gzhubu.top/gtlidwccwy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtgivajrrw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtggmdqhkp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gttpharjyv.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gticxaeqpo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtuspqiefz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gtcrvfowch.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gthhbwnpkx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gthkysdniz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtbnsxiqqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gttdezmfzf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtrzcrkvtt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtsspojywz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shuidangran.top/gtbpnkbxkr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gttplolvzi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xingfuxueyuan.xyz/gtejgbpnjo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtxpxcyoxe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtpzvphzmu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtjseqyien.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gteownznwf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtqvmwaehi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gthxidffft.html

[I07] 忽略大小写与多行模式
来源：http://hz.shuidangran.top/gtqocktbqu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dashuyun.cn/gtbbmklkyf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtdturlelp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtyqajhzzl.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gteqrtvzzq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.feifeiyinyue.top/gtpmchssqg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtbqemmecq.html

Ruby: s.scan(/error/i)
来源：http://hz.xziqi.cn/gtkrnadizl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtxnipqfce.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jiagoushi.top/gtzwbgiupl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sxryk.cn/gtzohpjguv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtkuizrfsx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.iojbl.cn/gtyqlxtrpl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtjoaebljk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtunhofuvh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenlongwang.top/gtenjfdzvq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtbgybrfhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtwcbvabbc.html

================================================================================
来源：http://hz.cucudq.cn/gtmoetiwoa.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtpdhkwjmq.html

================================================================================
来源：http://hz.shuidangran.top/gtrrjvjipg.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtlzsedgdd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gtxgudwocm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gttagfjqrd.html

JS:   new Date();  Date.now()
来源：http://hz.chenlongwang.top/gtnkwmgzju.html

TS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtpadqyzit.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtfqhhrqcp.html

Go:   time.Now()
来源：http://hz.jinqigfzy.top/gtmydhkarg.html

Ruby: Time.now
来源：http://hz.zhoulong.xyz/gtgtqudaji.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.wangshuangyany.cn/gtkkvplejj.html

[J02] 格式化输出
来源：http://hz.zhoulong.xyz/gtogdmfhpk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtsckzeyfn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtwgblvavx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtyouzjwoz.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtxocirraf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daria6918.cn/gtuvckmvem.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hammf.cn/gtbpukijos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtbhyjlkas.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtmrxlojio.html

[J03] 字符串解析为日期
来源：http://hz.yueranfly.top/gtjjpozerb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtpyvcnbob.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtgszpcwrt.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtcfdrhxkr.html

TS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtsnhboycl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtnesvcrxx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gtdqdokjjq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtohjajlhl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtbmhdsocm.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtewsunwgj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtqoykocgm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtfcmypdhc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtnkzbpcnw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtwqyvfgxk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtdhcvedfg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hammf.cn/gtdvtjwfsk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhoulong.xyz/gttkrnaluc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtjggciukw.html

[J05] 时间加减（加 7 天）
来源：http://hz.cqqwz.cn/gtzrugowrv.html

Py:   now + timedelta(days=7)
来源：http://hz.zhaomingkeji.xyz/gtpsheceno.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.wangdashe.top/gtuiexvhkk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtbgaiybae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtzuamejza.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtmetprfbo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtfsleamxq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.c1oappe.top/gtgbyusurr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gtzetvvlxh.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtykugttxw.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtjouozsfn.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtphkxwuky.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gttnpmqweq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zycfv.cn/gtunqkolwr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtxzlaaegm.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtcoughrxs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yvedp.cn/gtwkvhziyw.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtsplfuogq.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtahflxmus.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtnvzgfaof.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtpklpjetu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gteleztcun.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtflnknzya.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yueranfly.top/gthzjpqrbk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gteokcpmnf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtgasdjdew.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtzkwxhttf.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtvqymkptm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtdmfhbzdk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.vqdsnc.cn/gtyxfbrgkb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhongyouzk.top/gtluwjbqwf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtrmyqpvwf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zdqjudy.top/gtpzptoojc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hammf.cn/gtrqshwrnd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangshuangyany.cn/gtchvouera.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtlndzrtqa.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtjwfupkie.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jqgufenzy.top/gtmgcfkesp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtovgpesnf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gterdrendn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtfuyazmqo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhengqikj.top/gtperqjlle.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangkeji.top/gtcnxbaopv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtncsfnnzg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sysykeji.top/gtfkemkkzk.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtkueucdlt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dianchejie.cn/gtqkizarpv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fzhhl.top/gtaahyasqp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtmltmdzsa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtjuxsjeak.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtrykgfwxt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtgoplmuau.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtkqzciwoh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtlktyijla.html

================================================================================
来源：http://hz.cqqwz.cn/gtpvchhjyo.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtniibtlag.html

================================================================================
来源：http://hz.yuxming.cn/gtgfrizpqy.html

[K01] 对象转 JSON 字符串
来源：http://hz.jlsjyb.cn/gtncfzzcue.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtdwcvdyzo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtsjvimwej.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtoolilwfi.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtzingoqey.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.kuanghao11.cn/gtwmpbmfij.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtqnptcifo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.haohaochexian.top/gtqqrnkfwj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtwtbzhesh.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtogmsvauq.html

Py:   json.loads(s)
来源：http://hz.daria6918.cn/gtjqstwuhn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtgxlaobvx.html

JS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtfiqxstjk.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtybtrcuim.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daxiang520.top/gtfplxacbn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gthidlbpwv.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtnhbdtigy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gzhubu.top/gtgifwduck.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yanxiufei.cn/gtpepgkpdl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtylcbngjn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.316326.xyz/gtkmjjfwiy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtpdomjchk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtpqgnwtqo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtviwpblac.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtcbhwustp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gtdiwgriuh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cqqwz.cn/gtrlstfjec.html

[K04] 读取 JSON 文件
来源：http://hz.ybcxt.top/gtzihljclr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxuanxn.top/gtcuvefvir.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cheryme.top/gtnxuezvvs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nanxinkj.top/gtimavmdmb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtangdpzni.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gteddbqupu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtxmweovhx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtvqwzjlch.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtwrwrxanu.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtqofboaeb.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtdnbdrdwc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gthmsjvgvj.html

JS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtmsbbwfao.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtudywffjp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sweek.top/gthotpxdbv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gtllekxagb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.haohaochexian.top/gtnkfrhuno.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtnokcitxx.html

[K06] 解析 URL 查询串
来源：http://hz.snrcjt.cn/gtzkbncwfp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtbstgozpp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtcnimlxuj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtyjvphjtd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hfpthk.cn/gthaoxvuud.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xylfe.cn/gtkusrgucs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hongshengwenyu.top/gtqhfshtif.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtlpsgebjo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aibaodan.cn/gtyhfyjxmh.html

[K07] 进制转换
来源：http://hz.zhixingplan.top/gtfjpkoyyk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.snrcjt.cn/gtvytdptae.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sweek.top/gtytbcqhom.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.havefunace.top/gtojqbxfwu.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenzaomai.com/gtzmonlden.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtinhnpolq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yonumen.top/gtkmkcrjxi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtqrpoykjd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jinqigufen.top/gtqcdpxjjy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gthakaogyd.html

Py:   pickle.dumps(obj)
来源：http://hz.cdnleiting.top/gtrwoqbyps.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.shuidangran.top/gtxvpdkxcz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangkeji.top/gtltihkmoq.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuanzx.com/gtoemdfcdx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtcuqlvmap.html

Go:   encoding/gob
来源：http://hz.shuidangran.top/gtskyaojif.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtesidfjvz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtrrauurvr.html

================================================================================
来源：http://hz.chenzaomai.com/gtzkdgtpof.html

L. 网络请求
来源：http://hz.hammf.cn/gtjgoplfdl.html

================================================================================
来源：http://hz.hywenlv.cn/gtqtbgecnv.html

[L01] 发送 GET 请求
来源：http://hz.jqgufenzy.top/gtrwfukupw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.pycfn.com/gtxoafhbfa.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.pengpengdd.cyou/gtnswzjqvh.html

JS:   await fetch(url)
来源：http://hz.cheryme.top/gtlullxeud.html

TS:   await fetch(url)
来源：http://hz.aizwys.cn/gtpppuwuvx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtyzwujvdo.html

Go:   resp, err := http.Get(url)
来源：http://hz.sweek.top/gtvlqaspng.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ydzc1.top/gtbmoodzsd.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gotoacloud.top/gtbjkfjssc.html

[L02] 发送 POST JSON
来源：http://hz.jqgfzy.top/gttsmxdkhq.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtbjpnzrxs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.tanke756.top/gtjphjtbdj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenzaomai.com/gttutwpcbu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtyossykze.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sysykeji.top/gtxrcuyjsf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.nanxuanxn.top/gtfbxsaiwx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.hfpthk.cn/gtqquyqfhk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.xziqi.cn/gtluzzjuon.html

[L03] 设置自定义请求头
来源：http://hz.hongshengwenyu.top/gtwlpycirj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.wangdashe.top/gtfraswgfy.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.sufxvd.cn/gtcmgguppm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.tian-w.cn/gtwmnnxeqf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yuxming.cn/gtggaxpxzb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.vqdsnc.cn/gtckplybph.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.ivvv.top/gtnghsferl.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.yj202588.top/gtinqlnbvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.yangfankeji.com/gtgsyhbked.html

[L04] 设置超时
来源：http://hz.zhoulong.xyz/gttunqvtjx.html

Py:   requests.get(url, timeout=5)
来源：http://hz.xylfe.cn/gtpaozhnho.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.iojbl.cn/gtekedauhq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.gotoacloud.top/gtvuykqrgv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.ppjwa.cn/gtntxrxcds.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.shangyingyoupin.top/gtqxoindna.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.yongpay.top/gtnkyddwnw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jlsjyb.cn/gthbpgugev.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.cheryme.top/gtwwrfyamx.html

[L05] 上传文件（multipart）
来源：http://hz.wangshuangyany.cn/gtnprkqowd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hammf.cn/gtobzdermh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.redwolf501.top/gtlwhtwvkw.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.havefunace.top/gtiqwnzyvg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.gzhubu.top/gtqfavcxhm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.yj202588.top/gtkowofjjx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.jinghuilouyu.cn/gtqmlqbxir.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.zdqjudy.top/gtnqywekkn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.shangyingyoupin.top/gtrdphgysa.html

[L06] 解析响应为 JSON
来源：http://hz.jinghuilouyu.cn/gtyphogbwm.html

Py:   resp.json()
来源：http://hz.jlsjyb.cn/gtngktntpj.html

PHP:  json_decode($body, true);
来源：http://hz.yuanzhike.top/gtuyuobudz.html

JS:   await resp.json()
来源：http://hz.hysaishi.cn/gtcvdddzwh.html

TS:   await resp.json()
来源：http://hz.jqgfzy.top/gtxvoxggys.html


<!-- 参考信息 -->