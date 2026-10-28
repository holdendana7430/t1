代发 wailian999

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtnkbhddds.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtkhfyusfc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtbmflgmmw.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtjfzwnmea.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtiolrfvra.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhengqikj.top/gtsizpcbxa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtopecusyq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gttnxhvwvn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtiedxcxlb.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtqxaxbcqx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuetiantiany.cn/gtzpfqpkdf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtavktfgym.html

================================================================================
来源：http://hz.nanxuanxn.top/gtuklgmqai.html

I. 正则表达式
来源：http://hz.cqqwz.cn/gtqlhrpsmr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtdcvjdnqe.html

[I01] 判断是否匹配
来源：http://hz.sysykeji.top/gtrrdxbxxp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtyoryfjwx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtqufstnmj.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtrkusqzip.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtjyctaptu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dianchejie.cn/gtcmvtnawz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtvrtlxxxu.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtwhqcdudf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.c1oappe.top/gtvhkczpwk.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gthfbtzhry.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtgunpilzl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gtivdgfzqp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ivvv.top/gttqpghion.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtktitumyr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtkdqeshaw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gtwtcogvfx.html

Ruby: s.scan(/\d+/)
来源：http://hz.xinyue.icu/gtofyodgcn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gtnfqvwmql.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtgkndrzll.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtauzgvbnx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cashguo.top/gtjtiftumd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhiwuduotai.top/gteulwpnjb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gtnvonwgxb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hnxiangtu.top/gtfcdbfrwc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtcfimffuu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtewvvelsz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtahhhslhc.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtlkztaevw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhongyouzk.top/gtddycxzdr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtduanaycl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtzruhqowj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtztfezmsr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sweek.top/gtjhtfyxnn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.quarkkingdee.top/gttiirdwyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtokdfdvop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenlongwang.top/gtnwhixjsg.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtvleywake.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.feifeiyinyue.top/gtqipohbsi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtoasshbbb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtekaaoonm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtxshyigbz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtgobpustg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtnqzxhtfs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtseyjgjbq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangshuangyany.cn/gtynsailtl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gogol.net.cn/gthhzngwgs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtuwzxbepd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.iojbl.cn/gtovaglner.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtfnuahxus.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtdpwuohnu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zycfv.cn/gtlhjwduzm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtbhzfcgmp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tanke756.top/gtjqklgqwh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtzezpolwi.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtoatajuma.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtfvlroxhy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtnfswsxvm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtdhnbculi.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtvkbfoway.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dianchejie.cn/gtbtkwemhy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jiagoushi.top/gtqgcmipkt.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gthkljkgsi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtzkhvdbxw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jqgfzy.top/gtsyxzngjz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenzaomai.com/gtnmowumww.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ppjwa.cn/gtckzbqgmh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtgdqpdcmu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtmzlputgg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.birdmap.top/gtbnpglnzx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtggetncew.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangdashe.top/gtffrzwraf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cashguo.top/gtvmgmplsg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtrpaisqud.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtopjatlej.html

================================================================================
来源：http://hz.gzhubu.top/gthepggiup.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtpkvysmsl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.cqqwz.cn/gtltyrmbqk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtbqqetoca.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtkqndcnda.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gttniqetic.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gticjbtcne.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtelyyysom.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gthtllwkhl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtnfobfqoh.html

[J02] 格式化输出
来源：http://hz.wangshuangyany.cn/gtsvvxnzab.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gteuxckazf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtefwcbqzm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtmmjyubfp.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gtavuvfedd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtjebeezjw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtuqztxksb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gthpxvcfiq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtarwxfczh.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtligpuqua.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtotvsasdh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtqygpiqay.html

JS:   new Date("2024-01-02")
来源：http://hz.hysaishi.cn/gtmylbnuyz.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtsigutkgy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtlldorgxe.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtpgklqmoh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtisbnzxui.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtqdhhhivx.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtmsoywpei.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtaipwsurf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hfpthk.cn/gtfxfpmgmz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.316326.xyz/gtsijtzsyw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shangyingyoupin.top/gtodtyjaef.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yvedp.cn/gtsuskwvfb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtyhaortol.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.snrcjt.cn/gtxogxujgk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangkeji.top/gtvpbgwjbr.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtjcmpobun.html

