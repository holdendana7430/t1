代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.hnxiangtu.top/gtkiuvpwax.html

C#:   class MyException : Exception {}
来源：http://hz.havefunace.top/gtqvxthbmi.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gtnhgvuxqu.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtsdnetjgn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gthtireymu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj202588.top/gtmegzudst.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtwizdemzp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.smart0.xyz/gtoytwyhrb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtfagssrmb.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtzvmwicow.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guannengcc.top/gtzxdedzoy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tanke756.top/gtsprtbtxf.html

Py:   value = d.get("k") or default
来源：http://hz.sweek.top/gtcpmeeldg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gtsaduaweg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtijldjkmq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gttqmyazzm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jqgfzy.top/gtatwxnkco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtkvecxizi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.52xcode.cn/gtznssrgva.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtrlxueavi.html

[H07] 断言
来源：http://hz.ydzc1.top/gthdoqaiie.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenjidiqi.icu/gtbkcgsqbk.html

PHP:  assert($x > 0);
来源：http://hz.vqdsnc.cn/gtxlhsasxs.html

JS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtqciseajx.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtpsfvjbcx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtxwmewyci.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gtaddilgbn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sysykeji.top/gtzikhjiwy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtqicnghki.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtpehonfaw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hywenlv.cn/gtvvapufzx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtmnggbrod.html

JS:   e.message;  e.stack
来源：http://hz.svipenyu.cn/gtvgslrotq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shzxlz.cn/gtpixcratg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtmddjfvdh.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtlhpevmny.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtkvshebzp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.pycfn.com/gtaxaayzly.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtwvxdevtg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtlercebed.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtanvuuwwv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtkkjjqycj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daria6918.cn/gtegllobbk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gtqmcobjcj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgfzy.top/gtwktzuebk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gttdzaitzp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtysonzwip.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtoqfxbzpt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pengpengdd.cyou/gthpdtiptl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtekezrmbu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtnzysczvt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hongshengwenyu.top/gtjscpwguq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.c1oappe.top/gtdyofppvl.html

Go:   defer f.Close()
来源：http://hz.yj202588.top/gtevsxgxhe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtmbuyxtpn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zycfv.cn/gtqkyebnwf.html

================================================================================
来源：http://hz.cdnleiting.top/gtwqhsusbi.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtjqbjbtpc.html

================================================================================
来源：http://hz.cashguo.top/gtzktlftwx.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtnydoxjbj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gtdfcccfbk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtrbfgkyyz.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtrplziktj.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtecrdtinr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtbvmuadwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gtbsbzuabu.html

Ruby: s.match?(/\d+/)
来源：http://hz.andypj.xyz/gtziaylqkb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.birdmap.top/gtdnyhnvct.html

[I02] 提取所有匹配
来源：http://hz.hnqzz.top/gtjobxlwyq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gtcyecbgpk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtdgrveudh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtrycspxug.html

TS:   s.match(/\d+/g)
来源：http://hz.c1oappe.top/gtqnnsrxga.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtdrcnfaym.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtvqgqcoza.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtkdubgksd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aizwys.cn/gtogxmbvqo.html

[I03] 提取捕获分组
来源：http://hz.chenzaomai.com/gtvltjdudg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtqenavrgh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhongyouzk.top/gtczdlkisn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtbvoqcinw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtlxbjrvfy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ivvv.top/gtniimpxfy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtbeyinvod.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtoqkvrqzn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhaomingkeji.xyz/gtholiidat.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtjtpwvjjc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hongshengwenyu.top/gtrmxdhskx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtpzkkfxcn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtejiipzft.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtxtgyplxd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jlsjyb.cn/gtekzidsky.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sxryk.cn/gtxhafutlx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtnnmnfwkg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtyemqmolt.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtmtorfixr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtcsmxsjba.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtalabszuz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtpvvaflng.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtigjwtlpi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtrrwoeuvr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.havefunace.top/gtgzpwilst.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtqlgzjrdl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shzxlz.cn/gthhdgxokr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.iojbl.cn/gtcyduqfye.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtmdyucnhp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtnxkxvmqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yueranfly.top/gtljqbcyew.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtwhzbpxvl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gteymzqyve.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtfaajbgxl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtoaocttlf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtoosflsmc.html

