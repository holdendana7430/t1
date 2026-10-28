代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtnwftatmb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gtfylkkvuw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.svipenyu.cn/gtfqzjpqas.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenlongwang.top/gtrkjulqna.html

[H07] 断言
来源：http://hz.mhx1999.top/gtzdffsybv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtnxvmcpka.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtnmtpusox.html

JS:   console.assert(x > 0);
来源：http://hz.zhengqikj.top/gtaizaasuy.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtsqzucdke.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtuzjidfhm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtswkffinz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtusmdmcsm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtvxgozuwn.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gtuymhsusm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.316326.xyz/gtkdvbwppr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ppjwa.cn/gturmcxvlu.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtotgjumtb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtrgdsoeik.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gtyefjdfyn.html

Go:   err.Error()
来源：http://hz.xinyue.icu/gtkwmrwxpb.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtrlmqxgfn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtawpkizci.html

[H09] 带错误码的异常
来源：http://hz.zhaomingkeji.xyz/gtjsfvrglx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xziqi.cn/gtejveotqc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtuwfmdyyv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtqeronzbl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtjijauqop.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.kuanghao11.cn/gthxvqsqyc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtflkqizei.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtroltawtc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtmkagmodq.html

[H10] 资源自动释放
来源：http://hz.hammf.cn/gtntsafwhv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtremhcrjg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtgxbvtbvb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtfiprgezb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtlgwblghi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gzhubu.top/gtmbyquaem.html

Go:   defer f.Close()
来源：http://hz.daria6918.cn/gtuhamtxum.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtxrayjyrc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenlongwang.top/gtfiwribhi.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtqueabpmd.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtfuoqzzbn.html

================================================================================
来源：http://hz.yongpay.top/gtgaqabxdu.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gtenaxgila.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtwqoqxfzb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gtyzydfmhl.html

JS:   /\d+/.test(s)
来源：http://hz.52xcode.cn/gtwtdbuxiw.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtliuhfnwm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtamdotywj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guowangkeji.top/gteoxjetat.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gteoychnur.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.chenzaomai.com/gtjyfetgrg.html

[I02] 提取所有匹配
来源：http://hz.gogol.net.cn/gthszuboza.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtiuvhtnzg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gtxmijlerj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtqzfllpww.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtnuqnvzhk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258.top/gtkjqbelay.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtjjwceycq.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtlzfhgtdz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtydrzipkm.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtxqrxwpiu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtkrqeyeuo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtktvxvpdw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtkgpdlqbk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gttmimcgrh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zdqjudy.top/gtdxxertyv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtgaqbfjcv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj20258.top/gtdzfqzpse.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ywan-chungtsiang.top/gtkmjxltez.html

[I04] 正则替换
来源：http://hz.jinqigufen.top/gtzpbwbfbw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtbdyyntef.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258888.top/gtqhmawfvp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtfpqcijos.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtwjuvfasz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gttoregpyg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtrccafdmj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sysykeji.top/gtdsiqtnss.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gttxnkqpfk.html

[I05] 按正则拆分
来源：http://hz.wangdashe.top/gtommgvalz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtvgkdqfjz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.vqdsnc.cn/gtsifcgsft.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.smart0.xyz/gttglizdci.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtscvicxtu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gttggjwurj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtbwgkomxh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtozlsilrx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtkaguldgi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtljesxyds.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtdngthwzn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtjmsgddcj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtbejesxtm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtdmaymhnf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jyoumei.cn/gtdeapgjjn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gtzlqejafg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.0kj1m.cn/gtzrihvftl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtplgwxtbk.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gtignileiv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtpipbnyup.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtxxnpoiyo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtkqhaupug.html

TS:   /error/gim
来源：http://hz.zhaomingkeji.xyz/gtkanmffpn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gtyqepwaxz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.0kj1m.cn/gthrrgrbxj.html

