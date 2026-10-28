代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gthogjxxix.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtvvchgmfj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtoktquaqv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtlmvqwowg.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtjwsnnlbj.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gtrxdtoaez.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtvwejptue.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtlldmxose.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.haohaochexian.top/gtlfupodae.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.fengsongda.top/gtuxxwjqna.html

Java: enum Color { RED, GREEN }
来源：http://hz.gaohongyu789.top/gtklvoeavm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigfzy.top/gtitlydixw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtapqwjmvw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtagdfvqkf.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtqueuhfne.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinqigfzy.top/gtptnvsygy.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtlrobyvif.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtlagluhbw.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtkslhfnex.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.wangshuangyany.cn/gtsdahzltb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gtqevkpwjl.html

Ruby: obj.instance_variables
来源：http://hz.yj20258.top/gtqjzqkhtp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258.top/gtxvbrwcgw.html

================================================================================
来源：http://hz.zhoulong.xyz/gteieeannd.html

H. 异常与错误处理
来源：http://hz.shangyingyoupin.top/gthirukuzr.html

================================================================================
来源：http://hz.guowangkeji.top/gtcrkhlkfl.html

[H01] try / catch 基础
来源：http://hz.hongshengwenyu.top/gtqpglsycs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gthnvgihlx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.meibo888.top/gtxpomhpkb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pycfn.com/gtitlcijzf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ivvv.top/gteyobqwsr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinqigufen.top/gthyaikzmx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zdqjudy.top/gtnysjmoxw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhengqikj.top/gtnqjusdcq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gtkjepbhzq.html

[H02] finally / ensure 收尾
来源：http://hz.sysykeji.top/gtcjwpmtik.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ybcxt.top/gtefjoneeu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtclybaxpg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtdptcojbq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gogol.net.cn/gtbwqlwcqx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtwskbrnnl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aizwys.cn/gtbraepvzt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtbedvjjjv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hnxiangtu.top/gtvwkxtann.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtzzbftcao.html

Py:   raise ValueError("错误信息")
来源：http://hz.redwolf501.top/gthntcarki.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj202588.top/gtwhcroaoy.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtgmcxlcpf.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtzgpngqic.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gthnekntcv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yongpay.top/gtvfngusdk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtucfcppse.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtoejwfnhg.html

[H04] 自定义异常类型
来源：http://hz.zhixingplan.top/gtddfaqvrd.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtedqrxoyt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hammf.cn/gtclqxgtsz.html

JS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtqzzruime.html

TS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtfwndabjg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtqnlmmmfn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtfabtemnc.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtljgyauhn.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gtwhhivnat.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtqlohoriy.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtgahofwxf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.tanke756.top/gtjnwhrndf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtyixehhva.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtgcfpfomz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtuwlbszbr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jiagoushi.top/gtsqfwkfxb.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtgdfvisnb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhiwuduotai.top/gtroanprlo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtvwvliqdq.html

Py:   value = d.get("k") or default
来源：http://hz.sysykeji.top/gtzvfietnb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gtjeoejxdk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtdaultjkn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydjk.org.cn/gtbbnckcao.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangtech.top/gtqarxsklx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gttbnjiycs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtcqfilmmn.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtovjcogcv.html

[H07] 断言
来源：http://hz.cheryme.top/gtdqordlrp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhijiandao.cn/gtgfupgkjq.html

PHP:  assert($x > 0);
来源：http://hz.shzxlz.cn/gtgueujqcz.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtnpfsflws.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtjisoftxs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtagtcsutl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zdqjudy.top/gtmdeiuwhm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gttwrclvib.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtqvxpcpig.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gttzxefzkj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenjidiqi.icu/gtvpxxdsxd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yongpay.top/gtgyarcwqz.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtamtchrxx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnxiangtu.top/gtjgskobha.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daria6918.cn/gtcotcqjyk.html

