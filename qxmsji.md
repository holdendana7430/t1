代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtvdynjlrd.html

Ruby: obj.instance_variables
来源：http://hz.xingfuxueyuan.xyz/gtmqyofjnu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgfzy.top/gtfcnjfoxo.html

================================================================================
来源：http://hz.chenlongwang.top/gtxfzifjbe.html

H. 异常与错误处理
来源：http://hz.yvedp.cn/gtbvfidspo.html

================================================================================
来源：http://hz.xylfe.cn/gtlpzepfjz.html

[H01] try / catch 基础
来源：http://hz.zhixingplan.top/gtksimjhfx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sysykeji.top/gtyeyivuvp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhongyouzk.top/gtommekuew.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtuyjpvnla.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtoefntcrg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtsrbvibip.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xziqi.cn/gteziavypd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtzqbkaqjk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtawlhyyxq.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtrgdpaqmo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gtdcwljqfb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtycfcccym.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtcqicongt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtxzohslnx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gttqpqgxcf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xinyue.icu/gtljkrezxy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.fengsongda.top/gtvcjeihcg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xziqi.cn/gtbzqjqmpt.html

[H03] 主动抛出异常
来源：http://hz.svipenyu.cn/gthgeuiojf.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gtsxphxeya.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtvvrbqlnu.html

JS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gttgsuiqru.html

TS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtnxfcvnli.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yonumen.top/gtrpmofydg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yonumen.top/gtbayjyrks.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cucudq.cn/gthcxzggjh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtzhafdakk.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtlhpwhrfw.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtpwjxzfgj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nwbrower.top/gtdzpblrih.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtgzinuoff.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gthmejlljs.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shangyingyoupin.top/gtrhfokyyj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtiktbiblk.html

Ruby: class MyError < StandardError; end
来源：http://hz.jlsjyb.cn/gtkrlkifau.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gtdhknwumn.html

[H05] 捕获特定类型
来源：http://hz.cashguo.top/gtcamqweuo.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtsbjkvwaj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jyoumei.cn/gtxgrlkdgv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhengqikj.top/gtsgxyyjpk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gteqzuzpzj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gttnjqrijt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fzhhl.top/gtjaclotad.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtjxvoucvs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gotoacloud.top/gtoittvofb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hfpthk.cn/gtdhqjtaes.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtwoowhfry.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtkiancwat.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtbvswjblt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.svipenyu.cn/gtuwvosgly.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gtaxuxcezp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtgaexymou.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ehwqpu.com/gtizjblzuo.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtplwzwehj.html

[H07] 断言
来源：http://hz.daxiang520.top/gtqlfdeyjw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gttcidcfyx.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtwgmdvzyn.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtbwomhziv.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtnusnutsi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gttzsdeghf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtrtdeveic.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.andypj.xyz/gtqqdsmawa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pycfn.com/gtatlchonh.html

[H08] 获取错误信息与堆栈
来源：http://hz.sxryk.cn/gtdkocdlku.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258.top/gtqehsksaq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gthzzineep.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtdxsxtpnq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.birdmap.top/gtrdmjcmhy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtzwktruyo.html

Go:   err.Error()
来源：http://hz.jinghuilouyu.cn/gticbwodfz.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtlnxpdgnx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sysykeji.top/gtphemusif.html

[H09] 带错误码的异常
来源：http://hz.daxiang520.top/gttueyytee.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hfpthk.cn/gtvpkcwgaz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtummyulhu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtgrojdwbt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtsxxtfqxn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtaaitlmlh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtdrlspjtm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtmcfzmrkg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtossgfysv.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gtxjndkydb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtynxhftkk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aizwys.cn/gtftqjqooj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtudrnxypd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtsrzrallv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gaohongyu789.top/gtqsjwrmck.html

Go:   defer f.Close()
来源：http://hz.yanxiufei.cn/gteqyospji.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhiwuduotai.top/gtzzdwgyle.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhijiandao.cn/gtnirurtfz.html