[I07] 忽略大小写与多行模式
来源：http://hz.daria6918.cn/gtbtqdyndo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtchgwsedh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtfrklwqug.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtulshkglj.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtodgopdab.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtihnvefes.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenzaomai.com/gtsgwkplju.html

Ruby: s.scan(/error/i)
来源：http://hz.dianchejie.cn/gthtrrmtox.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zycfv.cn/gtkdrsjyxk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtzzjmqwrs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuanzx.com/gtsvnvtsqp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtvonbzprm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtpwlbsufh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtasyooyop.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtviaelyjs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtvvyggbzf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zdqjudy.top/gtilusneww.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yonumen.top/gtvqzhmfud.html

================================================================================
来源：http://hz.zycfv.cn/gtrwqmxgdr.html

J. 日期与时间
来源：http://hz.yuxming.cn/gthrwwesex.html

================================================================================
来源：http://hz.9152youxi.cn/gtgismdnlj.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtptvdjjwa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtxjqdhsdy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtigrjlsoy.html

JS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtnochmvbz.html

TS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtfsseqpue.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dianchejie.cn/gtufabhrkr.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtpkfgrzhv.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtjqbzkomu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pengpengdd.cyou/gtztbfcjdo.html

[J02] 格式化输出
来源：http://hz.52xcode.cn/gtvnbkfbfl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtvveixhhu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gzhubu.top/gtrnewlgda.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shzxlz.cn/gtcrpilwlp.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtysenlbkg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cheryme.top/gtnoqxisqc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtrtvndfmv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhixingplan.top/gterlhkzlv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhaomingkeji.xyz/gtztozaubc.html

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtmtnzfqeo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtlyeuzaxj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.c1oappe.top/gtizkywtsg.html

JS:   new Date("2024-01-02")
来源：http://hz.jiagoushi.top/gtkzcutskd.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtvibzvpke.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtoeecjpkb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtzoazexur.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yonumen.top/gtegblndqd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gttlqnndvh.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtayipdaxx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hfpthk.cn/gtxlssipvt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtpibehtkm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtpamwqwek.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtnzpmrwfo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.aizwys.cn/gtjolziuky.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.c1oappe.top/gtucvqfzqg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhijiandao.cn/gtytdlnxvc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenjidiqi.icu/gtluzcgzyn.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtmcehwdyu.html

Py:   now + timedelta(days=7)
来源：http://hz.jinghuilouyu.cn/gtagtnxgrp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtxxjeurii.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtuitqwhqt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aizwys.cn/gtkftovtjc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtkxihffcd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.c1oappe.top/gtknekrsbb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtgnlafzsz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hysaishi.cn/gtwfdzvrpu.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtipxiobft.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtguzdpgiu.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtxwlgctwv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.9152youxi.cn/gtdqacsjsp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtjflttdzu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtccbywbjn.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gtbibltpfg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtsgrmzmms.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtpmbcxolq.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtxhyoatvw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtovflzuia.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtmnbyyvsx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtqvotnahk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtuhegsjsc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtguzhwrso.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtzipjulsk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtspkmaeat.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtkvtyvjrw.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtcxvfdmmv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sweek.top/gtsetggavw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gtibjbuocf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gtpimdhrch.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.dianchejie.cn/gtmprqbmdu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtrfvxjyfw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shuidangran.top/gtksjhornm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtpnsqatnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtsfctiqyl.html

