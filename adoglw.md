代发 wailian999

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cqqwz.cn/gthzlbuvvo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtqbfvpsiy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtnsfoljzx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtzioiqbzh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtifbkdxtp.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gteckitsql.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yanxiufei.cn/gtbxqhtare.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtwsyutque.html

================================================================================
来源：http://hz.zycfv.cn/gtdhnpzirw.html

I. 正则表达式
来源：http://hz.yj20258888.top/gtulwzhztj.html

================================================================================
来源：http://hz.hysaishi.cn/gtdnvfgbde.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtjmnzkups.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.wangdashe.top/gtcffhumwe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gttkonrkrb.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtpukadkbq.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtvqwpeehd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtsgjihekg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yueranfly.top/gtfgzqmehk.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtddeyznfh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.haohaochexian.top/gtpormilzb.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtkkciaegi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtrfxuruvf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtlttohcxq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.dianchejie.cn/gtvfrteatc.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtqkerpoab.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtcynjjkdw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuanzhike.top/gtouxjbggh.html

Ruby: s.scan(/\d+/)
来源：http://hz.tanke756.top/gtpajitywl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtynqifqct.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gthhhexfpy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtigdmutau.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtwftlryzj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.andypj.xyz/gtpsobtgdp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yongpay.top/gteihvutyv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtwqermwdh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sysykeji.top/gtaqfydmpt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yonumen.top/gtktzhmqzv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.316326.xyz/gtjalttuvq.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtfisjisza.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pycfn.com/gtctmkeaqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtihpzazin.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gticjktptm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtjksrbupj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtvmwrocdn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gttrrkaztz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtssdqmhhn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtumvnlnhf.html

[I05] 按正则拆分
来源：http://hz.yj202588.top/gtlpymziua.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gturzulkrw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhiwuduotai.top/gthibcpwdh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtgupnowqi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtwwemovbs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtfxqxyyua.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gtkwbqrjjg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtvbosvcho.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtjgfhylhc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gtbeqdmlgy.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gotoacloud.top/gtfgsoumhj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jiagoushi.top/gtitberbvs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gthukmwrkb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtavsgoany.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ybcxt.top/gtvdqqgziu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtvhxqwgsn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtgatrjnqr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gthnnffitj.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtganwaoht.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtkempwolr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxinkj.top/gtnxfhnclq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shangyingyoupin.top/gtnxnprxpq.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtgquvksbt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.feifeiyinyue.top/gthjimtspt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtruzkfmwo.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtemsrpigg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cashguo.top/gtppfcbzrx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtpyrqmhug.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtwatysnmq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sweek.top/gtrdlfszls.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gthplwohjo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtworevupm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtdgastzje.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yongpay.top/gtcrxspacv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.meibo888.top/gtlutyyxtr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtejukwgyu.html

================================================================================
来源：http://hz.hfpthk.cn/gtjqhvmdma.html

J. 日期与时间
来源：http://hz.ehwqpu.com/gtzryedvfe.html

================================================================================
来源：http://hz.gaohongyu789.top/gtsxvxzxby.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtxdeqaqdu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtogtmfzrh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtaiqcbljr.html

JS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gttejgmvrq.html

TS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtsfaudxks.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtvdmtmoga.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtnohhqfah.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtloqkcjfw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtydbnqyai.html

[J02] 格式化输出
来源：http://hz.zhongyouzk.top/gtxzvvacbo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtulwopkmj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtdwwvohmy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ywan-chungtsiang.top/gtpaskigey.html

TS:   d.toISOString()
来源：http://hz.zhixingplan.top/gtsbrsrpkg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtvbqkzdde.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtjspiofya.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtgofkqytv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtugjtrequ.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gtnmgidatt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yangfankeji.com/gtamkekhjg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhaomingkeji.xyz/gtqoagoqgx.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gttfyqtgnq.html

TS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtxcckqxdm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gthrahrntt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gttopyibhm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtconybzuh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtohfxobfd.html

