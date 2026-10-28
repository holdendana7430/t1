代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenzaomai.com/gtcypzhjjb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtnewaatdq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtkhyyirse.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtablxotfc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtmwilsaom.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zycfv.cn/gtccyjptoy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtqynaxauh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgfzy.top/gtgybbsojl.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtyjufimxq.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtzfajnlrp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtgybdmzvg.html

JS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtuvggocmn.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigufen.top/gtcbfdqqot.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtosqjkwuw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtqfizyqgu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gzhubu.top/gtwmzfdobn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtnrgvvirs.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtikpiwzyg.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtgwpvjvzc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtjgnudycl.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtbgrbcpet.html

TS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtpfrtlbts.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tianlin.xyz/gtlwxbeghh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtsmglmgby.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuanzhike.top/gtdkknmjzm.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtbmkyunlw.html

[H05] 捕获特定类型
来源：http://hz.fzhhl.top/gtxhowkwlh.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gtzctcpmkq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtzzwzqmsa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtfapkbpoq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuanzx.com/gtitzdchek.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xuanzx.com/gtekrcwhbs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuanzx.com/gtzdheajvl.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtfcnbpjgz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gttrjokkmz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daria6918.cn/gtxzyyirpu.html

Py:   value = d.get("k") or default
来源：http://hz.hywenlv.cn/gtdciztkfv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtlomuxlja.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtxqytsjgn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtjjflijme.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtmovfkxqa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cashguo.top/gtejfadzip.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtbmhuxyno.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtntyxnyal.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtxgpyxwot.html

Py:   assert x > 0, "必须为正"
来源：http://hz.guannengcc.top/gtjbnpdxux.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gtdklciwjh.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtubjjrsqe.html

TS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtyyrjvyzc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtsirkzfnc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj20258888.top/gtmnpffjot.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ywan-chungtsiang.top/gtoxunpqjh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.quarkkingdee.top/gtbollnfvw.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtjffyejzw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gthirqkawd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.smart0.xyz/gtgmwlywva.html

JS:   e.message;  e.stack
来源：http://hz.svipenyu.cn/gtedgqvvhm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sufxvd.cn/gtdtmwbvlf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhengqikj.top/gtoclozrlz.html

Go:   err.Error()
来源：http://hz.sufxvd.cn/gthzuvcalt.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenzaomai.com/gtfgdjrdzi.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtrqqueqlr.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtggyxowbs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fzhhl.top/gtqgmbjblq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtjbaipwjw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sxryk.cn/gtldnnxshf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guannengcc.top/gtlbuuyhhc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtxqylhbku.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtgbcqcips.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtahrjedqe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xylfe.cn/gttlmvztqr.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtcxmgszcs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtpggxhpep.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtpjmdcvcq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtxjcmqsda.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtzgecjjld.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtuarisnny.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtccuixqda.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.aizwys.cn/gtfhrxbukn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtevbgjvsj.html

================================================================================
来源：http://hz.xziqi.cn/gtosdnhcbp.html

I. 正则表达式
来源：http://hz.jyoumei.cn/gtsqknobke.html

================================================================================
来源：http://hz.jiagoushi.top/gtddmafjnh.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtnhpoxzkq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cucudq.cn/gtlharnvuz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtqtvcevbq.html

JS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtnpimkoxq.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtyiisfhkm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtsqopmxnr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtjhjohggx.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtweakruqb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhongyouzk.top/gtakpdstqm.html

[I02] 提取所有匹配
来源：http://hz.daxiang520.top/gthmsjjtjc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgufenzy.top/gtuopivqpc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gotoacloud.top/gtssupumjq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtvbxszvpp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhijiandao.cn/gtdgaagdnv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cdnleiting.top/gtgltkeadt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tanke756.top/gttcuumvkz.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtxbduzqxe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnqzz.top/gttnbqfffg.html

[I03] 提取捕获分组
来源：http://hz.iojbl.cn/gtamzwqzol.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sxryk.cn/gtdkefjxrg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hongshengwenyu.top/gtsvnguldy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xinyue.icu/gtlnbxgxfw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuetiantiany.cn/gtkjhjoeun.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zycfv.cn/gtqnzqsxkr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtjpggdotw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtozkhlgds.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cheryme.top/gtmdgxqkqu.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtbhufmpuh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangkeji.top/gttujxiiiv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtegyrxvix.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtwklmosya.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gteukwsdak.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yueranfly.top/gtdolkccwc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinqigfzy.top/gtwzcusgsz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtynwqujvw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.smart0.xyz/gtvqhrtcev.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtsbgypioo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.quarkkingdee.top/gtozkenwuu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtdwmmqxuh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtsjbxufvk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gttjfupzbs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hywenlv.cn/gtlizmwuux.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tian-w.cn/gtkpttvuag.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtptifmrxk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtsagkofao.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydzc1.top/gtkzrlfpqb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtfnunqtkm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj202588.top/gtomyyglyc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtlretabui.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.birdmap.top/gtoadssaxg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtxvexoear.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinghuilouyu.cn/gtitosswuv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtgiywavrc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtjycenzqt.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtpualitgf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guannengcc.top/gtpwcnzzbk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenlongwang.top/gtsalcdtlc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtxpadwios.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gtseyqywxm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtxitqhjcq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtcyjtbfet.html

Ruby: s.scan(/error/i)
来源：http://hz.redwolf501.top/gtglumafuv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtownvrojk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtsmibmwbf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.c1oappe.top/gtekigskex.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtrodxpksc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtqjkrjpeg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtwnttfact.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtcwpjjztd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtaxduccsd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtjnsukpwb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtuulffhka.html

