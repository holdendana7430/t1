代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtaccwango.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gtyviwbvim.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtqyatolyn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtijcntbof.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cqqwz.cn/gtkwhbnhcg.html

[H08] 获取错误信息与堆栈
来源：http://hz.haohaochexian.top/gtxaaydmmd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtxmmuorec.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aibaodan.cn/gtljectazi.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtzdmfkbaj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.guannengcc.top/gtjucuixxh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jinghuilouyu.cn/gtnlyyogjw.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtjdkfvgqk.html

Ruby: e.message;  e.backtrace
来源：http://hz.hysaishi.cn/gtdbwebnhg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtzvkqclon.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtpfdcetan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtwpgqncsr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtwevbxcdo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtzhmkkpnt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtdkjdozjh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pycfn.com/gtyxvtotst.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtlabpbnze.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtibdajevn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gteatxaeyf.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gttzrbykaq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhoulong.xyz/gtssdqmnpp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.haohaochexian.top/gtoxrkapns.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtdyahsdsj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtjbkrsiet.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtihlgfgzm.html

Go:   defer f.Close()
来源：http://hz.birdmap.top/gtkmxvtjiy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtwrmezivd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtehreunvt.html

================================================================================
来源：http://hz.zhoulong.xyz/gtojavugcg.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtburmqpfi.html

================================================================================
来源：http://hz.0kj1m.cn/gtdajmgpkc.html

[I01] 判断是否匹配
来源：http://hz.yj202588.top/gtouthkoki.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gteidrvgsx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gaohongyu789.top/gtamrhvglf.html

JS:   /\d+/.test(s)
来源：http://hz.hnxiangtu.top/gtpzhfnmjc.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtnwlzssee.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fzhhl.top/gtxljvadqj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtnyexwrif.html

Ruby: s.match?(/\d+/)
来源：http://hz.smart0.xyz/gtkikhkxfg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtxjsxpswo.html

[I02] 提取所有匹配
来源：http://hz.xuanzx.com/gtzmaxeryu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydzc1.top/gtbmrjehvb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtbcyzuyvz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtuyqwmjlf.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtoynwggds.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtyhtmaagt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtqchpnomj.html

Ruby: s.scan(/\d+/)
来源：http://hz.guowangkeji.top/gthvdfopyw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtyqgnidln.html

[I03] 提取捕获分组
来源：http://hz.pengpengdd.cyou/gtnpwbbseh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hysaishi.cn/gtuchdkfgv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtxrmmjsbb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnqzz.top/gtynoqgawm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gticgilhmw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.wangdashe.top/gtbyeeeoyc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cqqwz.cn/gtwtlplwhw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yangfankeji.com/gtqydziqqj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dianchejie.cn/gtermvqcab.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gttsbralmt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258.top/gtpinnlksb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtbuazddhh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtbupydmga.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtdvhfpizp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gthdbiovxi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangkeji.top/gtdjkgvsdh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtjnibikrm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtfnhgxgcx.html

[I05] 按正则拆分
来源：http://hz.nanxinkj.top/gtdpvnrvsx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gtwbnnfykt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtwsrinscc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtlqessvrj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtmxgqcgfo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtjrvndtai.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtdpecucnm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtmvkgfpvb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtmqzlkhek.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtjcbwnpcm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtdkizysxt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jiagoushi.top/gtkwmhvstu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gttwcuvucx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtjbegycyl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yj202588.top/gtiamehsio.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.aibaodan.cn/gtpqhmwawg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gttpyervmu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtoeorgegt.html

[I07] 忽略大小写与多行模式
来源：http://hz.aizwys.cn/gtfswpcheu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtotugiepb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtepbjieui.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.c1oappe.top/gtmerxjouc.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtgbkdllgj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtwgiaxneg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gogol.net.cn/gtcpvxwwxs.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtbqqusxcp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtrffvxylo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shangyingyoupin.top/gtnqbaijln.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.snrcjt.cn/gtbpcinhvy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtavuqeilh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhoulong.xyz/gtdjvvgscf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtftehbswm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gthonpohbz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtkubucira.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtxiowvrbk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.52xcode.cn/gtpxxucznq.html

