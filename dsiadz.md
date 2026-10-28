代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtjpzolhwe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtdaowqzux.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj20258.top/gtjndqrwip.html

C#:   obj?.A?.B ?? default
来源：http://hz.hywenlv.cn/gtdatdfear.html

[H07] 断言
来源：http://hz.xinyue.icu/gtmrrxbpxh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gtqlisdmtn.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtltrapanp.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtiadpuods.html

TS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtzvafrurk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtpphbxvgi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtlintxumg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtnrmqxssq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtsctkwbwa.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxinkj.top/gtlmdelrsd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenzaomai.com/gtzosevyxk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigufen.top/gtwrgydfhb.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtfnvuicrp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtwgoizwym.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtdolrwrbk.html

Go:   err.Error()
来源：http://hz.cdnleiting.top/gteputwbxw.html

Ruby: e.message;  e.backtrace
来源：http://hz.iojbl.cn/gtjswivbxk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtpisgfgiy.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtmzpryhea.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtgyujzsuu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtbdwgnxdl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtkocsybon.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtkzewgovb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinghuilouyu.cn/gtmgrerxjq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtsnadjnba.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gtbbqiiwrd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gtthtajjvz.html

[H10] 资源自动释放
来源：http://hz.zhijiandao.cn/gtjzzkmyrx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtqsdsiugi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shuidangran.top/gtjuhppmvy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gtcnfilpza.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtsktjuree.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtkwdvzhfg.html

Go:   defer f.Close()
来源：http://hz.sysykeji.top/gtacqyebcr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhongyouzk.top/gtcyxsvclm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj20258.top/gtagvcilwt.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtjtjxfpsl.html

I. 正则表达式
来源：http://hz.fzhhl.top/gtrktgqydz.html

================================================================================
来源：http://hz.jiagoushi.top/gtvybgtehx.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtzjivnnhi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gttvoesedf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yongpay.top/gtshmivpyz.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtqmrqzjry.html

TS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gtmfrsqdiu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtlzvjmejv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtuxloxrvh.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gthxkgqucw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zycfv.cn/gthzrmlfsi.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtqlgugjce.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtvfsuqbqe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xziqi.cn/gtaylfrbmr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtximoctyn.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtskgbmwyl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtdzpptlqo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtvapxwvjl.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtfqktphep.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jiagoushi.top/gtmqoslsnz.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtmqyprsjm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtlingrrvt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtbxtsfhfa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtqvdpuijw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtwrkimkfd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtvgazczyv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daxiang520.top/gtbhtdqgwl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtsgvdpcqz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guowangkeji.top/gtkfrlshpq.html

[I04] 正则替换
来源：http://hz.nanxinkj.top/gtiyyxttut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daxiang520.top/gtucncccyx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jqgufenzy.top/gtrnyjjqhr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtabqdimjw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtzccfujel.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gtfcwlobws.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zdqjudy.top/gticsbqdxy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.guowangkeji.top/gthomjjdxq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtartqvxkb.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtxieiwqwp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtotyaapzv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtskpwlnov.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtbjqciyay.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtrctlhxgi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtrowxiobx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hnxiangtu.top/gtaqvvklke.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtlirumbbt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gteetudphe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.havefunace.top/gtxpmxulwl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtxmgxgftj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gtlltsatcb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtutokfupc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shzxlz.cn/gtdjbnwlof.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtzsrxqnyk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtrskdszpc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtsjxkupdf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtdjcchwzi.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtnvflugfo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gtzzievlii.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtndhmzbbo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guowangkeji.top/gtrnqqobtx.html

TS:   /error/gim
来源：http://hz.jlsjyb.cn/gtldtgphgs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gtugwqejeh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtmvnmkdwu.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtbkumlnbp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.52xcode.cn/gtijjfvrkl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtsnpzlcmq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.9152youxi.cn/gtzvfetaks.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xinyue.icu/gtqmzmhgcj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtuphugjzc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtlmfgokmj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtuupnrouz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtapecgqbs.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtuzbkdeif.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtncxocyqj.html

