代发 wailian999

C#:   Debug.Assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtnfhywthv.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtpewmftxn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtkvsdzonh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gtjcayfnwy.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gtsoncpqyt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtaqfeuxqq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtyykpupla.html

Go:   err.Error()
来源：http://hz.andypj.xyz/gtijwgsdiw.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtpojefzpa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtqnuzxbip.html

[H09] 带错误码的异常
来源：http://hz.guannengcc.top/gtekhrtuvd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gtypskhpff.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigufen.top/gtvcxojvdb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtnldiofdh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtjctqmarl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtmtiumztr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dianchejie.cn/gtoiuqhnjf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.9152youxi.cn/gtauejebbo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gtexizsdbo.html

[H10] 资源自动释放
来源：http://hz.chenlongwang.top/gtwslaustc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtgrdxotbl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.daria6918.cn/gtsgagnqaq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtulhppith.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtfibziizn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhiwuduotai.top/gteyvwdluh.html

Go:   defer f.Close()
来源：http://hz.tianlin.xyz/gtpkyeplcq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtqywiqtzt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.smart0.xyz/gtkdvzpsai.html

================================================================================
来源：http://hz.zhongyouzk.top/gttayaeudy.html

I. 正则表达式
来源：http://hz.ppjwa.cn/gtloglgvsy.html

================================================================================
来源：http://hz.jyoumei.cn/gtapvlitsp.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtwlrvekyb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gthajujagi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtyyhciryf.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtmivodnzq.html

TS:   /\d+/.test(s)
来源：http://hz.gaohongyu789.top/gtofvkysil.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.9152youxi.cn/gtkvvvdwoo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.9152youxi.cn/gtduwluuvo.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtvcipgxet.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtrcrbhqcd.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gtbnvpyixi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtgzxqnluj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.feifeiyinyue.top/gtsmrlwnik.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gthbsqzlng.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtlxurvfhq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gaohongyu789.top/gtaqwdyxhw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtqabovqkg.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtppwfpsxd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yvedp.cn/gtmervadiq.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtaryebkce.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.feifeiyinyue.top/gtsvdojadc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gtlubiscqj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangkeji.top/gtkgbxjtbi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.feifeiyinyue.top/gtumfurfku.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.quarkkingdee.top/gtjcimfmgg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtdxpbsnyn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtmzbxcity.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guowangkeji.top/gtiksxxpwb.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gtxfcsrury.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtbremdmiz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtfvfrzgsf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pengpengdd.cyou/gtpaoqhkmh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sufxvd.cn/gtquennjcl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtgxikojng.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cheryme.top/gtxwdmeofx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xuanzx.com/gtwhnscktl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnxiangtu.top/gtecexxaji.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtdbxrlwga.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gtoptpsnbb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtxdsaetlz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtcqjpywxh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtzmgazskk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.iojbl.cn/gtnfnhshmp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtxzvbjaxg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtllejjuwa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtvjsztppe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtrpeyzrtp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cashguo.top/gtdrplotuk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtivzcqpon.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtububddlq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtwjmhrbsn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtzqjsbnxl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtvtgfwnpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gtdyyoaizq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtmqwkxbfe.html

[I07] 忽略大小写与多行模式
来源：http://hz.cucudq.cn/gtgeqwewks.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtvbjbcnml.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtikwvnhgr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cashguo.top/gtrrnoxyue.html

TS:   /error/gim
来源：http://hz.tianlin.xyz/gtsdbzwfvv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cheryme.top/gtdiovvzxy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tianlin.xyz/gtrllbujhd.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtyxwxcqtp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtvlubonfi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zycfv.cn/gthuwcfmje.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtmftivzeo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gttzjuaoxq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtrvrnxuey.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtydhyzjvp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gthcaxjxon.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhengqikj.top/gtcftamywu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xingfuxueyuan.xyz/gtaspvmuoa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtsrnsbzud.html

================================================================================
来源：http://hz.zdqjudy.top/gtnwufebog.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gtzmgqfjuv.html

================================================================================
来源：http://hz.xylfe.cn/gtzlnmqgsq.html

[J01] 获取当前时间
来源：http://hz.jqgfzy.top/gtavocrvpg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtnqdhymgw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtiwvgrvbp.html