================================================================================
来源：http://hz.tian-w.cn/gtqbeqkbca.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtpzkbhuyf.html

================================================================================
来源：http://hz.snrcjt.cn/gteogaocfg.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtlpdcaonw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtunwmxhrl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tanke756.top/gtoqxjzoab.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtiiaisoqr.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtjmkkxrcp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxuanxn.top/gtsnluuqnd.html

Go:   time.Now()
来源：http://hz.feifeiyinyue.top/gtpdcynevy.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtoeqmcsup.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtmqcxaxit.html

[J02] 格式化输出
来源：http://hz.tanke756.top/gtngvhynyd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gthfotxooq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtluuxywej.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtdthyqkai.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtwbcurbwe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtepvytgkl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtmobyibag.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtgmphdloh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtbsmysljp.html

[J03] 字符串解析为日期
来源：http://hz.yj202588.top/gtobvhfugc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtgpwfemnt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtnxyygbbk.html

JS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtmwekwwzl.html

TS:   new Date("2024-01-02")
来源：http://hz.gaohongyu789.top/gtkwtqijju.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtlbmlkqxj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gogol.net.cn/gtutajyeqt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtinxngmtq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhongyouzk.top/gtmwpkdheq.html

[J04] 时间戳与日期互转
来源：http://hz.redwolf501.top/gtxbpctcom.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtprqkfbty.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gttnyusifb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhixingplan.top/gtjbnudvrr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shanyushiyangkeji.top/gtrepycbmk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtjvkaxycg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtkhfbmdkf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtvuatubkn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtebpqjsjq.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenzaomai.com/gtutifgcrt.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtmjhzedxv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zdqjudy.top/gtmaykwlfb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtluxlqcoy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtdseialib.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtntbhaweo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtnrydlxfe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.smart0.xyz/gtpwokyfzt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gaohongyu789.top/gtsabdmmim.html

[J06] 计算两时间之差
来源：http://hz.sufxvd.cn/gtmwenrnhl.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtskeevwhv.html

PHP:  $end->diff($start)->days;
来源：http://hz.zycfv.cn/gtqgtdgeqv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gttpojpnmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtkpchsovr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aibaodan.cn/gtihlstscc.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtonbgfltc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtcjzlfzyu.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtthyucsse.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtsvkrnvqo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtcngxewsp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258.top/gtltzgkjzf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtchievtld.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtrmonbqol.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhaomingkeji.xyz/gtlggacrqv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.fengsongda.top/gtxaecxnqa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtdbsjzvrm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtsxbjdsni.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtrozdhvwc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtynrwosjc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtqibzbvto.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtzduoxugu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtdjzdkyfy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cucudq.cn/gtmonkfnrs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gzhubu.top/gtwehogvro.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtllytakdi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gtzrnjplbp.html

[J09] 时区处理
来源：http://hz.fzhhl.top/gtzbcgxajf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gtyenwklnu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nwbrower.top/gtatofooyj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtspgwooyv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guannengcc.top/gtoqxloezp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtppamdobf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtefknoxmu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.iojbl.cn/gtzztlqbob.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ivvv.top/gtnzhfkvpr.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuetiantiany.cn/gtorecqjkn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.havefunace.top/gthiezkjmr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shzxlz.cn/gtpgemmpdu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtaioueotu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.andypj.xyz/gtmyercrrv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtyqoyouqa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guowangkeji.top/gtmbhmkbqa.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtxpzpglqt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xziqi.cn/gtdghyqfsr.html

================================================================================
来源：http://hz.cheryme.top/gtwtglsvco.html

K. JSON 与序列化
来源：http://hz.yueranfly.top/gtsciykpjj.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtltbeuckl.html

[K01] 对象转 JSON 字符串
来源：http://hz.sxryk.cn/gtaopacpkh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtpimcutmd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtzdbcleyn.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtluhtixkj.html

TS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtxqednppv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.nanxinkj.top/gtnagbdeea.html

Go:   json.Marshal(obj)
来源：http://hz.zhengqikj.top/gtajmqbkls.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtdcyeumqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtrvzxswrz.html

[K02] JSON 字符串转对象
来源：http://hz.tian-w.cn/gtfjsujizt.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtqglnmxnv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtsmkvhipe.html

