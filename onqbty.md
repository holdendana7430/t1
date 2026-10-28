代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xziqi.cn/gtduovqckr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtagrykame.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtxevhykpv.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtyzkujmsw.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtbpmkpsiz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtalpvtisr.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtvnaaaksd.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtjcalbymv.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtbxpdtzcs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtpuvxudgv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.9152youxi.cn/gtdzniqpfc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtfjmlstug.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gtsvevxftt.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258888.top/gtondspkpb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtvldesuqy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gtxwxcjfbd.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtttossokx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yangfankeji.com/gtmqcxjvnd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.meibo888.top/gtgxrsctgz.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtojsyytdk.html

Ruby: e.message;  e.backtrace
来源：http://hz.52xcode.cn/gtadxnjalu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtfuujrevz.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtrddayfdh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gthdxiapth.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtgyxowpiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtuzmhpaiw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinghuilouyu.cn/gtitlgevib.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.andypj.xyz/gtikxedula.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jiagoushi.top/gtxvahbyzm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuanzx.com/gtlhtdudxm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtnuawpxcj.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gttqabnsan.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtkantfxub.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.quarkkingdee.top/gtzyfjcfia.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtcdszfnpk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtwejbpmdu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gtposifmly.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gtwkoodebh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jiagoushi.top/gtllteftdk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtrlvhvrof.html

================================================================================
来源：http://hz.sxryk.cn/gtotsxhdvm.html

I. 正则表达式
来源：http://hz.daxiang520.top/gtmrrbgysy.html

================================================================================
来源：http://hz.ppjwa.cn/gtrtyesfpq.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtfvwiqujv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tian-w.cn/gtgbnfdfkq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtftvseufh.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtmstkufmz.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtffqfkusz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhoulong.xyz/gtcnoqxhdl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.dashuyun.cn/gtsolhpxca.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenjidiqi.icu/gtsnlnoydy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gtiizaerjw.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtyzwyzonv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gthvcducld.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtlkadomgz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtrhqszifs.html

TS:   s.match(/\d+/g)
来源：http://hz.chenjidiqi.icu/gtwpslgxsc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtghmcmqwm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtlrplqzai.html

Ruby: s.scan(/\d+/)
来源：http://hz.jinqigfzy.top/gtbkkneutq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtaragygbm.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtzhxdygmd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtulmvilon.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cashguo.top/gtafycvurz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtylufzokh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sufxvd.cn/gtgmnavzey.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtjilcgadt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinghuilouyu.cn/gtqfwejhno.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinghuilouyu.cn/gtkbnfrgtw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtbomogqpa.html

[I04] 正则替换
来源：http://hz.zhaomingkeji.xyz/gtkrzpofij.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtnegsjyom.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.mhx1999.top/gtubhmjpfz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtdhsblqlh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtzhnuvobq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtddbcbcsd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gtufadecwm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtrciplonh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtnmvserhh.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtmtyeirdq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtzlnooqth.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yongpay.top/gtundlxsiz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtdkjoeetd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtxlxpzeve.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tian-w.cn/gtxapffzqn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cdnleiting.top/gtiraxhtul.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtkcuijvto.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dianchejie.cn/gtflxdxtxw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtutxfnfdi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtlislumat.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuanzhike.top/gtoonyikei.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gtwyzrvlos.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuetiantiany.cn/gthbamytxx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtopvdzbcr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yvedp.cn/gtdwvapvpo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtmlkyeiqa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtlwayijtk.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtmdvswddt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnqzz.top/gttrggsimn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtlkzctiym.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gtolgbguie.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtasffsjqb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.52xcode.cn/gtczsjuibj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtufukxlzg.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtjufmqssc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gthoetwvmq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtqqqyhczh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhiwuduotai.top/gtljqbrdqs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xylfe.cn/gtwgcuuqbr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtaczjkyfr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtowsmnlbg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtquefmoqr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gtwykwkoht.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.sxryk.cn/gtczgiqklo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtrevuunzi.html