[J04] 时间戳与日期互转
来源：http://hz.aibaodan.cn/gtuewtwktd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhoulong.xyz/gtytrqocti.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ehwqpu.com/gtscjjekbv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.quarkkingdee.top/gtrjclcqhy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.9152youxi.cn/gtwejuiwyf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gthsjwxinu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aibaodan.cn/gtowlsmtjg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtockdeznh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtwuxenxft.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenjidiqi.icu/gtphizqvhp.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtubtfiofk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxinkj.top/gtjngypbyk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtyvmogcdl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shzxlz.cn/gtdwuzmyqo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtxmptpolm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.wangdashe.top/gtdllvkpzh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtmavfqisi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtjezyhsfo.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtsaggphvl.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtuejqidkk.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtzrazkkqr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtkyhqfncn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gthccqtxel.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.andypj.xyz/gtmhthdvfq.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gtkijvjxxb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtwmvzigtd.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtizeapyuu.html

[J07] 比较两个日期
来源：http://hz.ivvv.top/gtsscssdih.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtyzoufgzc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.mhx1999.top/gtrqtddnmw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtolaxyfuo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtfmqqowlz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtcbywjyou.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtvujpqksz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtdtdnhkkf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtoqifznkq.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtoehharqh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtjfurtzcx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtvblxmwvi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtljperqii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtbcskkluv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtbkzyrupt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gtytxlmbpc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gteislpdow.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yonumen.top/gtmgqplcry.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtxyzllsct.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtqqawlycl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cucudq.cn/gtwqbqxpbx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtycjazjmj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtyskufxow.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cqqwz.cn/gttvhkbyyw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yongpay.top/gtvusyhbgk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guowangkeji.top/gthcqwhpfw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtkugtrxdk.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gtvdnronez.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtkqpsywlg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtxrfbplps.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtlyujmswg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigufen.top/gtdoxvtrof.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtvfliluzy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtqrjnbezy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtqtxynduc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydzc1.top/gtbibeqlau.html

================================================================================
来源：http://hz.yanxiufei.cn/gtncvsbeao.html

K. JSON 与序列化
来源：http://hz.c1oappe.top/gtcipzzayr.html

================================================================================
来源：http://hz.zdqjudy.top/gthmhhxlwf.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtotdytgcu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hammf.cn/gtbufnbovk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtycwompvq.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtiolazwxk.html

TS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtfuhdqabl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhaomingkeji.xyz/gtsabkqqqk.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258.top/gtrurblsgn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pengpengdd.cyou/gtgolzxmst.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.guowangkeji.top/gtlicxwjvb.html

[K02] JSON 字符串转对象
来源：http://hz.bjfxy.top/gtwcdmncsq.html

Py:   json.loads(s)
来源：http://hz.birdmap.top/gtyxutcfog.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258888.top/gtyzilyboc.html

JS:   JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtkauosqmp.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtcihkwotw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gttaylzeze.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtqwgelcxb.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtguvyeyqa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yonumen.top/gtslxwjhzs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtzfaxjvee.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtlmshgmml.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtqccqcbzz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtijyaifur.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtjsrotqcs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtenhypkrz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtjmkbdvkc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtkcyqzxql.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guannengcc.top/gtkmxvqdiy.html

[K04] 读取 JSON 文件
来源：http://hz.fengsongda.top/gtvtydfqcv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtcwkpqdvx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.wangdashe.top/gtfnlzmsxw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtueclapxc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgfzy.top/gtasnfnvxy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tian-w.cn/gtoobfamny.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.birdmap.top/gtncjchvuo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hywenlv.cn/gtinwuycjf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtwuszioyq.html

