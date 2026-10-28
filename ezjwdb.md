代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhoulong.xyz/gtbhogwndj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtdigmfelx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtyelpgejc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtwmtgkzdi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtxaztxsvn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shzxlz.cn/gtcahtswte.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtmblxqqup.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hfpthk.cn/gtauxjjdos.html

[H03] 主动抛出异常
来源：http://hz.ehwqpu.com/gtkjnzgtft.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtdansqsid.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gttpntwjeo.html

JS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtujopnznf.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtvbrbdrda.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtwhzoizov.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuetiantiany.cn/gtksqodbzl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hfpthk.cn/gtarqbatqn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtgtrojvmr.html

[H04] 自定义异常类型
来源：http://hz.pycfn.com/gtodpipmzp.html

Py:   class MyError(Exception): pass
来源：http://hz.gaohongyu789.top/gtoetkkwhb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtiwbzgtcj.html

JS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtqspaohwx.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtfxvgoytz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtqnmhjehz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtjvxcfpqg.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtcayejxqh.html

C#:   class MyException : Exception {}
来源：http://hz.nanxuanxn.top/gtneyasypc.html

[H05] 捕获特定类型
来源：http://hz.ywan-chungtsiang.top/gttcyknfbc.html

Py:   except ValueError as e:
来源：http://hz.zhixingplan.top/gtsonmleng.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtumdjscvw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtadejbwyq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtcullkpqo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtenlshfir.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gtkrrieiqn.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhaomingkeji.xyz/gtybewbfiz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuxming.cn/gttvzmrukg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtshvxvdtt.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtutxuavzf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhaomingkeji.xyz/gtqpnvylam.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gthdlasnbw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtswrleoox.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtvsdvlohy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtpesanfej.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtdhdcbafy.html

C#:   obj?.A?.B ?? default
来源：http://hz.iojbl.cn/gtndxtrhma.html

[H07] 断言
来源：http://hz.316326.xyz/gtqzjypemm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangshuangyany.cn/gtehziafrq.html

PHP:  assert($x > 0);
来源：http://hz.tanke756.top/gtjclcoxij.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtjkscsxfx.html

TS:   console.assert(x > 0);
来源：http://hz.jlsjyb.cn/gtzivrmnix.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtwcbxrokd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gtnyumekhf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtbrtkmgky.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtveybybip.html

[H08] 获取错误信息与堆栈
来源：http://hz.redwolf501.top/gtjdwlivnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtccsylvwx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtfbundjpc.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtaqyghbiv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.0kj1m.cn/gtytgdycoj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shuidangran.top/gtibmwkldk.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtsnonfoxu.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtmpsvcevc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtspymsqli.html

[H09] 带错误码的异常
来源：http://hz.316326.xyz/gtjdqdmxhh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtqruacjmj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtfoxmjcfj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtkcjilrpn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangshuangyany.cn/gtcvtfcsju.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtdblljazk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jianghu66.top/gtrqrpcrje.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinghuilouyu.cn/gtgsedzbcz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydzc1.top/gtnmwpjgvh.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtycszaxrd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtqbradlbi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtveagtkpl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtaxhgonmt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtzienwhsd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhoulong.xyz/gtkeqibnpc.html

Go:   defer f.Close()
来源：http://hz.cashguo.top/gtefburifc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtchdnqckv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtemdovkpc.html

================================================================================
来源：http://hz.aibaodan.cn/gtpbolfgud.html

I. 正则表达式
来源：http://hz.yj20258.top/gtwoakrdji.html

================================================================================
来源：http://hz.hysaishi.cn/gtfkpgaoss.html

[I01] 判断是否匹配
来源：http://hz.xinyue.icu/gtptuihvsq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtdilaphfx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtqghewlyj.html

JS:   /\d+/.test(s)
来源：http://hz.ydjk.org.cn/gthqvnlria.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtmpmbuydv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.mhx1999.top/gtvyjmvyrc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtibfputvm.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangshuangyany.cn/gtaqptdzmb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gtqlscmlsr.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gtbidpqimd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtwkkptnsb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtolaxtbev.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangdashe.top/gtfzdgbooo.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gthtnosxuj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtupotbzlx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtkfmpaarr.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtgtddnmlr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtxrbxhizo.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtwguutluc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtxutnfnxy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gttojfhsix.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gtxspjlihw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daxiang520.top/gtdrlzrcew.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hammf.cn/gthvhukyqh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtnwtvjulf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuanzhike.top/gtfemqduxf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtpultiwcr.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gtypgxzghu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtjpjmrxdc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtvlkndktz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gthsnzoikj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtfxrkfjea.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.kuanghao11.cn/gthevtkifi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gteodijvdm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtulcyldad.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtrlyyhyko.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtouvwlhnm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtuouuspgk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnqzz.top/gtxunkhnoq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtysvskvvp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtcbsvsrih.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tanke756.top/gtggyjqtik.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtiaudmniv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtotgindmd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangtech.top/gtbwyzheyv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtfeedbvec.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtftkspnmo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtygvscbzr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtekwwybsu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtuixyrswg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtffgoiwdo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shzxlz.cn/gtzktrdijj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtlwgwomau.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtltpfzuna.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtytnsylyh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ywan-chungtsiang.top/gtjyeganob.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gttppjstml.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gtudlzrasg.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtrkpkyrcl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtznwttxyr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtpnvxfwrc.html

Ruby: s.scan(/error/i)
来源：http://hz.hywenlv.cn/gtqhcyuxyj.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtafiffvaa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sufxvd.cn/gtkimpvpor.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtnklirlfv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtfoghysxb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtwhooxxjz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtehykmerj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinghuilouyu.cn/gtjizlitlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtewjeenma.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cashguo.top/gtxsllvgkc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cashguo.top/gtkcppkpfp.html