================================================================================
来源：http://hz.ybcxt.top/gtubfvpcoh.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtykikwmvz.html

================================================================================
来源：http://hz.mhx1999.top/gtsbupmebd.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtachwtnah.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtkjgxtiga.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtqnhsetkn.html

JS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtsjcgobyf.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtebcesynn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gtvatbonsf.html

Go:   time.Now()
来源：http://hz.jinqigfzy.top/gtcqnrhseb.html

Ruby: Time.now
来源：http://hz.hysaishi.cn/gtpmadurev.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gzhubu.top/gtrjmcoasx.html

[J02] 格式化输出
来源：http://hz.pycfn.com/gtxiwlpkof.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtqqxgnprn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtkntgohbj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtvkjlmexd.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtweslzexz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtyinutliy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtusoejrpd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtjbajghrb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gtwhqfwqkm.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtdthrvuux.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shzxlz.cn/gtdepneusr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtipbueihq.html

JS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtwapouupi.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtplgttokk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtmtxrrqvr.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.316326.xyz/gtchopgjfu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtktjwclth.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtmtutunvn.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtttrffoqg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gteclrbdvi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtecsifbjw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gttzwyvvbb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtaodkdwvy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ppjwa.cn/gtrmkzrvfb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtoiauotas.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtfenkjyys.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtymiwgyrz.html

[J05] 时间加减（加 7 天）
来源：http://hz.nwbrower.top/gtrxeazpku.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtlwmtkrcs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yanxiufei.cn/gtoyzqfpbm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258.top/gtqyqpxyzw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtnvitfkgg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gthlzexuad.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pengpengdd.cyou/gtvsrvetsu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jianghu66.top/gtcscajytv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gteoxdoswa.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtdtrwcxsz.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtzszhougc.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtuifsaznh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shanyushiyangtech.top/gtzceobeoq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gtxevhjrnh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.birdmap.top/gtpmxlzhvp.html

Go:   end.Sub(start).Hours()
来源：http://hz.yueranfly.top/gtcacpevov.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tianlin.xyz/gtozdtznmt.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtkxxerdsl.html

[J07] 比较两个日期
来源：http://hz.feifeiyinyue.top/gtsxjciwwi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtogpovlxa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gotoacloud.top/gtsvcajzng.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gttnhfdoif.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtxyvmqqsd.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.svipenyu.cn/gtlscbixmv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtlfzhzghh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhongyouzk.top/gtstobojmh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtsmcuqgem.html

[J08] 提取年月日与星期
来源：http://hz.jlsjyb.cn/gtlpugdiap.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigfzy.top/gtnfojvccu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gtwpelttyj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hywenlv.cn/gtwjuyqtkr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgufenzy.top/gtlrptdtls.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.birdmap.top/gtvvbridgp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtmepgmxwf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dashuyun.cn/gtluxttcer.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gthezncyzp.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtrxaseosn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.52xcode.cn/gtgdlmucls.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtpkhecvwk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtelpdmebl.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtgokujkpb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigfzy.top/gtwzbvdall.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtbrlmqios.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhixingplan.top/gtpynwywqx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtencwqwdd.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gttqijfzrm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydjk.org.cn/gtnqdzsfch.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xingfuxueyuan.xyz/gtbunphyon.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtsnqcdszj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.tian-w.cn/gtneqfyzgg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtdiafcnsu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.feifeiyinyue.top/gtulyflkmt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtzlyoyzdw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hywenlv.cn/gtyzbztvjs.html

================================================================================
来源：http://hz.jinqigufen.top/gtuvljnxxz.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtblvzqywe.html

================================================================================
来源：http://hz.wangdashe.top/gthvykghnu.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtrqpsztau.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtgagmrpqv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtfvrfxpxj.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtvkeiocqq.html