================================================================================
来源：http://hz.yongpay.top/gtiupugxge.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtsbarnpsx.html

================================================================================
来源：http://hz.zhixingplan.top/gthvjsvrdr.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtnxbveklt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtiypvmtdx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtupzkrskr.html

JS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtxdkljwah.html

TS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtbnsaybju.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hongshengwenyu.top/gtmhmpjboj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtgripxdze.html

Ruby: s.match?(/\d+/)
来源：http://hz.gotoacloud.top/gtazkuquhv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtwkvixmey.html

[I02] 提取所有匹配
来源：http://hz.hongshengwenyu.top/gthgosxibu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gtayhbbrqy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ivvv.top/gtyvdbmekr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shuidangran.top/gtstpzbgwv.html

TS:   s.match(/\d+/g)
来源：http://hz.svipenyu.cn/gttiubxxbz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hammf.cn/gtjaikxdrz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtweuluhes.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydzc1.top/gtyutmskvg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtfeyeiejx.html

[I03] 提取捕获分组
来源：http://hz.pycfn.com/gtwakqwwab.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtapcmtlkk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtyofgmjyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtdrhcpgap.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtgxhpklbm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtiyohcjmp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hywenlv.cn/gtgizkffci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.aibaodan.cn/gtioidsdvn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gtkgspvvzr.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtnvcztvce.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yanxiufei.cn/gtodisuxwr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hammf.cn/gtkecatdjw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtdwouzsuv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtpeonxket.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gttyrhfskj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtkcaosbur.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtvwnczsrr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtzvxodvqo.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtwucbvoze.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cdnleiting.top/gtaxkjnhar.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtoizmezpc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtnpgooglo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtcknltoyh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gtaeseyrel.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.meibo888.top/gtknlifteb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shuidangran.top/gtexdmnqpj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtuqxvppar.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yueranfly.top/gtjnjhvwol.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtebpbonwn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.vqdsnc.cn/gtkvfmyyeq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtfcedpibh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtzmhgckqv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xinyue.icu/gtpinotjpp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.andypj.xyz/gttgnjyiar.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yuxming.cn/gtdnesrfqm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtqexgqlcn.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtcmuvlvof.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtwdzfovcu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtdhtvjzji.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtlpmezjup.html

TS:   /error/gim
来源：http://hz.yongpay.top/gtkmgpeaxz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gthssxpdil.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.nanxuanxn.top/gtilxsqzbl.html

Ruby: s.scan(/error/i)
来源：http://hz.xuanzx.com/gtcorvvfpv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangshuangyany.cn/gtesphfqfq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shzxlz.cn/gtjxehokus.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yangfankeji.com/gtvmcwaidy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jianghu66.top/gtohluhekq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtqxafmdmg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgfzy.top/gtprzjiqyi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtorhkbons.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jianghu66.top/gtsokfcpgb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtklhhdlqp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtapnlbbuu.html

================================================================================
来源：http://hz.cheryme.top/gtxfjonzin.html

J. 日期与时间
来源：http://hz.tian-w.cn/gtldfkswtd.html

================================================================================
来源：http://hz.tian-w.cn/gtgzmjiieg.html

[J01] 获取当前时间
来源：http://hz.jlsjyb.cn/gtkzgxucso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.pycfn.com/gtlyhofpmy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtascoyesf.html

JS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtqqfsmppe.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtjbvizgxm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtldobpcwx.html

Go:   time.Now()
来源：http://hz.jinghuilouyu.cn/gttvdoswgv.html

Ruby: Time.now
来源：http://hz.hywenlv.cn/gtwumxqvsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtrcpgpzup.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtfwlsskqe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtstctkmuf.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtklmyfsjq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinyuanbaomall.cn/gtdavsgzvg.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtwltkiskm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aizwys.cn/gtvoolzaep.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gttsutjfoa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gtxxswberp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.iojbl.cn/gtohrtaqgr.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtacghvchj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gaohongyu789.top/gtbfgctken.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhongyouzk.top/gtmixvysil.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtganmjplx.html