Go:   err.Error()
来源：http://hz.shanyushiyangkeji.top/gtjzhisxra.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtovrmpwgc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenlongwang.top/gtjdeecutq.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gtaivbgdog.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtmpuxjpvj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nwbrower.top/gtktjskxmq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtrzawlyip.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shangyingyoupin.top/gtscoqjgrc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yuanzhike.top/gtbuevyvwk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtnlplpczg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtkysrxfjp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtbagochlo.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtresyktbp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtmpxorpuo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hammf.cn/gtbmfvpdqb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtrdugexja.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtuptrjlwd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gtzjyqwrix.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtyxbyboav.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gtzeggrlyn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtulchwdww.html

================================================================================
来源：http://hz.daria6918.cn/gthzcuuzxg.html

I. 正则表达式
来源：http://hz.yueranfly.top/gtuawxgclk.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtzzklyjab.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangtech.top/gteegoptma.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtqkgrtepj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtilthdwkt.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtxrvruwvd.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtygibhvrl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtaaevavuj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtgkbmnypr.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtgvujevkr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtwesagbue.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtxleedehp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtpiyqnumg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gturnhnpyb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.wangshuangyany.cn/gtkbpkjawn.html

TS:   s.match(/\d+/g)
来源：http://hz.chenzaomai.com/gtpblzxdmq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtbkrcbbck.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhaomingkeji.xyz/gtkixemscq.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtznampdbc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daxiang520.top/gtcpfptdfd.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtjyukymwj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtwhbwdgop.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ivvv.top/gtexjihxbd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtutwtsnbf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtwemzbabh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtrvdcpqyn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.svipenyu.cn/gtdjexnymc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jlsjyb.cn/gtrnfrixiz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sweek.top/gtdecnvtns.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gtznachpmq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtvbizweau.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sxryk.cn/gtcgthqhjd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gtrpzpvoqq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.smart0.xyz/gtzcfbasub.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtjlpnznax.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtruimmcdi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtbmmiemfz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.aizwys.cn/gtnlahjnmi.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtgwwrqutw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhijiandao.cn/gtwvuvqsmu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pengpengdd.cyou/gtpqyaopul.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtnhuvargd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtqjubztxi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtjmjqkjjc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtykwieind.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtgbgbmtzn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhixingplan.top/gtajdlenit.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtafgphmly.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtzzyqrnwg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtincrxmsw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtwcolbckk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtnrlgsmdl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.svipenyu.cn/gtdwfznvtw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jyoumei.cn/gtmlgubvhu.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtdvmhzshr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtkmjscspw.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtkqrsatcu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtupxdbphd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.havefunace.top/gtuhbcynqu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtouifpcwx.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtbjtvpbys.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shuidangran.top/gtcocoettm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtvatbyavg.html

Ruby: s.scan(/error/i)
来源：http://hz.yanxiufei.cn/gtbyhnspkp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtvxephlel.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gtjshijgns.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cashguo.top/gtuyxhpgia.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtknrpceet.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtcwjqqdtb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtpwkmkeqh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtrqmzmyng.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yongpay.top/gtksuqsviq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtyvulwohf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtolxadakf.html

================================================================================
来源：http://hz.sxryk.cn/gtokvdfrez.html

J. 日期与时间
来源：http://hz.zhaomingkeji.xyz/gtyntcuein.html

================================================================================
来源：http://hz.xylfe.cn/gtektlyauk.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtxqddpzlz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtkgwhsvuz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtwtckifjo.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gthpgjhnun.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtqaujjdha.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jlsjyb.cn/gtbmxmvhms.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtyhgjvwnr.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtgfemhboc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cheryme.top/gtczxpwpaa.html

[J02] 格式化输出
来源：http://hz.guannengcc.top/gtagngmyyh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtqsojbpmq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtkpiovveb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtqfomkekh.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtfvnwfqgt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gthxcaelta.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ivvv.top/gtiaxbjwcr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtyxodujsb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtvdpvaldt.html