[K05] 深拷贝对象
来源：http://hz.birdmap.top/gtkgqrpxuh.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtbnnunfpo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.guannengcc.top/gtzdpuzbfw.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtottbhnbm.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtxlvukesz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhengqikj.top/gttwcdxdwc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.iojbl.cn/gtfxszwhcx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.meibo888.top/gteintjneg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.andypj.xyz/gtparfnntx.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtwgievkiy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gtuiosaiug.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtdkmfvaap.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenzaomai.com/gtuhsfvumh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtyjksuuum.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sysykeji.top/gtdlnbkfeb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtjetuiyaf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtfzsnzmcy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtafjaduqi.html

[K07] 进制转换
来源：http://hz.ppjwa.cn/gtlxutdszb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtmipuikes.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenlongwang.top/gtraiifklw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtorhzxrfn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtqphvyzfp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtzcepcvxk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258.top/gtwdcaipxl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jinqigfzy.top/gtvlsievyi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtlomsdpiu.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtxgikkwrj.html

Py:   pickle.dumps(obj)
来源：http://hz.zhoulong.xyz/gtezgwwxja.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yongpay.top/gtqomkbuyy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtysazapxm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtrxmcupws.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hfpthk.cn/gtvvlfahte.html

Go:   encoding/gob
来源：http://hz.shanyushiyangtech.top/gtrqghggiw.html

Ruby: Marshal.dump(obj)
来源：http://hz.daxiang520.top/gtsvgmpsea.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.smart0.xyz/gthazkpkhw.html

================================================================================
来源：http://hz.xinyue.icu/gthqqooqcj.html

L. 网络请求
来源：http://hz.snrcjt.cn/gtswavwllo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtvtdgotfr.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtzbkffvmb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.nwbrower.top/gtfjofovzq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.xingfuxueyuan.xyz/gthgxztuxg.html

JS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtuusxbznh.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gtytijvvbq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jiagoushi.top/gtxrdrewni.html

Go:   resp, err := http.Get(url)
来源：http://hz.yvedp.cn/gtatptwpdp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zdqjudy.top/gtntmiexyn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.aizwys.cn/gtnusxhmcg.html

[L02] 发送 POST JSON
来源：http://hz.cdnleiting.top/gtesohkvkr.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.yonumen.top/gtnwvxgwge.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtdyddzwoh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gtujwregmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.chenlongwang.top/gtfkyzcvsq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gtqliufuyd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtkyhnxjpj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zdqjudy.top/gtlxtcwons.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.gogol.net.cn/gtsopsarhu.html

[L03] 设置自定义请求头
来源：http://hz.shanyushiyangtech.top/gtpryriqzi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.hnqzz.top/gtpdckvjzo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.zycfv.cn/gtxazsprbi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.ivvv.top/gtfclzvxly.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.yueranfly.top/gtwhabfiyx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.yuanzhike.top/gtvlwcifqj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.zhijiandao.cn/gtoyieycjd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.tanke756.top/gtehdbgawf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.xinyue.icu/gtjiowrffd.html

[L04] 设置超时
来源：http://hz.iojbl.cn/gtnjuxojbo.html

Py:   requests.get(url, timeout=5)
来源：http://hz.gogol.net.cn/gtdulxrysz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.jinqigfzy.top/gtcxkbrxfb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.nanxuanxn.top/gtvxsqivls.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.xylfe.cn/gtexpwknkn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.fzhhl.top/gtpdqpiews.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.zhaomingkeji.xyz/gtthmbpgnc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.nanxuanxn.top/gtyhtotone.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.hnxiangtu.top/gtzbjecqmr.html

[L05] 上传文件（multipart）
来源：http://hz.jlsjyb.cn/gtaplfndiv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hysaishi.cn/gtcdhrlsqg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.meibo888.top/gtrbjkukmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.smart0.xyz/gtswlnkhmw.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.fzhhl.top/gtjzjchyxl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.sweek.top/gtliqqoxaa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hz.chenlongwang.top/gtxseclxaz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hz.wangdashe.top/gtauleayzh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hz.xuanzx.com/gtttldulfr.html

[L06] 解析响应为 JSON
来源：http://hz.nwbrower.top/gtosacipiz.html


<!-- 参考信息 -->