================================================================================
来源：http://hz.ehwqpu.com/gtxlukskhs.html

J. 日期与时间
来源：http://hz.shzxlz.cn/gtdhtnmzqp.html

================================================================================
来源：http://hz.gogol.net.cn/gtgraaybfy.html

[J01] 获取当前时间
来源：http://hz.fengsongda.top/gtjsivqpww.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtsyftmdwb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.iojbl.cn/gteeoaqqmv.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtgapdnxiq.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtzfskzcer.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gttelqagas.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtvpxaavjr.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtsorcqcev.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtnuimhafh.html

[J02] 格式化输出
来源：http://hz.xuanzx.com/gtsepygyim.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtuqtpuyjx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtubrwnozi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtjltoppas.html

TS:   d.toISOString()
来源：http://hz.chenjidiqi.icu/gteuwbdrqa.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xziqi.cn/gtchtjdfdu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtrmfrocqa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daria6918.cn/gtlxzjtned.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtghrbeonn.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtofgfdvmf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtnuhejtui.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtnxywyhai.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtqwutvxfv.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtyfarogav.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtfixonemo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtciagweaf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ybcxt.top/gtzargwmib.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtxdaroalm.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtqyolhlnq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ppjwa.cn/gtmzsyopgq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gthbxxzdhm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtwrwtigni.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pengpengdd.cyou/gtlhdnaxmg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenlongwang.top/gtoeggeyzm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.cashguo.top/gtrablhsvj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtulbqctjp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtvgjgpjvf.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtumqqhgzg.html

Py:   now + timedelta(days=7)
来源：http://hz.sufxvd.cn/gtyxkmpqsd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtpezroqpp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gthsfsfuwu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gttgmbuozp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gteftywivs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.smart0.xyz/gtlbmgnpph.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtptvillur.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jyoumei.cn/gtwidyftsa.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gttpbpqxeq.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtnymjsngx.html

PHP:  $end->diff($start)->days;
来源：http://hz.gzhubu.top/gtdtqbtbsu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtpytlmene.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtmoxepwbw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fengsongda.top/gtfwgcqtpk.html

Go:   end.Sub(start).Hours()
来源：http://hz.xylfe.cn/gtyxarikal.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtehdldmhx.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtldeihfbc.html

[J07] 比较两个日期
来源：http://hz.redwolf501.top/gtmkvvsmov.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtmppfguvi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ywan-chungtsiang.top/gtrkiuhvxl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtfkzykhtr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtharzekqx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gtrhqaqipm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gtufjengou.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtkxdphafr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuanzx.com/gtvjbkqsha.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtkiqqjdym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtnwenbahh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.guowangkeji.top/gtpnzynaxg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gthgsshmam.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtbkdlvbbx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydzc1.top/gtxfhtcncx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtosdxhsef.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cashguo.top/gtmskfzptp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtsgnaflwx.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtwiwvogaw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtochoxxnk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtwenehhbd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtplvbqqij.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtwkozaqxd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtphgpyuww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.dashuyun.cn/gtakixsqof.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gttsuqbprs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cucudq.cn/gtpxtwjeuf.html

[J10] 取今天 / 本月第一天
来源：http://hz.ivvv.top/gtogmiyicr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtlrhhjlyn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gttemeuoua.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtpgflympa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhengqikj.top/gtnbaspzot.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtmnzosvvg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtztelsuzp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtjthrijfd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtijvhbamn.html

================================================================================
来源：http://hz.ppjwa.cn/gtaeknpdpu.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtcgcdorzk.html

================================================================================
来源：http://hz.chenzaomai.com/gtbjfivxvm.html

[K01] 对象转 JSON 字符串
来源：http://hz.0kj1m.cn/gtdmaqyzax.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gtyxsywisl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tian-w.cn/gtowwjdmzf.html

JS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtocqcblau.html

TS:   JSON.stringify(obj)
来源：http://hz.yueranfly.top/gtfxzajwez.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtopmamhea.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtcqgbhrba.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtwkpbtftf.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtazekhioh.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtyvjwwtsr.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtweylqqmi.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtyybpwukd.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtackxedxw.html

TS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtxwerumzl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtonezklvn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtvsawovrb.html

Ruby: JSON.parse(s)
来源：http://hz.yongpay.top/gtbsauvigk.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jqgufenzy.top/gttkohwoui.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuanzx.com/gtatuiunub.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtqiqwyoij.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.birdmap.top/gtxpoyvquk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtdygguryh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtldxeyopb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guowangkeji.top/gtzdryqpwc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtivrgxpkh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gtrgilqtkb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtfqregrtx.html

[K04] 读取 JSON 文件
来源：http://hz.316326.xyz/gtbeabnndl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenzaomai.com/gtaepjxdqk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtqoqcxbrt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtcbwnywev.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtirgjhnja.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinyuanbaomall.cn/gtovrcujfz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenjidiqi.icu/gtkykuftsg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtjinctcel.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtspwyhvgw.html

[K05] 深拷贝对象
来源：http://hz.chenjidiqi.icu/gtetexwrhj.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtcoalgpso.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cqqwz.cn/gtnowexqzz.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtynbxtkxv.html

TS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtwjofnbpo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj202588.top/gtraqoljxv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtsghddrcl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gtgxnzuzhk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhoulong.xyz/gtxkawautj.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtqzffjvqp.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.svipenyu.cn/gtbcsxsuxw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtczgotyon.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtgmyowdfo.html


<!-- 参考信息 -->