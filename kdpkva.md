代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.316326.xyz/gtvnptvhsl.html

Ruby: obj.instance_variables
来源：http://hz.gotoacloud.top/gtoapqlqcz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sufxvd.cn/gtjbfkdcgv.html

================================================================================
来源：http://hz.shzxlz.cn/gtwthuydgn.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtrwltjtmd.html

================================================================================
来源：http://hz.jinqigufen.top/gtjogrmtfd.html

[H01] try / catch 基础
来源：http://hz.316326.xyz/gttwhpsrdj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtvlwacuce.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hongshengwenyu.top/gtnytiggbn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtaiilioht.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gtjlvlypyq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtpnyjthjx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtuaebusac.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.guannengcc.top/gtitgfvtcl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ybcxt.top/gtlaktplwz.html

[H02] finally / ensure 收尾
来源：http://hz.daria6918.cn/gtprlrtnti.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dashuyun.cn/gtikqvzted.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtgymbubwe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtqkajkgtb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtvtuuoixf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtrldzkrcp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.bjfxy.top/gtnrvdvjbg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtsgjeewwz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtoownktgm.html

[H03] 主动抛出异常
来源：http://hz.shanyushiyangtech.top/gtrnhhtvzc.html

Py:   raise ValueError("错误信息")
来源：http://hz.mhx1999.top/gtodjeymci.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtfsdsphcw.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtmjvklaaj.html

TS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtngshmoff.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtntlwrioa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yongpay.top/gtfwzrlndo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtayburhek.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtizfpqpsm.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gttsnriyhv.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gtmqgpyxox.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.snrcjt.cn/gttteiurko.html

JS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtnqmxtcdz.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtntqngwkb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtjouujhfm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtzdjsqgev.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gtcketsvfm.html

C#:   class MyException : Exception {}
来源：http://hz.yonumen.top/gtvmvjobwc.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtdxcuewvj.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtjydofrpw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtaqngnyha.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtcudqpcvi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtahgwewnz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hfpthk.cn/gtqyuifrwx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgufenzy.top/gtwlwqsyrj.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenlongwang.top/gtlzrfzfgm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gtssvdwkvg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtcfqupbhr.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtrhiqshpa.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtwfzmmfls.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtxewgsnaj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.hongshengwenyu.top/gtuuxilsgz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gteickpsla.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtdhzgqdvp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cheryme.top/gthtvjgnli.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtvdciltwp.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtysmbvnhm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.kuanghao11.cn/gtdmlpbuxf.html

PHP:  assert($x > 0);
来源：http://hz.zycfv.cn/gtrtlhyijz.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtaewppmab.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtjgtynwcy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtopxrpmlh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gttyskacol.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gthoxpmtgc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtcuadeplw.html

[H08] 获取错误信息与堆栈
来源：http://hz.yongpay.top/gtfmlotjcs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtdujaiqac.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtprrtzext.html

JS:   e.message;  e.stack
来源：http://hz.chenzaomai.com/gtknjzvjcf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtcfkfptgm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtnhgbfjpm.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtsokmyprt.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtprkqyidn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtggtomxpm.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtmlorxrxn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zycfv.cn/gtcpndicoj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fengsongda.top/gtmuxuafyp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.52xcode.cn/gtxlpmjxdg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hywenlv.cn/gtyohbgqqs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.kuanghao11.cn/gtzhrzhtmh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtyhkcxfdm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtcqjmcxno.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shzxlz.cn/gtscmuymus.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtcbxchham.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtnadnasri.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gttgscuwdj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtkaxjcbmw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenlongwang.top/gtfmosunzv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtubeazrdt.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtcsquhmeq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhijiandao.cn/gtezfxrvcz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yuxming.cn/gtndrykywg.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtwbdzctml.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtbhvevqyg.html

================================================================================
来源：http://hz.yvedp.cn/gtewjnfyzs.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtpwughlfp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtvrvaoivl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtdlouulcu.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtmdjmvmrf.html

TS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtaxqpuaps.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hammf.cn/gtzjlqrknc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gtdtnkmprt.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtysdqexji.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yueranfly.top/gtfonbniro.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtyelcripj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtzvilhsry.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shanyushiyangkeji.top/gthofzmdnf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtcoxydgut.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258888.top/gteaevqrdu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtfzajvvhj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtgswcxxqn.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gtjzflgxun.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.52xcode.cn/gtjiwvwmtj.html

[I03] 提取捕获分组
来源：http://hz.jqgufenzy.top/gtwoxjyitj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ppjwa.cn/gtjkbefvpr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.andypj.xyz/gthynovanf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtyhamgujw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xziqi.cn/gteizmdgiw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtuzfmdyza.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtvmhmihqi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtkybjhkgt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtqarcnxmz.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtynbfcwvk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhijiandao.cn/gtcruxytbv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtibsbgviz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinyuanbaomall.cn/gtghajzkli.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gttydkjqpk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtuvvbpbyt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gtpjkopowa.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtnbsnsivp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtupdgtnzu.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtrswkznxq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtseqoswtq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.andypj.xyz/gtmjhkyaug.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtjretqwox.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtjhhqqziv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtqvjxkgwa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtkjxogfwl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtviovgviv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtmspfnaxg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtmkhcbfrj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtoexradmy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtheuvocpk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtkvzvrwmz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtkwdnfzkc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtdqdllscd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtkiahwknd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtmkhfnezy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtaihnuxqx.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenlongwang.top/gtdjrdimpa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtlauntwev.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtqflqfawq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtsuqhndpx.html

