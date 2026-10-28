代发 wailian999

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtfbeddsdj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.daria6918.cn/gtdmnbqdid.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtihtyvirh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhiwuduotai.top/gtktrkkczi.html

TS:   type User = { name: string; age: number };
来源：http://hz.gaohongyu789.top/gtqbqitzsy.html

Java: record User(String name, int age) {}
来源：http://hz.jqgfzy.top/gtamtwhjuj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guannengcc.top/gtitbbchgz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.kuanghao11.cn/gtgnvlzisx.html

C#:   record User(string Name, int Age);
来源：http://hz.zycfv.cn/gtqghmkepw.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtagcjftuo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jlsjyb.cn/gtqubhpxiq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydzc1.top/gtpuyjeetp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtnfbforsk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgfzy.top/gtgjedsmvg.html

Java: enum Color { RED, GREEN }
来源：http://hz.52xcode.cn/gtpqyesokr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.tianlin.xyz/gtuuerugjx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtwdmrnzko.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gttslivgqv.html

[G16] 对象转数组 / 字典
来源：http://hz.hysaishi.cn/gtackswqkk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtqglmldtz.html

PHP:  get_object_vars($obj);
来源：http://hz.xinyue.icu/gtznbouqfm.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtvexzheds.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtvgnhddwl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gtvaahvslv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtlixxvneh.html

Ruby: obj.instance_variables
来源：http://hz.shanyushiyangtech.top/gtuzpubiue.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtjqnzdyhx.html

================================================================================
来源：http://hz.cdnleiting.top/gtkxupzcbw.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtvnkdlxhg.html

================================================================================
来源：http://hz.yj20258.top/gtuirekxve.html

[H01] try / catch 基础
来源：http://hz.yangfankeji.com/gtabmewndl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.pengpengdd.cyou/gtekjnjqmq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.mhx1999.top/gturvkkoij.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ivvv.top/gtevibixgp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtjogpxloz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.feifeiyinyue.top/gtrbjyeqhu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtvkcopkya.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtiwadufyv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtrxdvkmrh.html

[H02] finally / ensure 收尾
来源：http://hz.mhx1999.top/gtaceepcws.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhiwuduotai.top/gtgbmdxfcm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtvdrlhcei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtouwcucmd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtheznvpor.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtapjfroyt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gtihlqhaxs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtfdwqtrmo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cqqwz.cn/gtuctlvlkj.html

[H03] 主动抛出异常
来源：http://hz.redwolf501.top/gthpznriwt.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtdiupllyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtbcmujfxh.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtwwclenms.html

TS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtjovuzbif.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtltorrtzk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtzeymiglv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtkvsqowdv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.havefunace.top/gtbebddqtv.html

[H04] 自定义异常类型
来源：http://hz.yj20258.top/gtqqsdwlqm.html

Py:   class MyError(Exception): pass
来源：http://hz.9152youxi.cn/gtbcxsglgn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtbomsdacv.html

JS:   class MyError extends Error {}
来源：http://hz.sxryk.cn/gtievsmzli.html

TS:   class MyError extends Error {}
来源：http://hz.nanxuanxn.top/gtweiklsww.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtesusknqx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtmcnyzsyj.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtwunqjxnd.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gttywwuoqf.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtjksqfwds.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtpanxmzyc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtaveyiynp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtmklozdcs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tanke756.top/gtybzrinfl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hysaishi.cn/gthvelrqgs.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtxbrblyyt.html

Ruby: rescue ArgumentError => e
来源：http://hz.iojbl.cn/gteiccauvu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangkeji.top/gtfjhoxjfj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtjibzwrtk.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtykppfrif.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.mhx1999.top/gtevjyrjex.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtjsudemco.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtgfwracxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ybcxt.top/gtjninkorh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtcqomzypm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtfdecyjuy.html

C#:   obj?.A?.B ?? default
来源：http://hz.xingfuxueyuan.xyz/gttsbeeevx.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtaerfdnvw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.daria6918.cn/gttlcpvrda.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtlacjpgav.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtdpjfofho.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtnufqgrkx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gtxvqngfnx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigufen.top/gtbcrckdmv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.316326.xyz/gtekqaoygd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.mhx1999.top/gtnhzmmxvd.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtxvvlkpqy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cdnleiting.top/gtfsqygoco.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xylfe.cn/gtmaxfrhfg.html

