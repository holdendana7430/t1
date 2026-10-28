代发 wailian999

[H07] 断言
来源：http://hz.ywan-chungtsiang.top/gtliwnnkpx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gtuedhoxwh.html

PHP:  assert($x > 0);
来源：http://hz.kuanghao11.cn/gtryfyrgsd.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gttnaumvbm.html

TS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtdecpsnlg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.316326.xyz/gtrsqmjrzn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.sxryk.cn/gtwhoviypr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtbcpqblkg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ywan-chungtsiang.top/gtenqsfhgm.html

[H08] 获取错误信息与堆栈
来源：http://hz.meibo888.top/gtbwquoozh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gturwhhkgm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhixingplan.top/gtnhcgabcn.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gttburylqk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xingfuxueyuan.xyz/gtghimjcpl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtrkukpkux.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtosxpreiz.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gttvlcruwj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtcaxbufkb.html

[H09] 带错误码的异常
来源：http://hz.xziqi.cn/gtavdmjvmd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zycfv.cn/gtqufcgydp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtqpwvxelh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuanzx.com/gtctfejtgc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtfckobdaz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtmipvyrsr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtbicbyctf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtwtdnxkov.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtlxpwxvtm.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtjgfsjdlm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gttlahhlhx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jqgfzy.top/gtoahbdylg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtifvbezrj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtenafwlqc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ybcxt.top/gtnfyjwxuy.html

Go:   defer f.Close()
来源：http://hz.yueranfly.top/gtfkwurxse.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.kuanghao11.cn/gteaqphhax.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shangyingyoupin.top/gtcfifkpmo.html

================================================================================
来源：http://hz.zhixingplan.top/gtwepifexy.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtpmncpsss.html

================================================================================
来源：http://hz.yuanzhike.top/gtyxfmghke.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtjwkfijva.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtfniogbld.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fengsongda.top/gtbskldmrf.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtxakpccjg.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gtotvxggiu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gthqmitsyp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtjkelpbsa.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtrfvimkqq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.meibo888.top/gtngjryvfo.html

[I02] 提取所有匹配
来源：http://hz.xuetiantiany.cn/gtklkhqmpb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtyzwjzuic.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtpusowunh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtiblsfais.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gtwwjilzgc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtlalkrosn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gtsnqohjhx.html

Ruby: s.scan(/\d+/)
来源：http://hz.haohaochexian.top/gtmvcamtpg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxuanxn.top/gtbsxlfumu.html

[I03] 提取捕获分组
来源：http://hz.kuanghao11.cn/gttqubhyzc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtxzsdgnyq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtmqculaxn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gtcqdsuvmn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtkdtopxib.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtgvmnsrxw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtdjickrpz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.c1oappe.top/gtrmwdjcyh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yanxiufei.cn/gtyxkwglnd.html

[I04] 正则替换
来源：http://hz.fengsongda.top/gtbwiwasra.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtdrobmvvw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtvfpwqzyl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gttqpgauta.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtqebrwzyy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gtgepdvqdm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xziqi.cn/gtkywethle.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhixingplan.top/gtfqdmsfac.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtepxqlybo.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtstdtbccj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtclrmhgri.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guannengcc.top/gtlejqfesv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xylfe.cn/gtxiumlrpp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gteiofbhwb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gthntsxeql.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fengsongda.top/gtfdsznowj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gttmdhvghk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yvedp.cn/gtuhyptpvq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangdashe.top/gtplzuwumq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtrxaatcgj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dashuyun.cn/gtrojdjlrn.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtovwnizfj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtlumloswi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtffrhgpvi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cdnleiting.top/gtcermzsys.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtpxjatqjf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtyblssdup.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtiwzjnuij.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gtgfzdbexs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtagswhrhr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gtocqtsyjo.html

TS:   /error/gim
来源：http://hz.hywenlv.cn/gtrfhwxivv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gtxfkxdeom.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtxhgzyvbz.html