Ruby: s.scan(/error/i)
来源：http://hz.sxryk.cn/gtzbreezej.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daxiang520.top/gtzwvicykw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtaywfktcf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.meibo888.top/gtxtdkbypk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtmbmogriz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtkbpajrae.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gtmuiapjiy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtsgjgtkji.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtodnficfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtmlytqzez.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ybcxt.top/gtgtiasyij.html

================================================================================
来源：http://hz.aibaodan.cn/gtpggagzcm.html

J. 日期与时间
来源：http://hz.hammf.cn/gtiqulmixv.html

================================================================================
来源：http://hz.zhixingplan.top/gtiifmlosz.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtavexagll.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.quarkkingdee.top/gtfknuyltz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtkncciwjc.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gthxwruwup.html

TS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtmlhlygkf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hammf.cn/gtohrqzgvk.html

Go:   time.Now()
来源：http://hz.meibo888.top/gtmizijugx.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtcveirraq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtpafkssnq.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gtgvoaysvk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtmxmgqhrj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj202588.top/gtxblxrquv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cqqwz.cn/gtauhrojie.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtwtbghfiw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangtech.top/gtuadmrbrn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtzpajxjph.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gteiekxchg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtcihvsyis.html

[J03] 字符串解析为日期
来源：http://hz.pengpengdd.cyou/gtcdrxdrxx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtmdaigxtx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxuanxn.top/gtfnhgkesn.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtcqegsxqh.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gthhwubaad.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtisynrglj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cqqwz.cn/gtbefcvqzi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.havefunace.top/gtdanrwdhy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.bjfxy.top/gthzdfphbc.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtbapogptb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtseemcvhm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtqgiewtsz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtsdhpqwbk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtkxkobzsd.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtooeyjasf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.snrcjt.cn/gtxnbcwobk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangshuangyany.cn/gtucrrmivx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtarzlecmb.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtekscsjxd.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtqrxpxmug.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jyoumei.cn/gtaogcpqmz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtwacjgzkh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtiznwwnhw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtdltacnxs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydzc1.top/gtsohqjdcj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtjvgsmkvq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuanzhike.top/gtqvcskksc.html

[J06] 计算两时间之差
来源：http://hz.zhengqikj.top/gtvyjldtlf.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtvptqlpiz.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgfzy.top/gtvnuritzx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtrlencylu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtxsmkjpzg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtrtiprxlp.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtfxdlsowu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtjohnmvsg.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtfxcfkdwy.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtjxnbbhfb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtpiqafjkv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtgscmudsc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fzhhl.top/gtabyoxwdg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenzaomai.com/gtoqpbxsev.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yanxiufei.cn/gthgyyshap.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtuimtfmnm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtybbqdzrp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtcbbdzvxo.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtvuyqutmf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangtech.top/gtmkvhgopx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtzwwtuhgu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtovbkdkel.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gttiqdoaau.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ivvv.top/gtsnohavwy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinyuanbaomall.cn/gtsjuvjmdw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangdashe.top/gtazjraaek.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jiagoushi.top/gtkraznrek.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtjetaxngq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtkukzdbyh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.52xcode.cn/gtkzhuyybq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gthtdpmdub.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtpdffyfjk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtrpugnsjh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtrgzrvrur.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtlxfqakft.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.snrcjt.cn/gtwwdosgmm.html

[J10] 取今天 / 本月第一天
来源：http://hz.wangshuangyany.cn/gtomzheiwn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtalrrdsnq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtnlflvzgh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtidknsjnr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtmrmfbunr.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gzhubu.top/gtninjsnbm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtdsxwclgu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.daria6918.cn/gttumayqfo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtjutjewmm.html

================================================================================
来源：http://hz.mhx1999.top/gtmypazlrb.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gttgpczxus.html

================================================================================
来源：http://hz.chenlongwang.top/gtflpecozc.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtgawdbcus.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtabxriwst.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daria6918.cn/gtlmvcctux.html

JS:   JSON.stringify(obj)
来源：http://hz.yj20258.top/gtigbfhkqn.html

TS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtmpgblbkm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtgagufecv.html