TS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtjpejbpfa.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtyxmtfhuj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gttgahjypf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtmrngwphi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtldjmhsgu.html

[J04] 时间戳与日期互转
来源：http://hz.shuidangran.top/gthjjmbgpq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtjeessjsa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtzfdslidp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtdbcnkmsp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtphjdvpnb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangshuangyany.cn/gtyrkeoqom.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtccsdvvlm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jiagoushi.top/gtzjjortmg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtcxiqfsfc.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtzadsskmq.html

Py:   now + timedelta(days=7)
来源：http://hz.jiagoushi.top/gtckqhagyo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtbxbdrvjd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xziqi.cn/gtyjnmxcon.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtqpcwxxym.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nwbrower.top/gtzktmwqom.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.meibo888.top/gthgorznhz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtllytxvco.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gtftvkcpzo.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangtech.top/gtwvdvxguk.html

Py:   (end - start).total_seconds()
来源：http://hz.nanxinkj.top/gtieksgjir.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gthvzzqbrf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hywenlv.cn/gtdkjmpnxq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.mhx1999.top/gtwvexshqy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pengpengdd.cyou/gtlnwxtuzb.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtgvcvznin.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hnxiangtu.top/gtugdtpaum.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtlkmazlgt.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtknhajirw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gterxbkwgj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xziqi.cn/gtujujkclj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtwsqkhlpm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtmmnehaja.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtcamzbjhm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gtuhjehghz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtyjvluwvp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtbqbegyjb.html

[J08] 提取年月日与星期
来源：http://hz.ybcxt.top/gtalveclyr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtclafwdzi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gtjxngzfnx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtmflpiuar.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yanxiufei.cn/gtdkfylyvn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinyuanbaomall.cn/gtlfudcnip.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtersupneu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtoupxvebh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtmjvqhdry.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtddsxpogh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guowangkeji.top/gtlrckznhy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtllzruabv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtaymlklry.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtbgmoqiwe.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtdoyejhkr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tanke756.top/gtslkqhykj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sufxvd.cn/gtahwdnrin.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtfhkodrts.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj202588.top/gtwdzqerhi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.aizwys.cn/gtwnlipoxk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtlwgogmph.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sufxvd.cn/gtccvqlveq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtbebdzfst.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtrtapuhsj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtunvpqash.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinghuilouyu.cn/gttydhwkct.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cheryme.top/gtslmxlngg.html

================================================================================
来源：http://hz.jyoumei.cn/gthrnyladw.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtnpsxloqe.html

================================================================================
来源：http://hz.hnqzz.top/gtnwfjdgkd.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhiwuduotai.top/gtljvevkpi.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtlilldtfz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.wangdashe.top/gtiazidpuw.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtxejqdhnq.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtdrrhyrum.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangtech.top/gtshrppukm.html

Go:   json.Marshal(obj)
来源：http://hz.svipenyu.cn/gtgxaslkwt.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtsdcsicqt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.52xcode.cn/gtdizphcba.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtefoneyey.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtkrrhbrik.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.tianlin.xyz/gtcfvozqli.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gthugesdeh.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtjgmginxj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtskrvlpyc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.svipenyu.cn/gtqlupgwco.html

Ruby: JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtlvpmgewt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtbtyvcuxv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guannengcc.top/gtrbcihkdu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtkeczjzbj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtxjrjdafy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.haohaochexian.top/gtaoqfbjjj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hysaishi.cn/gticntxrqc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tian-w.cn/gtjhrpczhx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jiagoushi.top/gtwhxwiipb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gthyjtvuix.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtatnkrgef.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtiaxasikp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtvxoynpyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtymozaizn.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jiagoushi.top/gtaxzcntum.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.52xcode.cn/gtiespghbh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yvedp.cn/gtihqakusq.html


<!-- 参考信息 -->