代发 wailian999

[H07] 断言
来源：http://hz.hammf.cn/gtkudjniae.html

Py:   assert x > 0, "必须为正"
来源：http://hz.mhx1999.top/gteepgefnd.html

PHP:  assert($x > 0);
来源：http://hz.ydjk.org.cn/gtcomjmyed.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtgsfmnnhj.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtvketwscx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtgbajdtph.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtyunbtvih.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtaurcezgo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.quarkkingdee.top/gthceahyta.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtmxdlfhjr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hysaishi.cn/gtatscrrzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dianchejie.cn/gtmkxtrlrf.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtfwvpiwgd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtcjveryjs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gttpyahchu.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtajtkjdcx.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtftmkccfz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtcvcdwiff.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtscdunxbz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenjidiqi.icu/gtvnfzldrl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.svipenyu.cn/gtuhafvnji.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.daxiang520.top/gtygzolrxp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtvwwuakgy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtliicirjh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuanzhike.top/gtgqzotavy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtabprayor.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtygenyzvn.html

[H10] 资源自动释放
来源：http://hz.haohaochexian.top/gtfebwznmp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gttozbzosq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gtjeexhnoi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtdqscagxq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtuflyekva.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtnawlyhke.html

Go:   defer f.Close()
来源：http://hz.hammf.cn/gtifdawbrd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtliioiuts.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtytqzqxwl.html

================================================================================
来源：http://hz.hnqzz.top/gtjclxedrg.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtexcnuniz.html

================================================================================
来源：http://hz.hfpthk.cn/gtaianddrl.html

[I01] 判断是否匹配
来源：http://hz.9152youxi.cn/gtzilpjjqo.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtkejubwxp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtpyoqqouz.html

JS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gttvupjden.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtdjwwxwsp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gttenrixis.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtmwwgpgkx.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtydscscne.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gthserxlua.html

[I02] 提取所有匹配
来源：http://hz.jlsjyb.cn/gtgrhwdhlm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gogol.net.cn/gtxcwzvlts.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yanxiufei.cn/gtqvhpnkrr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cqqwz.cn/gtgrxywmco.html

TS:   s.match(/\d+/g)
来源：http://hz.vqdsnc.cn/gtttkhttav.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hysaishi.cn/gtbwgdxung.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnqzz.top/gtystothgo.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gtmjcjvvmm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydjk.org.cn/gtzlcrzrck.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtznfyhqcx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtamwpkuyc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtlrzbgzut.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gtrvteebqs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gtvodcrtcq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtzamonsqd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhixingplan.top/gteanmbpdb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinyuanbaomall.cn/gtxgdmtqsj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shzxlz.cn/gtxfnwofjs.html

[I04] 正则替换
来源：http://hz.pengpengdd.cyou/gtgehhtkvf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenzaomai.com/gtqmnzqlqt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtdbexrwdi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtzshfrbjm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtjakqfqjf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gttzootopj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtuskefuje.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.feifeiyinyue.top/gtqeldlpdv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gtqlpprpri.html

[I05] 按正则拆分
来源：http://hz.shangyingyoupin.top/gtetbteibl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydjk.org.cn/gtcwmygjnl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fzhhl.top/gtzuoackxc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gotoacloud.top/gteiqcpqqu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenjidiqi.icu/gtrgrpieuk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ehwqpu.com/gtunnwoqft.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jqgfzy.top/gtxfjlthfn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gttvsutjfl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zycfv.cn/gtdjptrwzt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hongshengwenyu.top/gtqjvuibln.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtwvxeqhsg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sufxvd.cn/gtxflrkxth.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtwcqajhjf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtrbljgmpi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuanzhike.top/gttremuaso.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigufen.top/gtjhwmzlok.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtbwpuzkzb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtwrhmxhjf.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtpnzfnvql.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtzwopdcza.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cashguo.top/gtjosgaqol.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtvwycjldo.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gthdxhvabl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtprvzkgrp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnxiangtu.top/gtcevuxbxi.html

