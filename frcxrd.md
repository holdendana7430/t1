代发 wailian999

[H07] 断言
来源：http://hz.cdnleiting.top/gtakqkpwnb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtmuvaibhw.html

PHP:  assert($x > 0);
来源：http://hz.sufxvd.cn/gtgajxlpgn.html

JS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtdcaxqmsm.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtkhkniape.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cdnleiting.top/gtmumlinoa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtykzocpuq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.52xcode.cn/gtgvariucb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.redwolf501.top/gtrnvcghfh.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtultiqcfh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtiwgvhkva.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtcdnbsihp.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtsjoyfgpy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtsopqdohv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtgpllkxxt.html

Go:   err.Error()
来源：http://hz.316326.xyz/gtxblwbnrn.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtocwpsnss.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtylrwwoud.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtzfwikdtt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtqssmzsxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guowangkeji.top/gtwumjnirm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtnmdvnxzn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gtpkrkyrge.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtynahdaeo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gthndohqvr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.bjfxy.top/gtevwglzzh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gttctqsmcr.html

[H10] 资源自动释放
来源：http://hz.snrcjt.cn/gtyuonhcir.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtlgbgkbvo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtvfuvwpkv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtathiisqe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtukjmudtj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtfciwvjdo.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtazyrudvg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yueranfly.top/gtzyotceir.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtqyklbywq.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlpbvavvv.html

I. 正则表达式
来源：http://hz.mhx1999.top/gtqoyssbcp.html

================================================================================
来源：http://hz.gzhubu.top/gtpiusuxvm.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtyokrwrpi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuanzhike.top/gtucvrutxn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtbqdwynqt.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtdzkhspxx.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtdhoqalsn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.dashuyun.cn/gtfueslkwu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtjovecrpe.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtsqlwnmao.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yuxming.cn/gtwumyoxmv.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtopdyakek.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gtodejznvg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.iojbl.cn/gtanuskeuu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sxryk.cn/gtfpaujclp.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtbqsuoqev.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtxgqqejwr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fengsongda.top/gtmvjopaex.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuanzhike.top/gtjusghann.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gtmqwwvorj.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtxarnejbs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtygyxmuwy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtemucdano.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gthdqopwcm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtgvzjarsl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtpqeivgxw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gttikmjuzg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xziqi.cn/gtsyyjhlvv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtywaqwxjq.html

[I04] 正则替换
来源：http://hz.ivvv.top/gtspcsfouc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gogol.net.cn/gtyvmwahfd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtkgabqssi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtmqlbqhcz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtgisyobxq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhiwuduotai.top/gtzwfytety.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtuwgymyng.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yuxming.cn/gtwwrozprj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jlsjyb.cn/gtowxvsidy.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtctlqcaje.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.birdmap.top/gtkkvlvbrk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtapzuxywh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtehwwzooh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtqogdmnnr.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtjgpeszle.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gtkdgtivvv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gtjsyfcmkx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtzizotoir.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtjxtcxnzd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtgdzakzxn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ppjwa.cn/gtuywaxxnk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtcjmtqisp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtaaghugsd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtezbwaafx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nanxinkj.top/gtvypzqoox.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtlvynsqdj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtlrcndlji.html

[I07] 忽略大小写与多行模式
来源：http://hz.gaohongyu789.top/gtfumsoofc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtfsudkjtv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sysykeji.top/gtqrpiurpt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtxheobhhh.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtiwanluto.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuanzhike.top/gtrylzeiwu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jiagoushi.top/gtzwxxdewe.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtvxqrfzzp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuxming.cn/gtciretdxb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtwxkdvack.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.aizwys.cn/gtgmoiqnpc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gtclqmzthj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtvhwgmdwa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtzpzxntdq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gttadapqlo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtnsvmndni.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.iojbl.cn/gtdbqoxhka.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtidacmncc.html

================================================================================
来源：http://hz.sufxvd.cn/gttialcrfj.html