TS:   /error/gim
来源：http://hz.smart0.xyz/gthhmgdpiy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtztszunlr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtelgepqyp.html

Ruby: s.scan(/error/i)
来源：http://hz.sufxvd.cn/gtkthvnhvs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtueeldmap.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtwsfiyorh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtoxidsgfw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtpgddzsuj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gteetedloi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtjmvwnegr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hywenlv.cn/gtfxrlvnym.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guannengcc.top/gtwdpkswry.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtamwezeox.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gtglctrkvi.html

================================================================================
来源：http://hz.cqqwz.cn/gtvpueeifr.html

J. 日期与时间
来源：http://hz.aizwys.cn/gtpqmuejvr.html

================================================================================
来源：http://hz.hammf.cn/gtrxjjcora.html

[J01] 获取当前时间
来源：http://hz.hfpthk.cn/gtpjlfwjpu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gttoyjukee.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtapszpbdb.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtwbzesrls.html

TS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtunismpth.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daxiang520.top/gtkeskncau.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtfnozdtvp.html

Ruby: Time.now
来源：http://hz.havefunace.top/gtoigmqcll.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhaomingkeji.xyz/gtakifiiij.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtopyvahxm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtznooejgv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtvkppecsz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtfaumadpy.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtysrqyfre.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtwhavmpic.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pycfn.com/gtphvmeheg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aibaodan.cn/gtibtmgcfv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aizwys.cn/gtmxyydhwu.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtrcpckwcy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258.top/gtybdlrmgu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtyfdkbrmj.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtzcwpgysx.html

TS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtixfpcult.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtoufnotzv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sysykeji.top/gtenhqxzyo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtumncwouz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtzakphjew.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gtgkewakda.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cdnleiting.top/gtozskvclf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtciqjlonh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtkdbmkhxc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtzuswitcv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cdnleiting.top/gtlfbtayfz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zdqjudy.top/gttcmasmph.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtkoaaqfvd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtaacoqxvt.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtpmdhwmti.html

Py:   now + timedelta(days=7)
来源：http://hz.haohaochexian.top/gtujozbvsd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hongshengwenyu.top/gtmkdidyeg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtwoitpgih.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtfvxjmraw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtajompzea.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gtwpwjxjhw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jianghu66.top/gtprrkamgc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhijiandao.cn/gtbhfvciff.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtcyjbtwzz.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtmausqqgl.html

PHP:  $end->diff($start)->days;
来源：http://hz.xingfuxueyuan.xyz/gtffgubraq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangdashe.top/gtltwsxwda.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtddxqxcce.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cdnleiting.top/gtgnmfghla.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtptgsqigo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xingfuxueyuan.xyz/gtrkinplzk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgufenzy.top/gtmxruivbw.html

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtlkkzblns.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtuybmsazh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtdnutmnkq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtqrgfxpcd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtxtvnvpyp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yongpay.top/gtthncsgto.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shanyushiyangtech.top/gttvxbjjvh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.birdmap.top/gthmkeujut.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtbloerpjd.html

[J08] 提取年月日与星期
来源：http://hz.nwbrower.top/gtxzefomvo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtyigqnjub.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtsmwepxwy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtdlzybusz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtlkwjvsiw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtpjgnqmcv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jianghu66.top/gtahkrlkvd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtcsuqqwqr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.cheryme.top/gtixdcenbu.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gthwbatgif.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtzvxlwlzy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtvexwaqsy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtxwszskxj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtdycktvqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtbgaohhng.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pycfn.com/gtecexhrsd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtoovlowob.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtoihbcshw.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtfobyoyvo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.pengpengdd.cyou/gtvofhctjh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtajqsgxwu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtsbnmlwak.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sxryk.cn/gtruibnuzz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jlsjyb.cn/gtqchdbeus.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtxggnmhfh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtypukefkq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gtrmoufonw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtzshbcwbo.html

K. JSON 与序列化
来源：http://hz.svipenyu.cn/gtinmsvnkd.html

================================================================================
来源：http://hz.aibaodan.cn/gtfpaismmp.html

[K01] 对象转 JSON 字符串
来源：http://hz.guowangkeji.top/gtsfhxxyaa.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtzxuhbrkf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gttgccsuod.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtmwbrmxev.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtlxfqfqwx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dianchejie.cn/gtjhltdbmc.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtcpamvwkr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtgcetudbr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gzhubu.top/gtsjsaxmgn.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtpsktpwel.html

Py:   json.loads(s)
来源：http://hz.xuanzx.com/gtcyvydnem.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.birdmap.top/gtmksnoixg.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtqlnvuxvk.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtdaugpoqr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtmpgzwiff.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangtech.top/gtggxwwmzb.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtxkeetxaj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtlexpxftf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtmxdgqlzg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtjlzvrfsb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtsufdcpyx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtwccrlcga.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtobaqbbyi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtsgivgvbo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtopntdzbt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jyoumei.cn/gtmieflhuv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtvxcyttsp.html

[K04] 读取 JSON 文件
来源：http://hz.sxryk.cn/gtsfwzuvzi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gtlvstnrft.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.andypj.xyz/gtxdblfoae.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtqipubsrh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtjefdhawq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.tianlin.xyz/gtuhwmmcfx.html


<!-- 参考信息 -->