JS:   new Date();  Date.now()
来源：http://hz.ydzc1.top/gtdfwwztem.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtjwprjqxh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtvfuesegd.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtljszyjkn.html

Ruby: Time.now
来源：http://hz.tian-w.cn/gtljkkeuoq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.c1oappe.top/gtyaozeoyr.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtcewlwwbf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtigmzbpgr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gtzilzhklo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtygrtwweg.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gtqmjttdsa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gtrhplczgl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gteqwlpzml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtigacbsut.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtetcqjoii.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtxvcpgoxf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtheufcxun.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtlvqlyyrp.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtbjapkiia.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtsqkihdtt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtbfphkjlp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.9152youxi.cn/gtflwkqnrj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtuozyeipv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hywenlv.cn/gtrqkzghiq.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtpemqisig.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtqshmofby.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtmhxbpbxo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtjkqlbuvi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tian-w.cn/gtafhkkytu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtedfpnzer.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinyuanbaomall.cn/gteeufhwdg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtngsqqwpp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jiagoushi.top/gtyiffnaho.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gthnswtqts.html

Py:   now + timedelta(days=7)
来源：http://hz.zycfv.cn/gtocykumjj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtysgnesvh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtxkvmsbst.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtlqbgzegw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtqlduslyg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtuzhavyca.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtukmvynsj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtozhwjrif.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtaiihyoxg.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gtzjjhdjum.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtdujzcsbl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtpmnzrhai.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gtzwjuxyph.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.iojbl.cn/gtezqkdfbu.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gtdrzxgtwb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aibaodan.cn/gtaronnned.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtrnrvirvx.html

[J07] 比较两个日期
来源：http://hz.zhengqikj.top/gtbnyiwscy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtfabhqgkh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtbfugxaoi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtauhyockc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtbwxqrocf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.haohaochexian.top/gtyaffbnxr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtjlmhuzqv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtmscnhyjd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtvwwdwkdz.html

[J08] 提取年月日与星期
来源：http://hz.quarkkingdee.top/gtpwdqpiie.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sxryk.cn/gtqqgqgzee.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nanxuanxn.top/gtnfeyaltv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gticpqiayt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtyabswqmx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.kuanghao11.cn/gtfnmvhaxr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtsdnizbwb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtxumluqga.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangdashe.top/gtwztonhqs.html

[J09] 时区处理
来源：http://hz.ppjwa.cn/gtbuefjpfn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.316326.xyz/gtqvjzicgo.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangshuangyany.cn/gtoojqdypv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenjidiqi.icu/gtpmsytwwl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtuxxpfdxg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtfokswexa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtzrdrnypo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jyoumei.cn/gtggszlbwg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangkeji.top/gtmhwwoxso.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtqlbxnylx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gthlrcwzea.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.bjfxy.top/gtpjjcwkwg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtnjtptzoz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtlwyujmjx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cqqwz.cn/gtnnkuovxj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtxfytmgji.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tanke756.top/gthocwbpvo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtvrupdtck.html

================================================================================
来源：http://hz.jyoumei.cn/gtmyjaaabe.html

K. JSON 与序列化
来源：http://hz.vqdsnc.cn/gtaorfwwxs.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtxkfdhwgy.html

[K01] 对象转 JSON 字符串
来源：http://hz.quarkkingdee.top/gtxozlecqq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtdtrnakkx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pengpengdd.cyou/gtqyvhunta.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtdzofnhgp.html

TS:   JSON.stringify(obj)
来源：http://hz.gzhubu.top/gtyjiauigh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.andypj.xyz/gthacxqnxa.html

Go:   json.Marshal(obj)
来源：http://hz.jlsjyb.cn/gtlrqxbomd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ppjwa.cn/gtnbnqmfaj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtkrsusdnj.html

[K02] JSON 字符串转对象
来源：http://hz.aibaodan.cn/gttuuiruht.html

Py:   json.loads(s)
来源：http://hz.kuanghao11.cn/gtiyczxswu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtmomqoxwh.html

JS:   JSON.parse(s)
来源：http://hz.sxryk.cn/gtafznbjir.html