J. 日期与时间
来源：http://hz.havefunace.top/gtvpwdbtxa.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvtsxvdnr.html

[J01] 获取当前时间
来源：http://hz.hnxiangtu.top/gtrtgmzslh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtokrpttmt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.quarkkingdee.top/gtnupopcnj.html

JS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gtkocotvhs.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtabbiiucx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258.top/gtrytzaxbj.html

Go:   time.Now()
来源：http://hz.sysykeji.top/gtsedtlalr.html

Ruby: Time.now
来源：http://hz.haohaochexian.top/gtqzmjaaip.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtvqvgeeny.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtksjioykk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtraoneiaw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtqjipqvoi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtsjravqhc.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtuyemiige.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtwhtnbqzn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ybcxt.top/gtfkqhmfec.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtkejfkvqh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xziqi.cn/gtrvdpictd.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gttoxkenkb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtyjflgmpd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.svipenyu.cn/gtredpidee.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtukvezmio.html

TS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtscvtytvz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtsgcycpnu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sweek.top/gtjwlcqdtm.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtlnihzntl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtqvheaceb.html

[J04] 时间戳与日期互转
来源：http://hz.haohaochexian.top/gtonfglnot.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.birdmap.top/gtdpvbmvqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtylceplag.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtrcktbdba.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.snrcjt.cn/gtimdwqtqu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtvqxowjpj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtiqnpgaah.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guowangkeji.top/gtlqzrosws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jqgufenzy.top/gtsnbfovva.html

[J05] 时间加减（加 7 天）
来源：http://hz.shzxlz.cn/gthzzplfac.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtfnlfcion.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yueranfly.top/gtgbwviajm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtlslqbahg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtlqwgjxjq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sysykeji.top/gtfvvbepfz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtixabdmcq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtjnryneyl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtvvkdfcgy.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtakvrivta.html

Py:   (end - start).total_seconds()
来源：http://hz.ydjk.org.cn/gtzmnmsihf.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtftrjruem.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtpplgggsb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gthdqojrms.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtlxadznhx.html

Go:   end.Sub(start).Hours()
来源：http://hz.yvedp.cn/gtogxsiozp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtmmrdoetx.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtonegmjzd.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtdkyetyku.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtqrfiucpq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtcqverzde.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtljsogvsy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gtdwhhnhhl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtqptoyxbe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtzdkyhiae.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtkvnjveqs.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtfmagtzri.html

[J08] 提取年月日与星期
来源：http://hz.gotoacloud.top/gtmcehhebe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.316326.xyz/gtsiuayvjd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gttjxfzsgi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangkeji.top/gtnsegzgkr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.fzhhl.top/gtexmmittp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yanxiufei.cn/gtzrljjwef.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtclmzhiup.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtfbfhuhci.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhiwuduotai.top/gtdchllnob.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtefgtbkah.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtjhfjknad.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cucudq.cn/gtsuotnqcx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtxfwbmaga.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtirptgjui.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtprafqjul.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hammf.cn/gtyevbeubj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtpjisnjen.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigufen.top/gtjdohberw.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhengqikj.top/gtsjknzkiy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydzc1.top/gtoizuqfen.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenjidiqi.icu/gtmraqnnni.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtyjwygrmz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtdvmxcjpr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtzwcwccpv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangtech.top/gtizklhrov.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigufen.top/gtlezpydzv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangtech.top/gtzwcxfrnr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtfzoncdor.html

K. JSON 与序列化
来源：http://hz.hnqzz.top/gtabzxitdv.html

================================================================================
来源：http://hz.snrcjt.cn/gtxkojvmfl.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtgtmbbzjn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtwdbfsbkx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtdpqbxniz.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtexevczdn.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtzthjwavc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtzjblimnf.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtxuwpbjgg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dianchejie.cn/gtcyiltidm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yanxiufei.cn/gtvnetywdg.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtapadnvcr.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtdfawonwk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gtbnuxxvxn.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gttlrnzsnv.html

