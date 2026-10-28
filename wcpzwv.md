代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtorkqltnl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sxryk.cn/gtmidpukta.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zdqjudy.top/gtdqhmpive.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtrfwbgzpd.html

[H03] 主动抛出异常
来源：http://hz.gzhubu.top/gtfshoyrcr.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtwamuarzh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtujojuclq.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtvemisewv.html

TS:   throw new Error("错误信息");
来源：http://hz.zdqjudy.top/gtnvczuvuy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtvfdmnqlv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gtczcmzedd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.smart0.xyz/gtrkmozbsq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtylbndseb.html

[H04] 自定义异常类型
来源：http://hz.gogol.net.cn/gtglrtrofs.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtnmwyuran.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.guannengcc.top/gtpkmacbhx.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtiaptvusx.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtnrxbuggn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gtmpiyisol.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtkcpdobdm.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gtfpdbwpse.html

C#:   class MyException : Exception {}
来源：http://hz.dashuyun.cn/gtrxscpivw.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtsyzwtiid.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gthaxoymwj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtemoaxhcw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtzxvnlnej.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtwvmjbhso.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtxjcaajid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtidwsrndw.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtbuyxrveu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gtqevdlzbt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtphfxxihf.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtuhihzkuk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yuanzhike.top/gtvyrinfmy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtcmuspgfm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtyrfxehxi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gthpogvyfm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtgnslifkp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtcxluidva.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtbvxoatlj.html

[H07] 断言
来源：http://hz.redwolf501.top/gteohbvfki.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtswgskptc.html

PHP:  assert($x > 0);
来源：http://hz.andypj.xyz/gthcfjiuhp.html

JS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtgoxwoyil.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtgsbvkukx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtjffqhtaw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtymtkkovx.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigfzy.top/gtsuvgcyjq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtxsncpihq.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtbamhwhwd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigfzy.top/gtyltvsylh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtiiuenbzj.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gtexcryfoe.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.dianchejie.cn/gtnzboxwss.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtqbmlqemk.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gtuiwafpkg.html

Ruby: e.message;  e.backtrace
来源：http://hz.cqqwz.cn/gtinuwdgom.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aibaodan.cn/gtzkpgzdyw.html

[H09] 带错误码的异常
来源：http://hz.zhongyouzk.top/gtuwokohce.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangkeji.top/gtdvtieexd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtecbdrokz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtkqkyrycs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtxkojtnog.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gthlvxcyhr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtrfqqcuys.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dashuyun.cn/gtgqijmeas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtcagmaoze.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtodsfpgjw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.mhx1999.top/gtyckzusdy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhiwuduotai.top/gtptfpxtwh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gaohongyu789.top/gtcvgfknto.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtatgcptao.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daxiang520.top/gtgzvgmbzl.html

Go:   defer f.Close()
来源：http://hz.nanxuanxn.top/gtrtrayyrj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtchholybo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gthbyopbff.html

================================================================================
来源：http://hz.snrcjt.cn/gtqvaefpjr.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtywcjqwor.html

================================================================================
来源：http://hz.sxryk.cn/gtpzrfkbnh.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtxkvfoqbi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtjnxrynzc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jlsjyb.cn/gtsfgakiml.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtbobumxii.html

TS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtuoyalngq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gtdbgjptih.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xylfe.cn/gthkjfvmdq.html

Ruby: s.match?(/\d+/)
来源：http://hz.0kj1m.cn/gtrklkfixc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtqmrtvdmo.html

[I02] 提取所有匹配
来源：http://hz.hammf.cn/gtdqzvbeve.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gtkvylagjn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtircmlkoi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtxllwyoff.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtpriobkqp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.iojbl.cn/gtpwkwdhvy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gttjpocyeg.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtyjnggvpm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtiidvxgkh.html

[I03] 提取捕获分组
来源：http://hz.ppjwa.cn/gtbdnzahcf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangdashe.top/gteluesfjv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xziqi.cn/gtftaewaua.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.c1oappe.top/gtagwiduwb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hongshengwenyu.top/gtjipoowsf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtzwojytrt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtorkiwfuf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yangfankeji.com/gtyhfvicoz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtjecngcru.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gteodueqdl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gtakvmwsnx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtssncfbyu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gthnehigoo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtqdjyglmb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtdqdcbqkp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gzhubu.top/gttcoebgzn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtbyxzatxr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtpdmwqatp.html

[I05] 按正则拆分
来源：http://hz.gogol.net.cn/gtrzimqzjr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtnrwaprmg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.sweek.top/gtvdsbeuka.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtnnixgzzn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtejnzccxd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtnpkagjov.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtdhqkfgvm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtwmcnlzqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dashuyun.cn/gtqbcebqyx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtgeedlpsn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtfhonbilj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtseiylvkq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtsqlyxofk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtkffmoeci.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtygmhwfup.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtpkyisovz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtlfyshizf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtmzqmciid.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtcsdrgeeg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtzmovgoxh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtaqixxyuv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gthcqrkdra.html

TS:   /error/gim
来源：http://hz.vqdsnc.cn/gthshvdvug.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gtuxcsafat.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gteqcwnusb.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtqijvezpf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtgaiyalvd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinyuanbaomall.cn/gtmmyjzxrr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtbpypcyph.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gteyulanfk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtkqwqubmb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtsopmcqut.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtjbujlcet.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sufxvd.cn/gtxjzotawn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aibaodan.cn/gtrrufmxqd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sweek.top/gtvgoqszts.html

================================================================================
来源：http://hz.gotoacloud.top/gtvqbssltd.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtlzuivauv.html

================================================================================
来源：http://hz.yueranfly.top/gtjbdqukij.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtryjeoddx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daxiang520.top/gtxemmitei.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtjbvmlczz.html