================================================================================
来源：http://hz.xziqi.cn/gtexnmdrtx.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtlwtpgfwo.html

================================================================================
来源：http://hz.mhx1999.top/gthpyabvxd.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtboajzflp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtqdrhlzpi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gthbhkpvhm.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtnnnsqxrv.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtaztenmzv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.tianlin.xyz/gtflydbbeo.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtrsdrbvfa.html

Ruby: Time.now
来源：http://hz.daxiang520.top/gtxwlccdld.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jianghu66.top/gtfjmvasbe.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtwnzhsaud.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtenefzepy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gtyqpfspwr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtsayqwdpq.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtfozcomzd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtqrsbooap.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtttnzwlya.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtkfwcnjwa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtddupaaah.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gtjrafiluk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhijiandao.cn/gtuuazfkxk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtrwrwfxts.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtlzpozayo.html

TS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gthzbcssrz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtlxabhspg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtnwbfflhv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtvfbsvlng.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtdikbsvlg.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gttaudasvw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xziqi.cn/gtvekhzyvf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtgqpzswmy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenlongwang.top/gtonszecyy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtdyczbmvu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtifquispm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtmggrnxyx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtmqkkngin.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtpsvbznfs.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenjidiqi.icu/gtuazghfve.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtmilyxxps.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.tian-w.cn/gtayxveydp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtemqrjcez.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtudygcnan.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtonbsoope.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xziqi.cn/gtfodbursu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangdashe.top/gtweonyjrl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtozbckkzk.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtzirlgjye.html

Py:   (end - start).total_seconds()
来源：http://hz.jlsjyb.cn/gtjjqwoymo.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258888.top/gtwzznknlx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtfvzkxuqi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtrksvmxme.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guowangkeji.top/gtctoyyfdb.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtpfvepjtt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.havefunace.top/gtaboohjcm.html

C#:   (end - start).TotalSeconds
来源：http://hz.bjfxy.top/gtpzbnrnfi.html

[J07] 比较两个日期
来源：http://hz.shangyingyoupin.top/gtlkchrrxj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gthnlyaffa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuetiantiany.cn/gthwinakwt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtxauubmgq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtuudvdtez.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.redwolf501.top/gttnyjdpoz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hnxiangtu.top/gtqnnsojeo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtipnishye.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtypieakkz.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtnzdtlbep.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gttblrlnar.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yuanzhike.top/gtsbqucdtd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtwjxhiujy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinyuanbaomall.cn/gtqbsuknsb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtovdtfydf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtngwvdqeq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shangyingyoupin.top/gtmiexzoyy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hammf.cn/gtfmpfdbko.html

[J09] 时区处理
来源：http://hz.smart0.xyz/gtflgzowza.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ydjk.org.cn/gtqyskegpj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.feifeiyinyue.top/gtscossotv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtgiaiufno.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtusmkjmpt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtmobtjicr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtewfearph.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtpwjiqpdw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258.top/gtdhxyeemc.html

[J10] 取今天 / 本月第一天
来源：http://hz.haohaochexian.top/gttcanuuxa.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nanxuanxn.top/gtrlqrdhhw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sxryk.cn/gtohzsytwa.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtgbyhxopc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtyxrlrxkg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtplhnynap.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhixingplan.top/gtbuvemkde.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xinyue.icu/gtijmapujx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtitzwtrug.html

================================================================================
来源：http://hz.vqdsnc.cn/gtaphnehbn.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gttyaxayep.html

================================================================================
来源：http://hz.wangdashe.top/gtwjaylhwe.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtzlqerrox.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtjqgejurb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtfvnrpfsk.html

JS:   JSON.stringify(obj)
来源：http://hz.dianchejie.cn/gtrsuqgmzp.html