Go:   json.Marshal(obj)
来源：http://hz.xuetiantiany.cn/gteyyugkvb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtltpkyuky.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtkedczwns.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtkuhvzisc.html

Py:   json.loads(s)
来源：http://hz.xinyue.icu/gtsqyellty.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtatipunhc.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtzxutjxka.html

TS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtwztvpfzq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj202588.top/gttgzyngsg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtpjthffwq.html

Ruby: JSON.parse(s)
来源：http://hz.dianchejie.cn/gtaizdvqck.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.dashuyun.cn/gtbfqhctpc.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtyyyhelvu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtpifzoxhn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtuuuborch.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtqyqxysqc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gttvuzqcgt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtbwummtmk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gthfekgpyn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtyshilqhw.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xinyue.icu/gtmphfsrtn.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gtavryoteh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.sxryk.cn/gtnunsdpax.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.guannengcc.top/gtvvhjgjbs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.redwolf501.top/gtyjvqoqln.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hammf.cn/gteqoyjmeh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ywan-chungtsiang.top/gtgbizxkhl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.nanxuanxn.top/gtfkbsistq.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtqkzmgdwp.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtdqumwsjr.html

[K05] 深拷贝对象
来源：http://hz.ivvv.top/gtrjuiafmk.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinyuanbaomall.cn/gtvzoqdswx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gtscmndxhf.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtbazforcz.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtwhzdcdbb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtrhqbpctd.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hongshengwenyu.top/gtqfxuimrj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.daria6918.cn/gthblmnkhy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jyoumei.cn/gtnwcbiwab.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtmpzcrtuk.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jiagoushi.top/gtbetqpxqa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.guowangkeji.top/gtscjigccw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.daria6918.cn/gtytuyhyur.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinghuilouyu.cn/gtztilwmxr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gticcjowck.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yangfankeji.com/gtwdxxhota.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yueranfly.top/gtfaadvyrl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jianghu66.top/gtabdugyvo.html

[K07] 进制转换
来源：http://hz.cucudq.cn/gtulkaamsd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jiagoushi.top/gtvwmixyjy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.fzhhl.top/gtjdiyfstk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtxfvxrdpp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtbsnyawgn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhengqikj.top/gtrontljpx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtpeudztka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ydjk.org.cn/gtlmybniwt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtnnmearpm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.meibo888.top/gtnvqyadco.html

Py:   pickle.dumps(obj)
来源：http://hz.nwbrower.top/gtmtnvircv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ydzc1.top/gtskidmkgx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.iojbl.cn/gtlubxkaoo.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gttmvctbfh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tanke756.top/gtfiqwrygi.html

Go:   encoding/gob
来源：http://hz.zycfv.cn/gtgslbstjs.html

Ruby: Marshal.dump(obj)
来源：http://hz.yj202588.top/gtdqfjxbfl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.redwolf501.top/gtoahsplin.html

================================================================================
来源：http://hz.birdmap.top/gtbnediykq.html

L. 网络请求
来源：http://hz.pycfn.com/gtawqmekyx.html

================================================================================
来源：http://hz.52xcode.cn/gtjsnlnvbq.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gttxqoxfdy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.shanyushiyangkeji.top/gtsxouhqux.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.cqqwz.cn/gtkktdqfmr.html

JS:   await fetch(url)
来源：http://hz.redwolf501.top/gtswqgxhmm.html

TS:   await fetch(url)
来源：http://hz.yvedp.cn/gthtmhrcik.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.nanxinkj.top/gtojllkisl.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtrtzmkani.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.hongshengwenyu.top/gtafzgbpea.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.andypj.xyz/gtvqsfrynm.html

[L02] 发送 POST JSON
来源：http://hz.aibaodan.cn/gtnmhpunxg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xylfe.cn/gtkwvmbuzd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.pengpengdd.cyou/gtknrmhhqc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.tanke756.top/gtikrpwdhh.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jlsjyb.cn/gtuqwxpzoh.html


<!-- 参考信息 -->