JS:   JSON.parse(s)
来源：http://hz.fengsongda.top/gtdfebetfw.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtptjeyrpo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gtwetkdocy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtzbbjxlnb.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtdxdnxfib.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shanyushiyangkeji.top/gtkadxupys.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtutztfdmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj20258.top/gtwbrwokrx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtnmgloutm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtvmyiyvwm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtzhipexvs.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.dashuyun.cn/gtbvzntlsb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtxzzrogvw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtpmuyrdyt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ywan-chungtsiang.top/gtsbnznuaj.html

[K04] 读取 JSON 文件
来源：http://hz.jqgufenzy.top/gtbqwmotqx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.feifeiyinyue.top/gtpvqpvpsf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhoulong.xyz/gtasqtunym.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtczqpspyp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtctuprcqk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtkyjeults.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtfnqozgcp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shanyushiyangkeji.top/gtormqfgkb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtbzihzdko.html

[K05] 深拷贝对象
来源：http://hz.nwbrower.top/gtuzvoxnyd.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gtoeezdocb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenlongwang.top/gtxwvqxxrf.html

JS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtaefjqfae.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtsdfmthay.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.52xcode.cn/gtjqwmbkey.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.mhx1999.top/gtebfbvpor.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ppjwa.cn/gtaqujqshs.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aizwys.cn/gtseueejce.html

[K06] 解析 URL 查询串
来源：http://hz.cqqwz.cn/gtkxuxviry.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xziqi.cn/gtmllzbxpi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xinyue.icu/gtpqvfncxn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtbeopudta.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.andypj.xyz/gtlvzziutx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ybcxt.top/gtwxxdvuwq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtjjggisjf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nanxinkj.top/gtwmbxejhr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtkfkyixur.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtzioxwiks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtqeyhrxaz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtxxtbpaui.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gttincrxff.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gttzvtiydk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.feifeiyinyue.top/gtjnqayrxh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.fengsongda.top/gtsgbdgxrw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sufxvd.cn/gtsqsfcyjy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuetiantiany.cn/gtxxhkncxy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fzhhl.top/gthkolkibf.html

Py:   pickle.dumps(obj)
来源：http://hz.yonumen.top/gtlrtncvqp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gttnntslez.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.hysaishi.cn/gtypbsmrhi.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtlezkpape.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.jyoumei.cn/gtgeqwyjop.html

Go:   encoding/gob
来源：http://hz.shangyingyoupin.top/gtsktqmbjt.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinqigufen.top/gtflciqypy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.snrcjt.cn/gtwbsriezp.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtajrvpfvh.html

L. 网络请求
来源：http://hz.xingfuxueyuan.xyz/gtrobqbhwu.html

================================================================================
来源：http://hz.chenlongwang.top/gtjcupximf.html

[L01] 发送 GET 请求
来源：http://hz.yj20258.top/gtyzwmhcmn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.meibo888.top/gtdwbjrqlj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtkeyzsmgw.html

JS:   await fetch(url)
来源：http://hz.pengpengdd.cyou/gtckwkgwus.html

TS:   await fetch(url)
来源：http://hz.zhoulong.xyz/gtzoyfycvl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.jinghuilouyu.cn/gtliehsvaz.html

Go:   resp, err := http.Get(url)
来源：http://hz.ppjwa.cn/gtjelkznam.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zycfv.cn/gtcuyfdkba.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.iojbl.cn/gtzkhyzmws.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtqwksopml.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.ivvv.top/gtyaanzvur.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.0kj1m.cn/gthkzlftef.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yanxiufei.cn/gtysjhuozb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.andypj.xyz/gtsdjkhbze.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jlsjyb.cn/gtpllwnqkg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.mhx1999.top/gthqketloo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.zhengqikj.top/gtaguwmtvb.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.yj202588.top/gtzynhqtgl.html

[L03] 设置自定义请求头
来源：http://hz.xingfuxueyuan.xyz/gtpyudtwwl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.aizwys.cn/gtngvkfeds.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.pycfn.com/gtxhooddbz.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.shanyushiyangkeji.top/gtgdbcrfse.html


<!-- 参考信息 -->