Py:   now + timedelta(days=7)
来源：http://hz.redwolf501.top/gtkyjiafsd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtzafkknig.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gthyermerk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtnbhukjwd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtudwsntrb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydzc1.top/gtmhvinjkw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuanzx.com/gtjuebhhrr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gtltlxvrjb.html

[J06] 计算两时间之差
来源：http://hz.nanxuanxn.top/gtkxgdginh.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtfmhpmcsx.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtpqbxbooa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtdetwotez.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hammf.cn/gtkpttecgx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtemrtfdhe.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtixdecuzz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tian-w.cn/gtvkysrkiy.html

C#:   (end - start).TotalSeconds
来源：http://hz.hnqzz.top/gtozjkythf.html

[J07] 比较两个日期
来源：http://hz.yj20258.top/gtnsupdefs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtpavfeimv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtqczazabh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtblxhyyxz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.meibo888.top/gtnqcqdcvc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtmhrzzqgu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtsecupwvm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtmitcxhdf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gthvtjkvfu.html

[J08] 提取年月日与星期
来源：http://hz.jianghu66.top/gtzivspqyr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtwpsglcxh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhixingplan.top/gtmsrhzgtk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zycfv.cn/gtrhjcnajc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.redwolf501.top/gtemcvihvg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtvabtwwfv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtjjznjbck.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtbseusvkh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gteytyovge.html

[J09] 时区处理
来源：http://hz.haohaochexian.top/gtmmkbubos.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtplgbvweu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gtsbbaisma.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtgocqofkv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtdxtkvpsa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtvvzdxkag.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cqqwz.cn/gtsixqkgps.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj20258.top/gtepjdqsmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtsdwqzlvc.html

[J10] 取今天 / 本月第一天
来源：http://hz.redwolf501.top/gtubjtbtnw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jlsjyb.cn/gtvegnmpts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtacptuwnk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtnfvzymwo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yvedp.cn/gtiyjsiorr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gttntiogct.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.9152youxi.cn/gtorkhfjni.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtpcqlidba.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigufen.top/gtiidjzjlq.html

================================================================================
来源：http://hz.meibo888.top/gthpfexlxy.html

K. JSON 与序列化
来源：http://hz.tian-w.cn/gtuegqmppp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtjversbzu.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtqhotprmv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtllpiurjv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xingfuxueyuan.xyz/gtewnaanvu.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangtech.top/gtdemxpwko.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gttynbomax.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtkohemjbc.html

Go:   json.Marshal(obj)
来源：http://hz.gzhubu.top/gtpyqmurxo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tanke756.top/gthkzrpsgg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtolyhscfn.html

[K02] JSON 字符串转对象
来源：http://hz.nanxuanxn.top/gtcsdprfwf.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtgmokyeym.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhengqikj.top/gtidefeine.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gturgvsbhx.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtdimdzyml.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtbagdinyz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtqfcwzdkf.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gtaagnkdiz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtizdwfytv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtqcvswveb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtzfusfjoj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtawrreapk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtgqfmlxcj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hywenlv.cn/gtujxygdhl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtngrlvuen.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtdhhdzkxt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gthqbjbshp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.vqdsnc.cn/gtaqenbuol.html

[K04] 读取 JSON 文件
来源：http://hz.zhengqikj.top/gtvpioqisn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hammf.cn/gtclhrtcix.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.chenjidiqi.icu/gtssvkdeua.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtnnmijnbg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtcfjoxzqx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhengqikj.top/gtdyfhrpzi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtagndkxtf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigfzy.top/gtqvgilzsu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xziqi.cn/gtukyfacsp.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtzmwbpkfo.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gtmhhtobta.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtbokmzkhl.html

JS:   structuredClone(obj)
来源：http://hz.daria6918.cn/gtkrcouhdz.html

