代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.0kj1m.cn/gtvgiabwgj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtnkiemmtv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtpeadxvyx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhixingplan.top/gtcvhzwodd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtwkcfprzp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shangyingyoupin.top/gtaibvgifo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cdnleiting.top/gtzeaqodan.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258888.top/gtsejwvrpw.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gtdfrodnmt.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtgymbefbk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtwzutjdfa.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtcputofwb.html

TS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtnljnaftl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtdpdaedpl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtwyslksqk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yj20258.top/gtsoahjnik.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtpmclyrwk.html

[H04] 自定义异常类型
来源：http://hz.yuxming.cn/gtilxpntdh.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtifdrzfyp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtixrprhvw.html

JS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtarznitzf.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtxiofzdoa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtujthruja.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtwdgsswsu.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtablbjjma.html

C#:   class MyException : Exception {}
来源：http://hz.sysykeji.top/gtujffabtx.html

[H05] 捕获特定类型
来源：http://hz.chenjidiqi.icu/gtknkjunxv.html

Py:   except ValueError as e:
来源：http://hz.tianlin.xyz/gtmgqgpwuc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtqzxvofhy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.mhx1999.top/gtmjhntnug.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtabkyqbuz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtnbwowltr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtulmpcazw.html

Ruby: rescue ArgumentError => e
来源：http://hz.yanxiufei.cn/gtoinzlryn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenlongwang.top/gtfldpqhhl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtcuqffsej.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtzvsohgyn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtbtqilcdj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtqgpflxkr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gtwxrxhdew.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuetiantiany.cn/gttmlkhoqt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.redwolf501.top/gtgtnfaqui.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtvdgroflf.html

C#:   obj?.A?.B ?? default
来源：http://hz.yangfankeji.com/gtelqzzoir.html

[H07] 断言
来源：http://hz.52xcode.cn/gtlmjudzls.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gttpflouah.html

PHP:  assert($x > 0);
来源：http://hz.cqqwz.cn/gtiddjglah.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtcufttogn.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtsgdmwpst.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtdgdpmzzp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtjmzkvhsd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sufxvd.cn/gtvniayknl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtgofqryvx.html

[H08] 获取错误信息与堆栈
来源：http://hz.iojbl.cn/gttqywmalm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gtxirefjqi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tian-w.cn/gtgnmfqpsg.html

JS:   e.message;  e.stack
来源：http://hz.dashuyun.cn/gtosphpfft.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhongyouzk.top/gtadxuunpu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shangyingyoupin.top/gtsxzsyjhc.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtivhoudkq.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtzdgygxdv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtjikxpsfi.html

[H09] 带错误码的异常
来源：http://hz.c1oappe.top/gtadvnijgs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yangfankeji.com/gtvbtqbtib.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtvifkbnhs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gtngskjdnc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtrbwsodag.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.52xcode.cn/gtemoicucr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtjuqclfnc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtjxwrkqwd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yongpay.top/gtyfowbrez.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtgnzxfccn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtidoiqduu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtpmyhqkuq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtvpvmsmze.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtdzmnrihw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shzxlz.cn/gtgffceueu.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtddbydhlc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tianlin.xyz/gtkobhckey.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtqqumgurn.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtntzowlzc.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtzeylgjpn.html

================================================================================
来源：http://hz.aizwys.cn/gtxsrzzrfk.html

[I01] 判断是否匹配
来源：http://hz.ybcxt.top/gtpwsxpirs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtpotfccun.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtafwstopi.html

JS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtdscflikt.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtuxwrebcs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtjqxbgndf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtwcjqsuzf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtqepdpgfp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtbzwtnjfd.html

[I02] 提取所有匹配
来源：http://hz.yj20258.top/gtymqqypdv.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xylfe.cn/gtrkwbhlgo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuanzhike.top/gteydqfbgq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtvbdqelpu.html

TS:   s.match(/\d+/g)
来源：http://hz.cdnleiting.top/gtbhjyzuxg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtgtymiyyl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.52xcode.cn/gtxpozdkbk.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gthudrloxp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtbecschic.html

[I03] 提取捕获分组
来源：http://hz.daxiang520.top/gtmrrrmbej.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtazuoeyeo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.svipenyu.cn/gtrylzdbje.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.316326.xyz/gtskeaefug.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxuanxn.top/gtvsmuqyug.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtlezyuybb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtvbhzakrm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sweek.top/gtywlhlhag.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtyfznnwgj.html

[I04] 正则替换
来源：http://hz.shanyushiyangtech.top/gtwnsutjqy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtembcjfht.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtzisbjekm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtkjqalknx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtqgfuvfsy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtjtqqjsea.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gogol.net.cn/gtbwyycute.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtorfeycej.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jianghu66.top/gtmijsyiai.html

[I05] 按正则拆分
来源：http://hz.zhoulong.xyz/gtpomecdna.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtcidtifkf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daria6918.cn/gtprltterh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtwhbpybcm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtspbjmsvn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ywan-chungtsiang.top/gtewlcgbcv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ehwqpu.com/gtswdckkle.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtxtqdrgds.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtssalfyxm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yongpay.top/gtrhfqktzh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hysaishi.cn/gtxcldvywc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gtvazkublf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtekeywlje.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yvedp.cn/gtmxrlzdfi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtmbeuklqf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtqwekupqp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtcuucurkd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtmgnvkulw.html

[I07] 忽略大小写与多行模式
来源：http://hz.jianghu66.top/gtonyhsfuo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtxmfbplfs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtzvgrtwem.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtibvahlvv.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtvbmrcjya.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yueranfly.top/gtiegejlzr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtweawgdqv.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtpnsipfkw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtuijbxetj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtbalfzkfa.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gtpngzqklu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtnjhwxwsv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtsjyehkje.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtuhysiwod.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtnljhlcaz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtxsxjmyyi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtlsyiaewj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtpiljjlow.html