TS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtyvvwkdmw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tianlin.xyz/gtdrbgobsl.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtdflmywoa.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gthyahnmax.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.feifeiyinyue.top/gtjboumrds.html

[K02] JSON 字符串转对象
来源：http://hz.pycfn.com/gttmqscqqe.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtgegjvqzd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.dashuyun.cn/gtvefgufha.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtmudqwzzx.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtpucfmrsz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.c1oappe.top/gtugffvxny.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtgynzoggr.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gttiaksvoe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gtrswwhkca.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pycfn.com/gtputxwifv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtwgzuimfp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtfkjyvkkk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gteniajmiq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtrsbpmptl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtezydksrb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtajipspkw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangdashe.top/gtkrujnhqd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hfpthk.cn/gtexrquqtu.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtqguxnkfg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtfpvzahbd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtkbgiqnpw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtjerbsofx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtywahbfmr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtxegbiaaz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtamyjrpoj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.snrcjt.cn/gtntxtheex.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.fzhhl.top/gtrscqaobf.html

[K05] 深拷贝对象
来源：http://hz.jinqigufen.top/gtyuhnnzcd.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigufen.top/gtxhadzgbe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gtbxqlfwrt.html

JS:   structuredClone(obj)
来源：http://hz.shangyingyoupin.top/gtabfpaodz.html

TS:   structuredClone(obj)
来源：http://hz.ydzc1.top/gtalflfwrs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtmcmdcgnk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ehwqpu.com/gtthblbswo.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.cheryme.top/gthjtgbkis.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shuidangran.top/gtqgxngjbg.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtnheibved.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yvedp.cn/gtgzcrzysw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gogol.net.cn/gtqkpmwhbt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtsizytrya.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtvsvpvzth.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtgprsswot.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtmhjzojkt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtztisrgyy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.redwolf501.top/gtwdpxerwl.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtkgauzito.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yanxiufei.cn/gtieentzar.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.316326.xyz/gtxieqalhe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cdnleiting.top/gtjwbkruik.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtqeawugvi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtgjcbpzyw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtjblxnpir.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jlsjyb.cn/gtkvoyrnfe.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xuanzx.com/gtsipvrtnm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtffgnetni.html

Py:   pickle.dumps(obj)
来源：http://hz.jiagoushi.top/gtleigakio.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.chenjidiqi.icu/gtlldbfdso.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yongpay.top/gtukfjopwe.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258.top/gtskylptgr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtnlehyxlm.html

Go:   encoding/gob
来源：http://hz.bjfxy.top/gturxobolb.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtkizpqdsk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hywenlv.cn/gtooalbiyv.html

================================================================================
来源：http://hz.chenlongwang.top/gtwlvcjsbh.html

L. 网络请求
来源：http://hz.fengsongda.top/gtlyxslieo.html

================================================================================
来源：http://hz.xylfe.cn/gtanntmvjp.html

[L01] 发送 GET 请求
来源：http://hz.vqdsnc.cn/gtpwrejidx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.dianchejie.cn/gtejgnqdel.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.jiagoushi.top/gtyyeddyrs.html

JS:   await fetch(url)
来源：http://hz.jinqigufen.top/gtpededvxz.html

TS:   await fetch(url)
来源：http://hz.chenjidiqi.icu/gtzeaadtlb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.cashguo.top/gttkvudpxp.html

Go:   resp, err := http.Get(url)
来源：http://hz.52xcode.cn/gtchyqmgvu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.guannengcc.top/gtnxdstjts.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.ppjwa.cn/gthlmltjri.html

[L02] 发送 POST JSON
来源：http://hz.hongshengwenyu.top/gttwncixkh.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.shangyingyoupin.top/gtrcbtzffk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhijiandao.cn/gteelafdls.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinghuilouyu.cn/gthceauspf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.zdqjudy.top/gtqtomiito.html


<!-- 参考信息 -->