代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.iojbl.cn/gtslnmgniq.html

[G15] 枚举
来源：http://hz.yanxiufei.cn/gtoccmjhiy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daxiang520.top/gttltwzzrg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xylfe.cn/gtakgsthix.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.tian-w.cn/gtnyzmtqrt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuxming.cn/gtihmjljql.html

Java: enum Color { RED, GREEN }
来源：http://hz.xuanzx.com/gtapmgfmar.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ybcxt.top/gtrfathidw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sweek.top/gteudldetk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtfhwcdqtu.html

[G16] 对象转数组 / 字典
来源：http://hz.yonumen.top/gtxlkpbgvm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tian-w.cn/gteijjrcpo.html

PHP:  get_object_vars($obj);
来源：http://hz.zdqjudy.top/gtilffmqjd.html

JS:   Object.entries(obj)
来源：http://hz.redwolf501.top/gtruznzxqr.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtbeerozrm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtvbvcjbzl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xylfe.cn/gtaaivlcgg.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtuwejcmvt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnxiangtu.top/gtyflwkoyn.html

================================================================================
来源：http://hz.birdmap.top/gtznljjhss.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtpudmdixa.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtnbrwybxp.html

[H01] try / catch 基础
来源：http://hz.zhongyouzk.top/gtmnenlnci.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtmeelenil.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtrnvxfbpm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtkrxnctvg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtlimfcdez.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jiagoushi.top/gtadctszyf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.fengsongda.top/gtlccdkbyu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtckziakav.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hammf.cn/gtxsgnraqj.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtskbxhpoo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ivvv.top/gtoakvrrlh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtkrrqeecx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtvwodggnn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtdihoeukw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtfibzxfsq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgufenzy.top/gtpddqxhkz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtrgbtmpzk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.haohaochexian.top/gthpdqphza.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtqfdjlrnb.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gtifnrdgel.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.redwolf501.top/gtxafvbaac.html

JS:   throw new Error("错误信息");
来源：http://hz.chenjidiqi.icu/gtpjxytnsa.html

TS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtrgqslhrd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shangyingyoupin.top/gtbbnxwuay.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtpajjwarj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtizkmffbk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtqjiqbkmd.html

[H04] 自定义异常类型
来源：http://hz.hnxiangtu.top/gtbnconlbj.html

Py:   class MyError(Exception): pass
来源：http://hz.hnqzz.top/gtrcfyvpwt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtbspllwio.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtkodwcfjq.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gttwmrupeg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtgmdiefek.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtxzbrxnks.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtyrtkadjg.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtaavccwlj.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gthpyijwpt.html

Py:   except ValueError as e:
来源：http://hz.quarkkingdee.top/gtotuzldlg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gttdcmdelk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtszxpelbv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtdnklyrfg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtykmjvsvl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gttbpjrizc.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtqpeizsvx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangshuangyany.cn/gtmdpmgcqf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtdktuwnlm.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtpsuoleal.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtpwslizui.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtbpkgifug.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtfgbjfzey.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jiagoushi.top/gthtyqzbsw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gtrfrgwepd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtvpfoodnq.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtbgtbvmfl.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtcyqtzapf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtaeflbxka.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gtiokzleot.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtihddcmyx.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gtcrqvzvbj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cqqwz.cn/gttvtprkla.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtmjgwkent.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtgxuapbkc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtkfrhudyn.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtjxfhcgyp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigfzy.top/gtsreokgbs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sweek.top/gtagwewzzx.html

JS:   e.message;  e.stack
来源：http://hz.yanxiufei.cn/gtunvyjyds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtdwvqqhbn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtuaspdukh.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtzwlnlftl.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtluaumodk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtybloinjh.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtrxxioqyk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtmwgpyaht.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxuanxn.top/gttuaemszp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xuetiantiany.cn/gtondvlrlq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.guowangkeji.top/gtprlzdbms.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtfoiorkwm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgufenzy.top/gtsabxsenb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtcxfggige.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gtbziwkjvj.html

[H10] 资源自动释放
来源：http://hz.xylfe.cn/gtwdpacmqe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtlwrjbbes.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtkqmhmkgz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtjzqejtmb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtqskalplj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtppjqoapm.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gtirhpuzob.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtceumwatj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.iojbl.cn/gtocyznnjy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtltptpxlm.html

I. 正则表达式
来源：http://hz.havefunace.top/gtoxxggufe.html

================================================================================
来源：http://hz.cdnleiting.top/gtuygirugx.html

[I01] 判断是否匹配
来源：http://hz.jinqigufen.top/gtilpforfa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xinyue.icu/gtkyusduyk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.andypj.xyz/gtwtyagpkg.html

JS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtdechwnbr.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtfvjudycz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gttnviwskg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258888.top/gtfidmrtbj.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtmcfsusoc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zdqjudy.top/gtttishivp.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtczklunjf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.redwolf501.top/gtocbswxtt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtmzjlpihz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtfokosoye.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtwjosihfu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtjbgoqojl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtrqphphhq.html

Ruby: s.scan(/\d+/)
来源：http://hz.havefunace.top/gtgsvbujkv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtklienjlw.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtikwvufcw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtsxkrbdug.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtmtaoqxkg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gttjmeesgs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.316326.xyz/gthugyooxv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtfietkiph.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtgstieaew.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtfoencvmh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guowangkeji.top/gtftkznptt.html