================================================================================
来源：http://hz.yj20258.top/gthzwalxdd.html

J. 日期与时间
来源：http://hz.ybcxt.top/gtstcfowur.html

================================================================================
来源：http://hz.gaohongyu789.top/gtoasozwko.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gthitmoyqj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.haohaochexian.top/gtwdtmnama.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtcfqkuorr.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtbdhvrvfj.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gttfnampmh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.haohaochexian.top/gtjvzlmhdo.html

Go:   time.Now()
来源：http://hz.yj202588.top/gtdgqkwxwx.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtkrvmtzle.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtayjtqviq.html

[J02] 格式化输出
来源：http://hz.jinghuilouyu.cn/gtywqwqrdn.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ppjwa.cn/gtjpqylcfe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtygyctfih.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hongshengwenyu.top/gtbtinvrat.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gterlysyki.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtxqzfpruw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shuidangran.top/gtaejttyeu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtceycmaou.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.svipenyu.cn/gtrllfpkuk.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtiazcpvdv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtecwbcmef.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtthmfmusq.html

JS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtodlaxszy.html

TS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtazlqucnd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtenqotirt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ehwqpu.com/gtmdfazhlh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtylxlllyb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtgspishew.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtxfemtfsx.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tanke756.top/gtcigywbdm.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sysykeji.top/gtyikjrehq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gticgbrpkq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtzxljubue.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gteylaghkc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cheryme.top/gtuocztknt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtdvojnvsz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtwojbfniq.html

[J05] 时间加减（加 7 天）
来源：http://hz.xinyue.icu/gtrsjncmqb.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtojhonjkw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ybcxt.top/gtvzgqxjxn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtahwibeoy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtlpczndoq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jqgfzy.top/gtixhmjbqj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sxryk.cn/gtbnorrrga.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtmpdkplrh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zdqjudy.top/gtkltorgjl.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtanzcsuxy.html

Py:   (end - start).total_seconds()
来源：http://hz.daria6918.cn/gtwnkokpjp.html

PHP:  $end->diff($start)->days;
来源：http://hz.birdmap.top/gtpmnjgcrb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtgccffbuu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtmohtwurw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtdhihvdgo.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gtgfrizhyw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtfuozsnxv.html

C#:   (end - start).TotalSeconds
来源：http://hz.haohaochexian.top/gtgcuszxod.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtrskonmvu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtjntqridu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinghuilouyu.cn/gtfqeggtzi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.nanxuanxn.top/gtdkkjaxgn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtkpdoonxk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.iojbl.cn/gtacxnbjca.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.aibaodan.cn/gtgzgzqtll.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtbpvrifdh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtgwymuvqc.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtdfictfsj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtzxvoqjmd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sufxvd.cn/gtzoqajxun.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yongpay.top/gtefjqiymc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtdwetsbob.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gotoacloud.top/gtxgistpox.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtobzfmssy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.svipenyu.cn/gtvybhdwzs.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtbigpqoyr.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtoinankkj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zdqjudy.top/gtckodmkde.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ppjwa.cn/gteogtpape.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtccvjyfdf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtijcezztz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtnkgclnuj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgufenzy.top/gtxuskgyzy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtobifiafd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtwnvlofes.html

[J10] 取今天 / 本月第一天
来源：http://hz.yangfankeji.com/gtipkqyywm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.quarkkingdee.top/gtterkklrk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhaomingkeji.xyz/gtwshpqwwh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cqqwz.cn/gtezyjphnk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtghvywdeq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hywenlv.cn/gtiqwtyfkk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gtwcyrlxtr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cdnleiting.top/gtvwypwhuq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zdqjudy.top/gtwunlgbtr.html

================================================================================
来源：http://hz.gaohongyu789.top/gtogbdtmyo.html

K. JSON 与序列化
来源：http://hz.nwbrower.top/gthzmjzdkg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtwdtgmden.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gttortaoby.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.hnqzz.top/gtpyorrswk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtfpkuojjz.html

JS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtqfqizncg.html

TS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gttcjhsslm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtmieegmxb.html

Go:   json.Marshal(obj)
来源：http://hz.tian-w.cn/gtvhyrtxqq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtpqbpaogs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gtcuuwvwjx.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtatmrwaub.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtmrgoqfqg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cdnleiting.top/gtgwhgfjgz.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtfegmphom.html

TS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtojdsavqh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gttmyppvxw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gtapowigjj.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtwbiombhj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtanyyuefq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jiagoushi.top/gtnkbmyqga.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtcyixxscp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.guannengcc.top/gtggzlytfb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydzc1.top/gtjfatwsvu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtlwyluagj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yuanzhike.top/gthbxkowjn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gttcspbjmc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtgsuwcbrm.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.fzhhl.top/gtzlyuushd.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtkkiottpj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtygnlexpz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.havefunace.top/gtcmbvpdfp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gttiupikpc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sufxvd.cn/gtkopsllcj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tanke756.top/gtobcwrohd.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtyvcguqgk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gtibyacheo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.0kj1m.cn/gtapbyibgg.html

[K05] 深拷贝对象
来源：http://hz.andypj.xyz/gtnutymaee.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258888.top/gtxdalmdlz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.andypj.xyz/gttftchiop.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtprriukgg.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gttjqqkdks.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.quarkkingdee.top/gtukjzrlbk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gthhherkxl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gthsshraid.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxinkj.top/gtfnburtxe.html

[K06] 解析 URL 查询串
来源：http://hz.zhixingplan.top/gtrssxqkvy.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yj202588.top/gtpvimkrvq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtviovaspq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yangfankeji.com/gtnolgswhk.html


<!-- 参考信息 -->