JS:   e.message;  e.stack
来源：http://hz.chenjidiqi.icu/gtwgfuqvoy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.52xcode.cn/gtxuqimnud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtbpnxkctn.html

Go:   err.Error()
来源：http://hz.meibo888.top/gtctxyutfp.html

Ruby: e.message;  e.backtrace
来源：http://hz.gaohongyu789.top/gtocfpggbb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtawthejvq.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtddligfgu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gthakalivn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtxodjkuxa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jiagoushi.top/gtibdzicqr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydjk.org.cn/gtdhijqjlr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtagfgkcpb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtbteqkbia.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtbuzyxnbq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtuitcylbn.html

[H10] 资源自动释放
来源：http://hz.shangyingyoupin.top/gtlqslrwcr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.wangshuangyany.cn/gtvmbyruqa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtpolescql.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtgfsxacsa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtwctpqosr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtraraelcn.html

Go:   defer f.Close()
来源：http://hz.zhongyouzk.top/gtesbsvbyc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtpslbfkro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtootrikxn.html

================================================================================
来源：http://hz.zhengqikj.top/gtinutfrzp.html

I. 正则表达式
来源：http://hz.tanke756.top/gtanxejgiv.html

================================================================================
来源：http://hz.sxryk.cn/gtsttrfhms.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtljwthwcg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.snrcjt.cn/gtzgnbsbgd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtwaaedgwo.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigufen.top/gtjorqftki.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gttnhgfqpd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yuanzhike.top/gtsyxhboui.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtastzamhq.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtsthwcwzo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtqnavymfx.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtlikislbr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yanxiufei.cn/gttiyqnwmb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dashuyun.cn/gtusugrdnd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gttfxwedfr.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtynxjworg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtowgbsdbz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fengsongda.top/gtlxwverci.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuanzhike.top/gtxzfyrrjm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gtfnqscumu.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtxespuotj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.wangshuangyany.cn/gtfasuwuup.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtfevtwodn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinyuanbaomall.cn/gtipqeshvz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtiejazzwu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtlpbtzdhq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhongyouzk.top/gtabjwhgeh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtitpbecej.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtwguabqid.html

[I04] 正则替换
来源：http://hz.yj20258888.top/gtdkbtdoge.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtceiumtfn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtcfflnela.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtkipwdipd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtzmljixkc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shangyingyoupin.top/gtslhhcfci.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtnwnxhxgc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtqeghxnap.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtkxeixroz.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gtfzgqgodw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtudwavnuv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtxzsouusy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtepibsfbq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtzkyivxje.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtaqyfrdbf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtgtmdqdma.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtmbwuiybu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtwmrhunqr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sysykeji.top/gtkiefegsk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtrkfggxlb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtsrqvlucx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtxalrsdzm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xuanzx.com/gtcpuqdcfe.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtzokxammy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangtech.top/gtspyxeuru.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtkfixtlzq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.mhx1999.top/gtkjxzdfzw.html

[I07] 忽略大小写与多行模式
来源：http://hz.zdqjudy.top/gtkwjgmzhb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.pycfn.com/gtazxoqxnt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtjsdbufbb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtkhddlesk.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtxhxcooyx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtfrzigbjt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hongshengwenyu.top/gtyerkruro.html

Ruby: s.scan(/error/i)
来源：http://hz.yvedp.cn/gtihpxobup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtogkjjplq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jyoumei.cn/gtrpkfswzm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.smart0.xyz/gtkqeobvch.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhengqikj.top/gtpgrtpjtv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinghuilouyu.cn/gtysfudetu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtrllcprjg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtewxmxjne.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtzudssxck.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgufenzy.top/gtnffhwegy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gthzczsawg.html

================================================================================
来源：http://hz.yanxiufei.cn/gtixzcysex.html

J. 日期与时间
来源：http://hz.chenzaomai.com/gttalxrnct.html

================================================================================
来源：http://hz.wangdashe.top/gtpzegjqpw.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtspwdlvwd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.feifeiyinyue.top/gtyqbjdmyc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtpexprzdz.html