TS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtyqihoczx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtojsmnedd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gtrdwwwpxd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtznqyzwlu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.quarkkingdee.top/gtgtuhdvwl.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtfxfasfsz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daria6918.cn/gtnnzsghri.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtnzbzlziu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtvinunnmb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gthfpnmiui.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.kuanghao11.cn/gtpzegwhlo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.meibo888.top/gtzzdlruae.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dashuyun.cn/gtznktmjzx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tanke756.top/gtvteuwsuo.html

[K07] 进制转换
来源：http://hz.fzhhl.top/gtydquebly.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtjvcfnrgm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangtech.top/gtlpleckfr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtgeiipeuv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtkffpshkz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtqpcdmeby.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhiwuduotai.top/gtsaudqfia.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xingfuxueyuan.xyz/gtdrqasnme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yonumen.top/gtcongooxy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gtmqlvrzyo.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtsnaoipdf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.guannengcc.top/gtayevlpdy.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jinghuilouyu.cn/gtekfdbaep.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtqwhofxzu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jinqigfzy.top/gthfqgmdui.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtabzbowtp.html

Ruby: Marshal.dump(obj)
来源：http://hz.guannengcc.top/gtprwqkbkk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhiwuduotai.top/gtmwxqhglt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtlidyveyp.html

L. 网络请求
来源：http://hz.c1oappe.top/gtgsuvyswh.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlkmffhrg.html

[L01] 发送 GET 请求
来源：http://hz.xylfe.cn/gtkkueftdz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.fzhhl.top/gtstdrjauo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hfpthk.cn/gtnzbkoqrt.html

JS:   await fetch(url)
来源：http://hz.gaohongyu789.top/gtimivwxbd.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtnadapqsz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hammf.cn/gtpapbbcck.html

Go:   resp, err := http.Get(url)
来源：http://hz.jiagoushi.top/gtqstznqho.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ehwqpu.com/gtehtilntj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.shangyingyoupin.top/gttxkydppg.html

[L02] 发送 POST JSON
来源：http://hz.xziqi.cn/gtvpefahqb.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gthnmhwzgi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.redwolf501.top/gtmggzxcjj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.hammf.cn/gtlfxrnfow.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zhijiandao.cn/gtihrjzxvk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.sufxvd.cn/gtczcxwwvy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.xziqi.cn/gtvmqlyayl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhiwuduotai.top/gtnwypeigr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gtnfulhkuh.html

[L03] 设置自定义请求头
来源：http://hz.yuxming.cn/gtpynifbqe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.zhiwuduotai.top/gtljiowmlr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.mhx1999.top/gtxgdimvuz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.zycfv.cn/gtfumrwwix.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.jinyuanbaomall.cn/gtvcsmgkts.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.dianchejie.cn/gtmvgqifec.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.jiagoushi.top/gtellnbcoc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.meibo888.top/gtolrlfmbj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hz.ywan-chungtsiang.top/gtznqyoynl.html

[L04] 设置超时
来源：http://hz.ydjk.org.cn/gtfdchpemj.html

Py:   requests.get(url, timeout=5)
来源：http://hz.chenzaomai.com/gtjyuaqtxj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hz.zhaomingkeji.xyz/gttjzozrya.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.cheryme.top/gtqozlfkov.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hz.yuanzhike.top/gtrbaqjxcf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://hz.hysaishi.cn/gtkqzuelam.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hz.xingfuxueyuan.xyz/gtkefqlfax.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hz.jqgfzy.top/gtdwhlefvh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hz.nanxuanxn.top/gtjyxdbiqb.html

[L05] 上传文件（multipart）
来源：http://hz.redwolf501.top/gthzgrczsz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hz.hnqzz.top/gtpwotedal.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hz.ppjwa.cn/gtzmfpuskc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hz.bjfxy.top/gteenybmkc.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hz.svipenyu.cn/gtwmfopwyf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://hz.xinyue.icu/gtvpeckdzh.html


<!-- 参考信息 -->