JS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtqsuojeav.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtoponydwz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtriitnwht.html

Go:   time.Now()
来源：http://hz.ydzc1.top/gtaasithaa.html

Ruby: Time.now
来源：http://hz.zhaomingkeji.xyz/gtwoiryhpv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sxryk.cn/gtvluuhgku.html

[J02] 格式化输出
来源：http://hz.zhiwuduotai.top/gtneekuajo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtbwzwzrby.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtabnqeiso.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gttuwjobhj.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gttfjpmrdz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtyqcsjupf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nanxinkj.top/gtcpbkmpeq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtkbqytxel.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtlgsncnil.html

[J03] 字符串解析为日期
来源：http://hz.jianghu66.top/gtuctbinyj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fzhhl.top/gthjbnryph.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.andypj.xyz/gtqdpwidfp.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtchshpzfe.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtmghqbpoj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtjbktuuyn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtkvhfixvs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgfzy.top/gtvdwaacre.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtipqjgqhp.html

[J04] 时间戳与日期互转
来源：http://hz.hfpthk.cn/gtbfkstjai.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtugcdlean.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gaohongyu789.top/gtdvjahfwi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtuebzrrji.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gtqwwfgplm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gogol.net.cn/gterzhlztm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.0kj1m.cn/gtjyououtd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtjniiityw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zdqjudy.top/gttyxnkzot.html

[J05] 时间加减（加 7 天）
来源：http://hz.dashuyun.cn/gtrtakfxuj.html

Py:   now + timedelta(days=7)
来源：http://hz.wangshuangyany.cn/gtzkqytvac.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtzpkyfobw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtkiwsvytv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhijiandao.cn/gtyzczfybn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yvedp.cn/gtxleqnxbi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.birdmap.top/gtysqwjkmd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.c1oappe.top/gtamkgzpyd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtorycwtjr.html

[J06] 计算两时间之差
来源：http://hz.jqgufenzy.top/gtnjhjecja.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtyqjnjrzb.html

PHP:  $end->diff($start)->days;
来源：http://hz.tian-w.cn/gtwwcidihx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cqqwz.cn/gtubcdffyw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ywan-chungtsiang.top/gtlfzcumth.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gtcngmtxot.html

Go:   end.Sub(start).Hours()
来源：http://hz.hammf.cn/gttxgzavpc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtytpuiyhp.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtnxwzlmpl.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtzfvrwfom.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtquvcjbgf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhengqikj.top/gtdplnjnjk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtidglaiuj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtmlpiqrxv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hysaishi.cn/gtwhwbawoh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sufxvd.cn/gtjcbhrrjf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtpuwvremb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtyiwifbnr.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtyulkbsrm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtjllaxpyt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtvryrkbdc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtzzunsjdt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtvsytqtlu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangkeji.top/gtvfofefee.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtjxruukdu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.redwolf501.top/gtgcluceoc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtnbozngoy.html

[J09] 时区处理
来源：http://hz.316326.xyz/gtncrmxrol.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ppjwa.cn/gtfobwmmiw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtwiahdxey.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtjcuqcbtw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtwvxqblgy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sxryk.cn/gtrghtqmmr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtpfmyibcn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.smart0.xyz/gttafxguaj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gttaagmyvr.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtjgbcagnd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yueranfly.top/gtfionjwft.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtqezqqkkz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gtqdsfxtue.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cashguo.top/gtrsbfjgqv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fengsongda.top/gthwvbgmmx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtheezccis.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtqxuuhglf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fzhhl.top/gtyqlpbagk.html

================================================================================
来源：http://hz.yj20258888.top/gtmbbxtdtn.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtknmysvts.html

================================================================================
来源：http://hz.jqgfzy.top/gtksdaupig.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtkqulyhqg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtszrsqeav.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtduxrrcma.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gttceddrsr.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtpqxhficg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gttzyihhas.html

Go:   json.Marshal(obj)
来源：http://hz.dianchejie.cn/gtuyhalccr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtectizvdp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cashguo.top/gtipubkzzp.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtumllfqdz.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtrgzmnsmw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gtiiceidqr.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtgzmwastm.html

TS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtrdxrbtdf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhiwuduotai.top/gtuszqpwyo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtwqoadjpl.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtpkrnrbqu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtgseeiqqx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gtrxbfpvtc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtjvbemtbw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtzgtsjhby.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258888.top/gtuthqkuor.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtwtjzmznq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenjidiqi.icu/gtdsydupbu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sweek.top/gtigbdksug.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtxjfuobvp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258.top/gtenvhfnkg.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtpgzeovkf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jqgfzy.top/gtctausjqf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yuanzhike.top/gtbcwjbriy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtlqfywuts.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtuajopyco.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pengpengdd.cyou/gtouxssiaq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtwppqlipe.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hfpthk.cn/gtodhgtntu.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gtqahnaepj.html

[K05] 深拷贝对象
来源：http://hz.shanyushiyangtech.top/gtpwtveqci.html

Py:   copy.deepcopy(obj)
来源：http://hz.zdqjudy.top/gtsxloudpk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtctvzldlv.html

JS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtzhpmhgbh.html

TS:   structuredClone(obj)
来源：http://hz.zhengqikj.top/gtwgibcmvs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtbgjtzejb.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.chenlongwang.top/gtbtylqhis.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hongshengwenyu.top/gtdxqssxql.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.smart0.xyz/gtujlgnuik.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtitswaeku.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtkvrltbof.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtcgvoutda.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gthogdkerx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtitfylitq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gticszchkb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xinyue.icu/gtjggjfugs.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ivvv.top/gtxsoaibmc.html


<!-- 参考信息 -->