[J03] 字符串解析为日期
来源：http://hz.feifeiyinyue.top/gtvptlndbs.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xylfe.cn/gtmjmwhdlq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtramhxkcd.html

JS:   new Date("2024-01-02")
来源：http://hz.xylfe.cn/gtzsxmesov.html

TS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtosfjkjxy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtiezbzqzu.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yongpay.top/gtxsriwddl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtsboloyvh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtjwtkqsip.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gtxroehvuc.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtghcyuwwi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xziqi.cn/gtbgazqtzt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtgjcnkpdr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.svipenyu.cn/gtsvhnaamv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sweek.top/gtpycwvvwf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtklhqncny.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.quarkkingdee.top/gtfskafrir.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cheryme.top/gtcimlajua.html

[J05] 时间加减（加 7 天）
来源：http://hz.yangfankeji.com/gtasleioix.html

Py:   now + timedelta(days=7)
来源：http://hz.daria6918.cn/gtteuhymwf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtrnxokmmm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gzhubu.top/gthgrxgupf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtcfltjfcf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gtsakrendl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jyoumei.cn/gtddnpqhsu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtzbixfstx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtngzjdjwv.html

[J06] 计算两时间之差
来源：http://hz.ywan-chungtsiang.top/gthfrktriz.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtdnmthbrn.html

PHP:  $end->diff($start)->days;
来源：http://hz.zdqjudy.top/gtwkmcruib.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuanzx.com/gtyuznxdpo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtjkookpbq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtlkwhrbgr.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtfjhmsjhn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtalxrmypl.html

C#:   (end - start).TotalSeconds
来源：http://hz.kuanghao11.cn/gtghbpnbja.html

[J07] 比较两个日期
来源：http://hz.shuidangran.top/gtmwmfxgbz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtfajzgiir.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ehwqpu.com/gtkvrgicsr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gthjzrczyu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.andypj.xyz/gtlqyknozz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cucudq.cn/gtedwoinyv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cheryme.top/gtrqpmphfh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtoshnhotu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtiargfywe.html

[J08] 提取年月日与星期
来源：http://hz.gzhubu.top/gtjqhsuizx.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daxiang520.top/gtztinxbum.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangtech.top/gtvozijjjg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fengsongda.top/gtefrdnczy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtrgrlidmk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gthuabtyrl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.mhx1999.top/gtoglgwqym.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuxming.cn/gtbyeqbqlb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtsmpkpbup.html

[J09] 时区处理
来源：http://hz.ivvv.top/gtvukfbamm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.snrcjt.cn/gtljkwffgb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fzhhl.top/gtbngubxws.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hywenlv.cn/gtrylcwdkw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtyeslqegh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtudxskyhm.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gtqdurxxfb.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.bjfxy.top/gtqdvyjieg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.chenjidiqi.icu/gtbariaair.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtbpotptyz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtcayrdhvm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hammf.cn/gtcrnahkqv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.bjfxy.top/gtzjjgglwd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hfpthk.cn/gtbmynwohf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtayagdooz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shuidangran.top/gtcreltpuv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtjvrmbcwf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jianghu66.top/gtdfgfkdav.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtflryvgid.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtvtahgbrk.html

================================================================================
来源：http://hz.cqqwz.cn/gtbfpdcqqv.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtzqeseugn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtaryggxbb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtpusmbugr.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtzfdlcdfz.html

TS:   JSON.stringify(obj)
来源：http://hz.yongpay.top/gtydbpfkqn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnxiangtu.top/gtbhzxlwdd.html

Go:   json.Marshal(obj)
来源：http://hz.bjfxy.top/gtakzfnaia.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtdkglxaos.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtsgtkvahn.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtutmvtwdf.html

Py:   json.loads(s)
来源：http://hz.gaohongyu789.top/gtihpcdooj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtqggqhjpk.html

JS:   JSON.parse(s)
来源：http://hz.shanyushiyangkeji.top/gtxrgnhtze.html


<!-- 参考信息 -->