[I04] 正则替换
来源：http://hz.iojbl.cn/gtiijzvnfi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtewovqjov.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtmxcdibzy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtjxmqcqwt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtbikbpeob.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtcdxsogxd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fzhhl.top/gtnqhmayyf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ybcxt.top/gteenyxxpr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gogol.net.cn/gtffyygayx.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtlqkaadhp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ydzc1.top/gtioykuliw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuanzx.com/gtqhmtpuzu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtipmicaci.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinghuilouyu.cn/gtssxkmonz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gthqjiifqu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtzlvgjqte.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtjskcmzas.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fzhhl.top/gtdzycjwqs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gtwaawvfen.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtjespcajh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtvmzfjcwc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtlcetmrsf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.meibo888.top/gtdlcombzs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hfpthk.cn/gtxecstczc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhiwuduotai.top/gtuqkblvjo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.316326.xyz/gtvxvuboti.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtvjdjrzqv.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtepaermip.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gtojyklclk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.c1oappe.top/gtqjcbdvim.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtgroqdzec.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtgrfnwtgy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtubtysycw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtylxkjcda.html

Ruby: s.scan(/error/i)
来源：http://hz.sxryk.cn/gtbpnvihik.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxuanxn.top/gtvujsjwea.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuanzx.com/gtyjvgjkzl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cqqwz.cn/gtegkmxmgl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtalxljoyc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gttegqiift.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtlvaidovu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtikxileqa.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtjeyputyo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.iojbl.cn/gtwunmtloc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtjbacxsnt.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtznhcafyy.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtyztsyobd.html

================================================================================
来源：http://hz.hnxiangtu.top/gtthozcqyg.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtxsizoert.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtcyvlukzl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtvxsdjous.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtuifrtvue.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtuxkqeyzb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtrjbzaluc.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gtfjpoamkr.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtnymgvtnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hfpthk.cn/gtguktjaru.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtpoimsyej.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtdimjotfx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtdeohsheo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gtvgctuqge.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtzanuvbar.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtlolbogup.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pycfn.com/gtbimeoaoe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gttwvtwsrf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtcwovnhit.html

[J03] 字符串解析为日期
来源：http://hz.shuidangran.top/gtflrbzifq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenlongwang.top/gtyrnkdmnj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtxombzsdm.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtnfoxafvo.html

TS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtgtwczjmg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtsvmpseks.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtpfzaflnu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtcipnuobz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtxgenaaxf.html

[J04] 时间戳与日期互转
来源：http://hz.birdmap.top/gtngpcaszt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daria6918.cn/gtqstlzgrh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtpedwmxgt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ybcxt.top/gtmwiffsqs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtnyuuyyit.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtppteyyzd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtyujpgrwp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtoahoxbvg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinghuilouyu.cn/gtvolluexr.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gthuvuzvvm.html

Py:   now + timedelta(days=7)
来源：http://hz.havefunace.top/gtsbpilpyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ywan-chungtsiang.top/gtlgeeykwa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtdztmgtbh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtqmaoooch.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtjwmbqmge.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nanxinkj.top/gtehouhvlk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtlkrmngwf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.dashuyun.cn/gtauldabzi.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtunitesvv.html

Py:   (end - start).total_seconds()
来源：http://hz.xinyue.icu/gtyucodcza.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinqigufen.top/gtctkncuam.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pengpengdd.cyou/gtguijtbhy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtjbhxfljy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.wangdashe.top/gtrztshktn.html

Go:   end.Sub(start).Hours()
来源：http://hz.hfpthk.cn/gtuititjaw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtlhrujigc.html

C#:   (end - start).TotalSeconds
来源：http://hz.jyoumei.cn/gtuwivuwvd.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtjdretdey.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtzwqrbbpl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sxryk.cn/gtwholhygk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gtftmcqtfg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtdkcibqch.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.chenjidiqi.icu/gtnxjfbedz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hywenlv.cn/gtnoxcttit.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gthhaghrrq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtlimfploc.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtwtojcswc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtpzbkkoom.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yangfankeji.com/gtznjkbrxc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gtordtzulr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daxiang520.top/gtxzpckfxn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtzlavjyjm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zycfv.cn/gtguzimyzg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gtydhlrmnu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gtludoqpfi.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtebbbewaw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.bjfxy.top/gtlllppnyk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinghuilouyu.cn/gtwzslxhvu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtozoipqqo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cdnleiting.top/gtmwgzsbhz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xuetiantiany.cn/gttvftqgai.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj202588.top/gtpbhtdrkk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtuilkyoxi.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gzhubu.top/gtycdmiqnh.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258.top/gtanapngnz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtfjjkwfzf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhoulong.xyz/gtqaiaepsn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtgufxfbse.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtlnezqihv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yangfankeji.com/gtyueltorp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtuypemrly.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nanxuanxn.top/gtquognpzs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtmydlaafp.html

================================================================================
来源：http://hz.0kj1m.cn/gtgwbaokkx.html

K. JSON 与序列化
来源：http://hz.ydzc1.top/gtnjymfozr.html

================================================================================
来源：http://hz.yj20258888.top/gtfropkgmb.html

[K01] 对象转 JSON 字符串
来源：http://hz.vqdsnc.cn/gtxxuxtmtk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtplmarync.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtlhvhxyyi.html

JS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtxxbkqbfh.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtwjyyboyp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtlcpoymcc.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtnihanjpl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gotoacloud.top/gthbspslzh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hnqzz.top/gthhtnvagh.html

[K02] JSON 字符串转对象
来源：http://hz.cucudq.cn/gtijcialac.html

Py:   json.loads(s)
来源：http://hz.hammf.cn/gtrmencemh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yongpay.top/gtlrggorie.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtgtmbsxuw.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtiauousid.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.bjfxy.top/gtdmdflioj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtcbsblrql.html

Ruby: JSON.parse(s)
来源：http://hz.vqdsnc.cn/gthviznulo.html


<!-- 参考信息 -->