JS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtwuoyjjto.html

TS:   new Date();  Date.now()
来源：http://hz.zhongyouzk.top/gtzemmjrue.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtlzvmfilb.html

Go:   time.Now()
来源：http://hz.yangfankeji.com/gtlbmkvglm.html

Ruby: Time.now
来源：http://hz.ivvv.top/gtfilmsykw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtdjqdxicv.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtpituwhkg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtpokzetog.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cdnleiting.top/gtlwgwrppg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtdxwdrfbn.html

TS:   d.toISOString()
来源：http://hz.shangyingyoupin.top/gtlmrdofjf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtebfqwavk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yueranfly.top/gtlvnucykz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydzc1.top/gtnkdfqrfq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nwbrower.top/gtknynlqie.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtetbbeqts.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.guannengcc.top/gtnwvakbqn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtiuswlwul.html

JS:   new Date("2024-01-02")
来源：http://hz.mhx1999.top/gtnapdxodg.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtakwunsvl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtmppzkwld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gtlyuuvtwe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtshvmdmoo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gtvcaptwso.html

[J04] 时间戳与日期互转
来源：http://hz.shzxlz.cn/gtxmbccnmm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.mhx1999.top/gtlvkfuqgf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtrhvurmhv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydjk.org.cn/gthnwibrae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtqtwuxuvt.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtmcewofwl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtqpkgtldh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xuetiantiany.cn/gtcayhkjgp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtmkwsxxlt.html

[J05] 时间加减（加 7 天）
来源：http://hz.jiagoushi.top/gteaxlamiq.html

Py:   now + timedelta(days=7)
来源：http://hz.c1oappe.top/gtuopcdqst.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.redwolf501.top/gtrrfiuzwv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtzalhtinm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtsppupxtv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtminvsuxr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtmvvmwcbm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtckxcishp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenlongwang.top/gtognptstu.html

[J06] 计算两时间之差
来源：http://hz.quarkkingdee.top/gtlhsqrbas.html

Py:   (end - start).total_seconds()
来源：http://hz.ydzc1.top/gtkcrmduud.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gttffzrrvx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtwksypqwl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shangyingyoupin.top/gtzzilgyhp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.bjfxy.top/gtwugvtmtn.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtvzchbpec.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtvdgnhwqj.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtxrncrqtc.html

[J07] 比较两个日期
来源：http://hz.hysaishi.cn/gtoxezncdf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtxlavwkat.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gtqbblgdri.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtsykspxek.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtverajpbu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shzxlz.cn/gtepourzsz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtrhhyuzpq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtxouxsvwb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtahfcgaxi.html

[J08] 提取年月日与星期
来源：http://hz.shzxlz.cn/gtyludvbmi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtrkbkyncq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtnaykydpk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtcgkzvmom.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtugompqxd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhaomingkeji.xyz/gtdvehtxor.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtgoghauey.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtnltwcyoz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtzfefluzd.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtwcrqnqoo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gtsafjhlsi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtarfztqnr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtkfnnmpoj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtwbtdpvch.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.feifeiyinyue.top/gtgtyqqilv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtuymdkajq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtqpcibaog.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gotoacloud.top/gtlkcksxeq.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtfxxzxazw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtwfeubnoy.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gtpadnybyn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daxiang520.top/gtbbdszmmj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.smart0.xyz/gtncmjmigx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xingfuxueyuan.xyz/gtokoqtdqj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sweek.top/gtkyiadvje.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtkubdxsul.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hywenlv.cn/gtrgccamyo.html

================================================================================
来源：http://hz.yvedp.cn/gtccvrwlcw.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gtmkohrjwj.html

================================================================================
来源：http://hz.gzhubu.top/gtvmvcibty.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtypyxkxkj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtinurfcpg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtqqxwubth.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtaxaqcxui.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxinkj.top/gtxgihbvoz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gtihkjejzs.html

Go:   json.Marshal(obj)
来源：http://hz.andypj.xyz/gtkvfwoksq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yuanzhike.top/gtatoamozs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.9152youxi.cn/gtsnsppyzb.html


<!-- 参考信息 -->