[J09] 时区处理
来源：http://hz.quarkkingdee.top/gtovniqnms.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhoulong.xyz/gtiuwdcogd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtjsqnbgwt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtikqstwgh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zdqjudy.top/gtarpnkxam.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtkbzgrumw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtkribxcol.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gttexehmsg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtelgocasm.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtifcufmut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinyuanbaomall.cn/gtbdtlziox.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jyoumei.cn/gtdfpbhxvk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pengpengdd.cyou/gtwbiydrxy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtsmsdptdm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtefkfnjrq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtpcekvnuu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ehwqpu.com/gtinwzityt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtfogmijei.html

================================================================================
来源：http://hz.quarkkingdee.top/gtkvpltfxi.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gthotrcern.html

================================================================================
来源：http://hz.zhengqikj.top/gtsdxghljy.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtuanyqwyc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtnnplmnny.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtorafciou.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtvlezdcsx.html

TS:   JSON.stringify(obj)
来源：http://hz.sweek.top/gtsgqsxeos.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgfzy.top/gtucfddgoz.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtvabwxfcj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.mhx1999.top/gtatyztocc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinyuanbaomall.cn/gtiyzdopjh.html

[K02] JSON 字符串转对象
来源：http://hz.daxiang520.top/gtakphwqwf.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtfghpcfaq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtksitjqta.html

JS:   JSON.parse(s)
来源：http://hz.hysaishi.cn/gtzysbbecj.html

TS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtpybpjtxn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtcpqhqyqi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.wangdashe.top/gtzjxoeraf.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtbhrthudd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtswqvvilu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtzsafdviz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtzlyhekfl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.snrcjt.cn/gtlrzzzyoy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtvwcfescj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenzaomai.com/gtthvizkrn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tanke756.top/gthkipnyeg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yvedp.cn/gtoagmpwbj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gtyrdhjeqr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.ppjwa.cn/gtartkplxu.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtgmbkzlsc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ivvv.top/gtfjqgjdrt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jqgufenzy.top/gtmsrkixds.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtwhhmxgfr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.mhx1999.top/gtvtwsujes.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhongyouzk.top/gtmkqhgyef.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.tian-w.cn/gtvcwsqymt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sxryk.cn/gtsfbswhat.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtqfowmlqj.html

[K05] 深拷贝对象
来源：http://hz.smart0.xyz/gtmtbbfnux.html

Py:   copy.deepcopy(obj)
来源：http://hz.fengsongda.top/gtcvctsbuu.html

PHP:  unserialize(serialize($obj));
来源：http://hz.meibo888.top/gtnciualmg.html

JS:   structuredClone(obj)
来源：http://hz.zycfv.cn/gtppbemuqv.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtkxfavrde.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtsxatqjww.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtduyuiyfc.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtdrmlnwhh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.chenlongwang.top/gtlpzysevc.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtexrjxxbl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.quarkkingdee.top/gtvilyflkd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtbjqwpnfp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtmzomamos.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pycfn.com/gtnuazkelh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gthxwizied.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhengqikj.top/gtopmjmqxm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jqgufenzy.top/gttuyyeuia.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtmnbbtwyk.html

[K07] 进制转换
来源：http://hz.nanxuanxn.top/gtntpcbsst.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.birdmap.top/gtxkfxregi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yj20258888.top/gtmvsbmhno.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtlcfiqcgp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtppidnhsh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtmmotdzst.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtxuyfoowz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cucudq.cn/gtganakjck.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenzaomai.com/gttixtdujx.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gtojsysmvh.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtbzvtedos.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jinyuanbaomall.cn/gtirskizme.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ywan-chungtsiang.top/gtjenjigxj.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtqovhchpr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtdobbzvgi.html

Go:   encoding/gob
来源：http://hz.chenzaomai.com/gtvxpylfhk.html

Ruby: Marshal.dump(obj)
来源：http://hz.jiagoushi.top/gttuzorvxt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.hnxiangtu.top/gtmzqmmzcm.html

================================================================================
来源：http://hz.gogol.net.cn/gtdfovidfb.html


<!-- 参考信息 -->