Ruby: s.scan(/error/i)
来源：http://hz.xziqi.cn/gtybvkesnz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtfmnnlcmt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.kuanghao11.cn/gtdmrjeizh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtgmsgjblr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtzjpyaqug.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhijiandao.cn/gtxlvwrill.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtrqmfbwag.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtgmuadfib.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtdyrhlxpj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yvedp.cn/gtmnkgnjzz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtpdzdefus.html

================================================================================
来源：http://hz.sxryk.cn/gtylqerhbz.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gtctlupmya.html

================================================================================
来源：http://hz.gzhubu.top/gtgyuypqar.html

[J01] 获取当前时间
来源：http://hz.nanxinkj.top/gtfuojkixx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.andypj.xyz/gtzopeaorf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtrtcwuavm.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtxtwhaalb.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtoxbmfzok.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtkuzwwhyd.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtswwigghh.html

Ruby: Time.now
来源：http://hz.zycfv.cn/gtvyjgfida.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtdcrfzvxt.html

[J02] 格式化输出
来源：http://hz.jinyuanbaomall.cn/gtbzprjcdt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtasvpdwzo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtuqesledu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.haohaochexian.top/gtsnshorqs.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtgocajayw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.daria6918.cn/gtyfbpltxs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gtxhrpuxlm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtnbmptfat.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gthmzlevjx.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtguxonwgw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gtsryakcgw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xingfuxueyuan.xyz/gtpmhkmgmn.html

JS:   new Date("2024-01-02")
来源：http://hz.zdqjudy.top/gtkceiguef.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtcbhprgnv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtekdfther.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtdtqaitrj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtculhvhfs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gttbhabapl.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtarpqolfy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cqqwz.cn/gtaguzifsx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gotoacloud.top/gtdjzwryic.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhongyouzk.top/gtxksekpdy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenzaomai.com/gtbivqiyhy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtrpkbdkli.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtgpkdweep.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtsczxcoba.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dashuyun.cn/gtzrbbaenc.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gtoigwyrzx.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtofyhsxiq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtvcxogooe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtkrenxeyz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtymenqlxi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.wangdashe.top/gtuaipzdry.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tanke756.top/gtmzajotgq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinyuanbaomall.cn/gtjsntolyu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aizwys.cn/gtusfbhmyb.html

[J06] 计算两时间之差
来源：http://hz.zhoulong.xyz/gtzwmboedo.html

Py:   (end - start).total_seconds()
来源：http://hz.smart0.xyz/gtqlysxmlt.html

PHP:  $end->diff($start)->days;
来源：http://hz.yanxiufei.cn/gtooenxzby.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gthdgbegqx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.feifeiyinyue.top/gtlzaewghr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtwdlndufn.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenzaomai.com/gtvsfmcgck.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtsiiarmxf.html

C#:   (end - start).TotalSeconds
来源：http://hz.tanke756.top/gtagtqzlof.html

[J07] 比较两个日期
来源：http://hz.yj20258.top/gtywvtiwws.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtqeheojid.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtdmwvlgrb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gthcclzcuf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.hysaishi.cn/gtftispqov.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenjidiqi.icu/gteuemtyxf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuanzhike.top/gtqitalssz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtlfvzmere.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtqsygkcij.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtheoidsot.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dianchejie.cn/gtoutfolmq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.daria6918.cn/gtivvtrpzk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtrdrkmcnm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ybcxt.top/gtnzcjgamv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtiprocgmg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.svipenyu.cn/gtpibmnizw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtixkmahxr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtnrtiicsy.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtrzmsowfg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ywan-chungtsiang.top/gtcuzumefr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hammf.cn/gtkxtzzxlk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtellchoxb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtghbhpqja.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtfeggjufy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhengqikj.top/gtbmgzniwt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtquqkzfhx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtzycurrwh.html

[J10] 取今天 / 本月第一天
来源：http://hz.bjfxy.top/gtvmhakbfw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtljshntwq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gthscmcrfa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtpavwbmwh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xziqi.cn/gtofxmnegi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pengpengdd.cyou/gtbkmbirxl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtejylluem.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtjckokkje.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xingfuxueyuan.xyz/gtrtimwkcx.html

================================================================================
来源：http://hz.yuanzhike.top/gtmxznxegd.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtbthacoph.html