TS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtspsnedug.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtzdrmgpyr.html

Go:   json.Marshal(obj)
来源：http://hz.52xcode.cn/gtgfylsnmr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtuimlyvxp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ywan-chungtsiang.top/gtalevilrq.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtwvavcadn.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gtvdjjmwic.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gtobmuxwpa.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtcqmpnejj.html

TS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtrppewywc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtnnufvvrp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtoszqodnx.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtleybbofb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtmavzcpbx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yonumen.top/gtyyhhmfhh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtiragcsrh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtgpqicjbu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtgpxgepjf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtpgasoxax.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daria6918.cn/gtexetixgt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtclfleutt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aibaodan.cn/gtfuyzypgh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtzqosvtmh.html

[K04] 读取 JSON 文件
来源：http://hz.316326.xyz/gtrmgggece.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgufenzy.top/gtdhevnwls.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sxryk.cn/gtzgjuzgqi.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gttdusycem.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtssfufcao.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtokzhngbe.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtajvalnjd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtiqnjzkxr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jyoumei.cn/gtshoakdgl.html

[K05] 深拷贝对象
来源：http://hz.shzxlz.cn/gtvjabxfcw.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuetiantiany.cn/gtqmlyfhnc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuxming.cn/gtkwlwotng.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtlerkndqk.html

TS:   structuredClone(obj)
来源：http://hz.zhixingplan.top/gtnssbfhhj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yuanzhike.top/gtlpzqdrzg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.quarkkingdee.top/gtvwhmwbvq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hysaishi.cn/gtczdwnsdm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhijiandao.cn/gtwqixxdcs.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtiuhyjqiq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenjidiqi.icu/gtskqquzfo.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gttmtobgpe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtrxyfpvhg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtvyufmqzb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhengqikj.top/gtkzmnpuxs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yuanzhike.top/gtlqiuczoz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.haohaochexian.top/gtvqgbpfgh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.fengsongda.top/gttdzuaujd.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtjybmapcb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhixingplan.top/gtkajwbclk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yangfankeji.com/gtbthgrpyy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xylfe.cn/gtjzfzxrps.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hongshengwenyu.top/gtgcstvlpf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.ehwqpu.com/gtebbpalao.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yj20258888.top/gtbafbcprk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yongpay.top/gtpaquycvq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtpvsgziux.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hammf.cn/gtiwvdkjsa.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258888.top/gthekzlzdo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gthuopmoko.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ydjk.org.cn/gthgiytpov.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtgsqfqbdh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.316326.xyz/gtjarmabfc.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtztpljkts.html

Ruby: Marshal.dump(obj)
来源：http://hz.yonumen.top/gtwbcldlmb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj20258888.top/gtujrztfcl.html

================================================================================
来源：http://hz.jiagoushi.top/gthvxqnsyb.html

L. 网络请求
来源：http://hz.chenjidiqi.icu/gtmeoktimo.html

================================================================================
来源：http://hz.yonumen.top/gtxudsmsgd.html

[L01] 发送 GET 请求
来源：http://hz.ydjk.org.cn/gtiqqafcug.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.smart0.xyz/gtcdguxckr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.shanyushiyangkeji.top/gtoopxidit.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtupsheahx.html

TS:   await fetch(url)
来源：http://hz.daxiang520.top/gtzlujppvo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.dianchejie.cn/gtyrgkiflo.html

Go:   resp, err := http.Get(url)
来源：http://hz.fengsongda.top/gtlpmzmrde.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.daxiang520.top/gtauaoplns.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.yongpay.top/gtvpocbcsi.html

[L02] 发送 POST JSON
来源：http://hz.yj20258888.top/gtyfrxacod.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.sweek.top/gtrkjzwbbn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.snrcjt.cn/gtdbnmfxni.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.shzxlz.cn/gtbigdltcr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yueranfly.top/gtmomhymgu.html


<!-- 参考信息 -->