TS:   JSON.parse(s)
来源：http://hz.gaohongyu789.top/gtkjrugqzv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtfvbnpvwk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gttbtkauap.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtuohqxyco.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtrumccymy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtljcyymxi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yuxming.cn/gtjbkkauwi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtctumzesi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtlrddzxyk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pengpengdd.cyou/gtoztrmgyh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtnqndggdp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.gotoacloud.top/gtjogelljc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gteetpoflx.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fengsongda.top/gtltjpmuqi.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gtphbfjiya.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gttuuoepmr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtczsirjsh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gotoacloud.top/gtxpvdchcc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtljkrhdve.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtahevwtsx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtlwlfyzzl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtvpfuarni.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtpdgbuojn.html

[K05] 深拷贝对象
来源：http://hz.yvedp.cn/gtgzlbzatb.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtoezsatri.html

PHP:  unserialize(serialize($obj));
来源：http://hz.snrcjt.cn/gtyxpypnsf.html

JS:   structuredClone(obj)
来源：http://hz.hywenlv.cn/gtslbjxrta.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtexrlphrf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.cheryme.top/gtvktrxqid.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aizwys.cn/gtodbwpfvy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ivvv.top/gteozpmvsr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.bjfxy.top/gtnenkbvjy.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtxtzxwwjl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.feifeiyinyue.top/gtlbmnefxu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtbzunccip.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gttxoagikj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtpafnlbkz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gtznswuuxu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtywxqeyyq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.redwolf501.top/gtemtbszha.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtkidhttpl.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtazcetpdh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gtwryasdxm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.sweek.top/gtcjcqkwje.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtcjmgjhcb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.52xcode.cn/gtnaqqegjq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtiffxpawo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.cqqwz.cn/gtugckecij.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nanxuanxn.top/gtyktieeiv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtnyknylax.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.pengpengdd.cyou/gtzgbvhftr.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtjayaxqjj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cucudq.cn/gtaigxvaez.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.gotoacloud.top/gtetxznaxx.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtzxbaiirc.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtrkzcsauh.html

Go:   encoding/gob
来源：http://hz.birdmap.top/gtufmncgeu.html

Ruby: Marshal.dump(obj)
来源：http://hz.shuidangran.top/gtjxakbtcs.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.svipenyu.cn/gttkfbrczb.html

================================================================================
来源：http://hz.ybcxt.top/gtmfirludp.html

L. 网络请求
来源：http://hz.nwbrower.top/gtknzpgbin.html

================================================================================
来源：http://hz.yangfankeji.com/gtizyndzuu.html

[L01] 发送 GET 请求
来源：http://hz.iojbl.cn/gtjtngtmmg.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xylfe.cn/gtxrshfiyp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ywan-chungtsiang.top/gtapvlbxpx.html

JS:   await fetch(url)
来源：http://hz.yvedp.cn/gtcaubcavp.html

TS:   await fetch(url)
来源：http://hz.guowangkeji.top/gtlxctgrbx.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xinyue.icu/gtpwrccncq.html

Go:   resp, err := http.Get(url)
来源：http://hz.zhixingplan.top/gtjzuogfju.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yueranfly.top/gtuzkjgabx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yueranfly.top/gtblncbzps.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtrhijkmvu.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.gogol.net.cn/gthnxqciea.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.wangshuangyany.cn/gtvqbfgtda.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.quarkkingdee.top/gtewmhcozz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shanyushiyangkeji.top/gtwbzadpwq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.jinyuanbaomall.cn/gtlcfbydkk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.yanxiufei.cn/gtdcuinfwn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.tian-w.cn/gtjkcjedoh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.jiagoushi.top/gtsweltxez.html

[L03] 设置自定义请求头
来源：http://hz.xziqi.cn/gtfdwltzxh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.ybcxt.top/gthyeuucwk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.quarkkingdee.top/gtnxoxrbtr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.sxryk.cn/gtvuxqapph.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.wangdashe.top/gtxfoegkur.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hz.316326.xyz/gtbreatcos.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hz.xuetiantiany.cn/gtjcewtqvd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hz.jinyuanbaomall.cn/gtfmznzzur.html


<!-- 参考信息 -->