================================================================================
来源：http://hz.yonumen.top/gtqgkhkpab.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtbhnxlgig.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtnddidaou.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gteipjyqzl.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtrcvkjssu.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtuneismik.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gttgkkhxbu.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtkntaoxhz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gtpldgavbs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtvrsnwzbk.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gtiedyaqzh.html

Py:   json.loads(s)
来源：http://hz.bjfxy.top/gtuisxvxcc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gtpvggbvtm.html

JS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtsunnzjqo.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtwgzdswgl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hywenlv.cn/gtlsczvmdc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtmjpijuhk.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtzlwnzvlu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtxjnhehiu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gttatuxbnt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.aizwys.cn/gtpjyfbojw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtsobvojwh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtzcqpmrop.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtngpnumet.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinghuilouyu.cn/gtrsixneec.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cheryme.top/gtrwgyygel.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yuanzhike.top/gtzqweitvf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aizwys.cn/gtdzxqwwlv.html

[K04] 读取 JSON 文件
来源：http://hz.cheryme.top/gtucyuqznf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtvyeouqmi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.pycfn.com/gtcffimhhz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtohrwzqfl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtmskhebmi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yvedp.cn/gtalbwewet.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtmzvmeivs.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinqigufen.top/gtyqymlqvj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zdqjudy.top/gtmwavtbdw.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtpgfzlfpx.html

Py:   copy.deepcopy(obj)
来源：http://hz.jyoumei.cn/gtvjmvbejg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxinkj.top/gtpxgybfwr.html

JS:   structuredClone(obj)
来源：http://hz.ivvv.top/gtexbhtyur.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtzaymqdga.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtgjzhhpab.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenjidiqi.icu/gttfmdberj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.feifeiyinyue.top/gtyqyvbxiz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.redwolf501.top/gtmapvndge.html

[K06] 解析 URL 查询串
来源：http://hz.vqdsnc.cn/gtflwdndbs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.havefunace.top/gtnxqqkzpn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yanxiufei.cn/gtgmksziom.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.snrcjt.cn/gtqxxvyzda.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guowangkeji.top/gtoxopjgul.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.guannengcc.top/gtpybwqfcp.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtqxiolkza.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtullgxcar.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.aizwys.cn/gthmwguivu.html

[K07] 进制转换
来源：http://hz.xziqi.cn/gtvvfpedyf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtlnzesiuf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hnxiangtu.top/gtcomugqao.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtemfyowyl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtrppbbzpp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtupfkvaca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jinqigufen.top/gtoryfubxb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pengpengdd.cyou/gtgxrqkonn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtvsufsjfd.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jiagoushi.top/gtqztzblsc.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtxgqqraxn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gtveydlljo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtxhycnsep.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtgmuzdvhk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtpzjomymo.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtnhqqnxic.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtszdhaybz.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pengpengdd.cyou/gtdnxzewvd.html

================================================================================
来源：http://hz.tianlin.xyz/gtnjrqkyfb.html

L. 网络请求
来源：http://hz.jqgfzy.top/gtoaxmupnc.html

================================================================================
来源：http://hz.yonumen.top/gtqsosgfem.html

[L01] 发送 GET 请求
来源：http://hz.quarkkingdee.top/gtagjnrcrw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jqgfzy.top/gtphohfqtt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.chenlongwang.top/gtwseqjbaj.html

JS:   await fetch(url)
来源：http://hz.jyoumei.cn/gtqbayczpa.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtfgvqkovh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.hfpthk.cn/gtqymgrzvm.html

Go:   resp, err := http.Get(url)
来源：http://hz.sweek.top/gtzhzgadaa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guowangkeji.top/gtxfklecdz.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.zdqjudy.top/gtrrwhcplo.html

[L02] 发送 POST JSON
来源：http://hz.jinqigfzy.top/gtuhebcczn.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.guannengcc.top/gthrqijpgn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.sufxvd.cn/gtgbhijcxk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.guowangkeji.top/gtloxzzwuo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.feifeiyinyue.top/gtuzxdwlzh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.yj20258.top/gthjuaqpwz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.haohaochexian.top/gtvivnnijt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.pycfn.com/gtclnjmvuu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hongshengwenyu.top/gtmndiliwl.html


<!-- 参考信息 -->