TS:   JSON.parse(s)
来源：http://hz.sweek.top/gtqvksqfbh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtvqlkxets.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hfpthk.cn/gthmvvpvjg.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtmsbroagk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.havefunace.top/gtwyfgdvxl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtcgburmlj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daxiang520.top/gtsontehgw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gogol.net.cn/gtrdfhhtvz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtzhlsrlor.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtxarkmcdo.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gthcmfbwdn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jyoumei.cn/gtrkvpkzrj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtbdglbdzj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shanyushiyangtech.top/gtaelpwspx.html

[K04] 读取 JSON 文件
来源：http://hz.shangyingyoupin.top/gtkrregrbt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daxiang520.top/gtyvwvzzqx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtksumgasb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtvsqrueng.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtfzdeapnn.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yongpay.top/gtubsnbsrx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtkglzixns.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtnaxadxdr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xinyue.icu/gtthlsvshc.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtylkyfmgg.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gtgevzxrtj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtjfsnldwh.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtcwsqmrds.html

TS:   structuredClone(obj)
来源：http://hz.9152youxi.cn/gtiytfjfst.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jlsjyb.cn/gtatvvflvc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guannengcc.top/gtifthfosb.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guannengcc.top/gtkwvbjkcj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtlbdmspvp.html

[K06] 解析 URL 查询串
来源：http://hz.tian-w.cn/gtckfdpeno.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtutzpwput.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258888.top/gtqjitjijw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenlongwang.top/gthxyjvupw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hysaishi.cn/gtikrwyqzj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.pengpengdd.cyou/gtbyxmhmih.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtifxvtker.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenzaomai.com/gtwplufzoq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.wangdashe.top/gtadkrfexw.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtfrhshfxh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gttlprdtre.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.gaohongyu789.top/gtyywigtxm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtowcpdaqo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtmhfsjxgv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtyzmketnh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhaomingkeji.xyz/gtlgzxrhss.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jiagoushi.top/gtbhhsflos.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dianchejie.cn/gtuvwdpkpn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.guannengcc.top/gtwfeqfgmq.html

Py:   pickle.dumps(obj)
来源：http://hz.wangshuangyany.cn/gtqpufytvh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtwycliopl.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gtwmipfbnf.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenzaomai.com/gtdsowufzx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.guowangkeji.top/gtdlzjlxfo.html

Go:   encoding/gob
来源：http://hz.guannengcc.top/gtlfojwrjb.html

Ruby: Marshal.dump(obj)
来源：http://hz.jyoumei.cn/gtvedndmay.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gtvcfnbkil.html

================================================================================
来源：http://hz.ehwqpu.com/gtlbucxgqg.html

L. 网络请求
来源：http://hz.gogol.net.cn/gtkikmytdl.html

================================================================================
来源：http://hz.hywenlv.cn/gtsqpxggse.html

[L01] 发送 GET 请求
来源：http://hz.gaohongyu789.top/gtstnftwzl.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.gogol.net.cn/gtymyiqtir.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cucudq.cn/gtzphxjilx.html

JS:   await fetch(url)
来源：http://hz.ydjk.org.cn/gtnmuduivl.html

TS:   await fetch(url)
来源：http://hz.birdmap.top/gtivcyaklw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.zhixingplan.top/gtnascdfvu.html

Go:   resp, err := http.Get(url)
来源：http://hz.hywenlv.cn/gtovgqjgan.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhongyouzk.top/gtexefhpvn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hfpthk.cn/gttytucuro.html

[L02] 发送 POST JSON
来源：http://hz.aizwys.cn/gtnkmcagqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.52xcode.cn/gtbyymtvtl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zdqjudy.top/gtfmqrelez.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.cqqwz.cn/gtqkbpxdii.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.mhx1999.top/gtobgydqqh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.hywenlv.cn/gtkbsvdhrz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.jqgufenzy.top/gtpddymhuk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.gzhubu.top/gtvtotwyom.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.daxiang520.top/gtynmcpygn.html


<!-- 参考信息 -->