Ruby: s.scan(/error/i)
来源：http://hz.zhongyouzk.top/gtrmkpqazn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtxzqlrurz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.daria6918.cn/gtampzlntf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtdggsqyst.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtraazmzow.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtjsqhayis.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtgpnowlui.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258.top/gtincwryrn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtqhannpck.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtpbqpyhow.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fzhhl.top/gtjgpiyfji.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtcdnqnkon.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtsfnyfjxg.html

================================================================================
来源：http://hz.zycfv.cn/gtsactqcnv.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtlpebjgiv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gttlwawttk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtzaroygrz.html

JS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtxoswccvj.html

TS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtsyqszvng.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtkcktckuo.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtwgtyksjz.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtnwulwpij.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgfzy.top/gtvbiwddvb.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtsrtllzxv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gthxocpvvj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtdxzksqba.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gthahdsjgd.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gtpvebzxbx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zycfv.cn/gtafenlpap.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gteseupyni.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtfgunqijj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guowangkeji.top/gtwkpznarq.html

[J03] 字符串解析为日期
来源：http://hz.ivvv.top/gtxsdgeciv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtgfufkaxs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xziqi.cn/gtchfmlabs.html

JS:   new Date("2024-01-02")
来源：http://hz.tanke756.top/gtinettifr.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtjuccwtgp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtemxwbyvv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtkxjddflf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtnuvxedpb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cheryme.top/gtdcflxvyr.html

[J04] 时间戳与日期互转
来源：http://hz.andypj.xyz/gtdwmlcpjt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtadczptdc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtmcdgajfo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtkqcvqnoq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hfpthk.cn/gtvcpycrsi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hnqzz.top/gtmgsmkcjd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtsarcpybj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtirphqufr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtlwknojaf.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gtnxpfkdtk.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtrgokleur.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gttdjbchho.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtbgbiuboi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtygomwcoy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gthqohxfre.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.dashuyun.cn/gtaiaqyfqx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtlktziobz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtxgygfhed.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtjbxmhzeu.html

Py:   (end - start).total_seconds()
来源：http://hz.zycfv.cn/gtqzppjdzp.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gttwokrlea.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gtyczfsvut.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtkhxxotnl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtjngieyyn.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtxqlctqck.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gttkbaqetz.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtlqinvnib.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtmhdpwycg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtizjyjmgj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtgmlbjtpg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtslxexxbr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtchqmhqrc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.quarkkingdee.top/gthbhhvsie.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtbeqdnvad.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxuanxn.top/gtrhyseigt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtvcsbybww.html

[J08] 提取年月日与星期
来源：http://hz.hongshengwenyu.top/gtsafuuclv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtrkaiqkix.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenzaomai.com/gttsjkktrh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.vqdsnc.cn/gtkueiioui.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gtuiellosf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtxkxkktrv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtajcbwibi.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtnytavkpi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.9152youxi.cn/gtdunsnrpb.html

[J09] 时区处理
来源：http://hz.tanke756.top/gtwmbahhdm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtbescuvss.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.kuanghao11.cn/gtklcajtqj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtxxoaomkq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtdrcssrbq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtqeetcswb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ydzc1.top/gtmooiqjrc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtymmpqjbu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtnxejmwkx.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtvmyxavgx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtltsgdees.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtsmxvdpxy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhoulong.xyz/gtztmtjqki.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtpxqpawyi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gttbhzsukd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gteopnhemc.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtumlswclx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtrqkhwbir.html

================================================================================
来源：http://hz.zhengqikj.top/gtdneammkv.html

K. JSON 与序列化
来源：http://hz.haohaochexian.top/gtmctyadyq.html

================================================================================
来源：http://hz.316326.xyz/gtlnoaihkw.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtezsetqpq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtpwqspljz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.9152youxi.cn/gtjvloghtl.html

JS:   JSON.stringify(obj)
来源：http://hz.gogol.net.cn/gtgreeeyod.html

TS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtiwyzddur.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtehrvksfe.html

Go:   json.Marshal(obj)
来源：http://hz.yuxming.cn/gtfkuorzrv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtnhwfzrmm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtxwtewaky.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gterzwikpn.html