================================================================================
来源：http://hz.guowangkeji.top/gttcqlbiol.html

J. 日期与时间
来源：http://hz.zhiwuduotai.top/gtoaoobjnp.html

================================================================================
来源：http://hz.tianlin.xyz/gttexoichn.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtqubwauav.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nwbrower.top/gtazxuhgsi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtjuqlixcc.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtmfhiczge.html

TS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtwrefhyrv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ivvv.top/gtkhegxntg.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtbguylmns.html

Ruby: Time.now
来源：http://hz.xuanzx.com/gtdmuflzmf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xziqi.cn/gtpoxpwpma.html

[J02] 格式化输出
来源：http://hz.gaohongyu789.top/gtfndireeh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtxgpgdagx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtdrtnoznv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yangfankeji.com/gtoppgmxgp.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtayyfgfld.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gttgsflcor.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.316326.xyz/gttohgjtbe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtcgzcodgw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtjykbrvsu.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtqmcmejkm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gzhubu.top/gtukkaditj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.redwolf501.top/gtkicqbozu.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtmifxjybg.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtjaomwonh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtcrrwvlvb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.meibo888.top/gtatxrgdik.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtkdfnulcy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtdgdghngc.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtdpldfvmg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtqtahetdt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtszbtvlby.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shanyushiyangtech.top/gtpdchykni.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gtowondzmo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtnywnbrxd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hysaishi.cn/gtvapifkwj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ivvv.top/gthcdmricu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cucudq.cn/gtreoauibp.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtlhsqchmp.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtuxszixnk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtzzuzokim.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtfrlywpji.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtuidmftcg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhiwuduotai.top/gtjciablkg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtsdivqvag.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gtcmxgazro.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtdztxeuvw.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gtwziqjhso.html

Py:   (end - start).total_seconds()
来源：http://hz.shzxlz.cn/gtqxzwlfeo.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtloalonth.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtruujpeas.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.meibo888.top/gtdamrraqa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258.top/gthibgksxb.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenzaomai.com/gtepyhwbrg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtsahzrvju.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj20258888.top/gtofuqbqax.html

[J07] 比较两个日期
来源：http://hz.dianchejie.cn/gttlwuqyan.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtcaznfisa.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gttppavutm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtowcjuuev.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtsypavaqg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gteatsfvmg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhijiandao.cn/gtwdoubtfm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtqnqmydcp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtxgoeabhx.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtqtstvhpr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtjduwtbzr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtgxrwornl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtopytlozs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gthtcnxqsg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtprxxbqhz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gthodahgtn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tanke756.top/gtvantiydu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtyoqdnbqe.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtwoocrhdd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xziqi.cn/gtinruzscz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtjscqjecb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydzc1.top/gtuyfgiwfv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtmgtraaru.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ppjwa.cn/gtpdbyktfc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtoylizxsg.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtzilbidcv.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gtcufuzuds.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtmhdhtdll.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtulnbsujo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ivvv.top/gtnuidpigo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgufenzy.top/gtpnxkuqbz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtbtukoyfn.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtxgmqoohz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.redwolf501.top/gtgxxsksez.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydzc1.top/gtrznbjkcz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtcgasszab.html

================================================================================
来源：http://hz.bjfxy.top/gtjcjxljfl.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtqsvfwwrh.html

================================================================================
来源：http://hz.0kj1m.cn/gtwpwcwwob.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinghuilouyu.cn/gtfbyvfmlr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtxxnmxacu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtpkparzwa.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtdosdwswe.html

TS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtdvfvjfdf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sweek.top/gtxftkbjzi.html

Go:   json.Marshal(obj)
来源：http://hz.xuanzx.com/gttqaafoxu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtglgaafwt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gtaledhbbc.html

[K02] JSON 字符串转对象
来源：http://hz.hongshengwenyu.top/gtffeljgun.html

Py:   json.loads(s)
来源：http://hz.sysykeji.top/gthmuuidco.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtmwvokoea.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtoqimdyju.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtphjzcdnu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtauihmtkx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dianchejie.cn/gtgzcfrbln.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtznzayhfa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtukulzmjm.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtfzqsyxab.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtwsgnixdu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtljdrytss.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtvjzeherx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jlsjyb.cn/gtjpsyhwyd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhongyouzk.top/gticnwrbbv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sufxvd.cn/gtamgilawb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sweek.top/gtwzrddnby.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtkkxrajuy.html

[K04] 读取 JSON 文件
来源：http://hz.jiagoushi.top/gtrjqpejpw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuxming.cn/gtybsqhiur.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtgvnzlddh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtszgiifuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gthvsecxac.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtboueiazb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtnwqjkbpy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sxryk.cn/gtjjgclxxx.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gtazkakimp.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtolulfpdw.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtkkzsdzdq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gthmfmvljq.html

JS:   structuredClone(obj)
来源：http://hz.guowangkeji.top/gtgdvyillg.html

TS:   structuredClone(obj)
来源：http://hz.jinyuanbaomall.cn/gtwzucsrmn.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtsxijlvct.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gtgajihlzp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxinkj.top/gtdawsowar.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hnqzz.top/gtiqltpyut.html

[K06] 解析 URL 查询串
来源：http://hz.shzxlz.cn/gthasegrku.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zdqjudy.top/gtwjhxwuou.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtzcibfcuc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtnxfxgotu.html


<!-- 参考信息 -->