Py:   json.loads(s)
来源：http://hz.shzxlz.cn/gtzdfwennc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xinyue.icu/gteyiahmzg.html

JS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtunfvymzl.html

TS:   JSON.parse(s)
来源：http://hz.bjfxy.top/gtrlvanqjl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gteubdfyvh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtlgtjqxnb.html

Ruby: JSON.parse(s)
来源：http://hz.yuxming.cn/gteciwkkrc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhaomingkeji.xyz/gtaicglujg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hysaishi.cn/gtqegjbrir.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.redwolf501.top/gtskctxfnx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtotfsmski.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gttmtnxboy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtpdgboqls.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtbwshfbvx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gttcixodai.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.fengsongda.top/gttoteaonh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gtrxenrpyf.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtnmoyzaeo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xylfe.cn/gtpyhigpkw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtmyscaawx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtgyhbvkno.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.kuanghao11.cn/gtytcjdcmu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtibyodpcp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jqgufenzy.top/gtxjqkvcha.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cucudq.cn/gtqslmlcui.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtbjzaonhh.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtibtlpxdj.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtwcshzxbf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtusseebck.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtlgcuhzio.html

TS:   structuredClone(obj)
来源：http://hz.chenjidiqi.icu/gtuycvxiiy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtjxesdehn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xuanzx.com/gtbedjucey.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xinyue.icu/gtspbveqwg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gtornbvxrj.html

[K06] 解析 URL 查询串
来源：http://hz.fzhhl.top/gttsglolcm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtgyhnlggf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.daxiang520.top/gtkkbmoupk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtqorvgqmp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtvaiwpsvu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnxiangtu.top/gttawsfrgj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cdnleiting.top/gtgnozijqf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtxrlhwpqv.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dianchejie.cn/gtykrklxsq.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtjsqywynh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangshuangyany.cn/gtxhglimep.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ybcxt.top/gtjaancmqo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtetxzoxyt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuetiantiany.cn/gtkknbsqzk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtnxykbwht.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.52xcode.cn/gtddwuuppm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtrlpxihec.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gogol.net.cn/gtlbuzksds.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.kuanghao11.cn/gtdaapnhve.html

Py:   pickle.dumps(obj)
来源：http://hz.hnxiangtu.top/gtebluagxw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yonumen.top/gtfyzzwzxc.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtkwahtkml.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xuetiantiany.cn/gteqnjfoax.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtpgonazgl.html

Go:   encoding/gob
来源：http://hz.aibaodan.cn/gtnzqcohnl.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuanzhike.top/gtnebtwxeu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.fengsongda.top/gtjxptvovz.html

================================================================================
来源：http://hz.gogol.net.cn/gtzjdhmynd.html

L. 网络请求
来源：http://hz.yuxming.cn/gtxporqvco.html

================================================================================
来源：http://hz.gogol.net.cn/gtrxwrtybo.html

[L01] 发送 GET 请求
来源：http://hz.316326.xyz/gtoonachyb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.0kj1m.cn/gtlynpinqy.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.daxiang520.top/gtzludhgwc.html

JS:   await fetch(url)
来源：http://hz.jianghu66.top/gtghubsyju.html

TS:   await fetch(url)
来源：http://hz.yj20258888.top/gtzjwgoimu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuxming.cn/gtttqjshyl.html

Go:   resp, err := http.Get(url)
来源：http://hz.birdmap.top/gtpcxdkzfj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.zhiwuduotai.top/gtewlaibdv.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.tian-w.cn/gthtbefwsb.html

[L02] 发送 POST JSON
来源：http://hz.sysykeji.top/gtwvdcteyg.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.jlsjyb.cn/gtsgvwehyv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.yuanzhike.top/gthatfxzey.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jiagoushi.top/gtposkjpvn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yongpay.top/gtreyuxmij.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.tanke756.top/gtydhofqdj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.9152youxi.cn/gtlooeatua.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.havefunace.top/gtkkifezgh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.vqdsnc.cn/gtfwgdhahj.html


<!-- 参考信息 -->