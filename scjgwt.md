代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenzaomai.com/gtuyvhexma.html

Ruby: def to_s; @name; end
来源：http://hz.feifeiyinyue.top/gthfdbrwwq.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtcohvvmfc.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtkhvesgxe.html

Py:   isinstance(u, User)
来源：http://hz.xingfuxueyuan.xyz/gtzepdzojb.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtavyownew.html

JS:   u instanceof User
来源：http://hz.hnqzz.top/gtkziyauar.html

TS:   u instanceof User
来源：http://hz.andypj.xyz/gtdywrgogq.html

Java: u instanceof User
来源：http://hz.cheryme.top/gtrznrqmqo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yueranfly.top/gtkhgaywrg.html

Ruby: u.is_a?(User)
来源：http://hz.jianghu66.top/gtvvjclaic.html

C#:   u is User
来源：http://hz.sysykeji.top/gtxeabiwad.html

[G14] 数据类 / record
来源：http://hz.xuetiantiany.cn/gtjlapmkgx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hammf.cn/gtuqjwwgtv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.nanxinkj.top/gtjhrpomtx.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jianghu66.top/gtitxytkov.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gtlkzozuja.html

Java: record User(String name, int age) {}
来源：http://hz.jlsjyb.cn/gtewnlfeqj.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yueranfly.top/gtqkpvkfqf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtkblvgnrm.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtprimnoff.html

[G15] 枚举
来源：http://hz.jqgfzy.top/gtmrzimqpw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.c1oappe.top/gtxpdkxxtz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258888.top/gtxuyirzku.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtpjhccoci.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtobxhlgdx.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtcgrbwpyj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtcnqcglzc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtinccfyyo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtxqablxth.html

[G16] 对象转数组 / 字典
来源：http://hz.yueranfly.top/gtzqelwktg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtvvenawhb.html

PHP:  get_object_vars($obj);
来源：http://hz.gzhubu.top/gtriquuwtd.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtszsnqhpy.html

TS:   Object.entries(obj)
来源：http://hz.yongpay.top/gtveayedml.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydjk.org.cn/gtanfdaani.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtkbjqrvvq.html

Ruby: obj.instance_variables
来源：http://hz.snrcjt.cn/gtkoesuqce.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtopefwkxf.html

================================================================================
来源：http://hz.zhoulong.xyz/gtzjqxydih.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gtctvnrold.html

================================================================================
来源：http://hz.dianchejie.cn/gtnimfbnes.html

[H01] try / catch 基础
来源：http://hz.jiagoushi.top/gtnsvctroe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinghuilouyu.cn/gthnkbcfje.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gttbeppzxe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.haohaochexian.top/gttjvjqvoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yueranfly.top/gtaltqpsvw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shangyingyoupin.top/gttifzmjeq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtksbkjfoy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zdqjudy.top/gttgrfvkwf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jyoumei.cn/gtxztpwzai.html

[H02] finally / ensure 收尾
来源：http://hz.zhoulong.xyz/gtfkoczmjp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xingfuxueyuan.xyz/gtqbzsghwb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtqpxlkmsr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtissaumwe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtkvxrkbqf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtchmmhqyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.redwolf501.top/gtmjbceqwg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ydzc1.top/gtwdutdaih.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtvpuflzvs.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtqwwihpmn.html

Py:   raise ValueError("错误信息")
来源：http://hz.cqqwz.cn/gttbpkkzkg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtipqblycy.html

JS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtgjgbqvcl.html

TS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtoxrqgkzt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtvtcazhve.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtnyudjgpq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuanzx.com/gtcratzeqj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtfwrgxkpd.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtqllegqrk.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtynjreusj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtthchbtpi.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtpsacexuf.html

TS:   class MyError extends Error {}
来源：http://hz.cheryme.top/gtvqplvume.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtadinriuv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.havefunace.top/gtcvecrubo.html

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gttvwqpnnz.html

C#:   class MyException : Exception {}
来源：http://hz.xingfuxueyuan.xyz/gtzlpalkhu.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtykbolpxy.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtjamciqhu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shangyingyoupin.top/gtfkedhgct.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtmfnpjnfi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtaggynqxa.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sweek.top/gtsqkyvscc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gotoacloud.top/gtthjmbajt.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhijiandao.cn/gtzasjbxxs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtoahofqvb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtviplaium.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtgbvabinb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.kuanghao11.cn/gtrokgghap.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yueranfly.top/gtgkkhswgo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtajiqukus.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhijiandao.cn/gtpepbgbra.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtecbhaelp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtbbbsbahd.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtmbtoxiot.html

[H07] 断言
来源：http://hz.c1oappe.top/gttcldpajf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtobbbmlkj.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtifdecpje.html

JS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtmbtcpima.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtvnvkorpf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtoqnvowek.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtbwkebecn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtwundlsnn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gtvfmgjsrs.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtanwdlhff.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xziqi.cn/gtrzgvrihj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtmurrucam.html

JS:   e.message;  e.stack
来源：http://hz.gzhubu.top/gtafsirrdt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtgptmyffd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yueranfly.top/gtsldwvwdv.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtbhiflawz.html

Ruby: e.message;  e.backtrace
来源：http://hz.mhx1999.top/gtumdmaybj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtthftbtiu.html

[H09] 带错误码的异常
来源：http://hz.andypj.xyz/gtylbwcfuh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhongyouzk.top/gthmcjjgqz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cqqwz.cn/gtydtyqbgf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinyuanbaomall.cn/gtqswyktvb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gzhubu.top/gtdewivopp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtmhqvgkoc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtzinzpzza.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtpuyfatrh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtjkbjwfqo.html

[H10] 资源自动释放
来源：http://hz.0kj1m.cn/gttmxyfeam.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtbfgasbhx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtafcxshoq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gogol.net.cn/gttbsletyi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtrrjoblkt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtkgmflkwh.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtabvfmkdv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtkovovfhh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxinkj.top/gtkahyjbpv.html

================================================================================
来源：http://hz.ybcxt.top/gtycnwxubd.html

I. 正则表达式
来源：http://hz.52xcode.cn/gthrwvprdi.html

================================================================================
来源：http://hz.haohaochexian.top/gtokjztobd.html

[I01] 判断是否匹配
来源：http://hz.pycfn.com/gtbqqmxpnz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtepvslmui.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtkoulhdwh.html

JS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtaapqniar.html

TS:   /\d+/.test(s)
来源：http://hz.hongshengwenyu.top/gtztxwzkxf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtnxthxdou.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sweek.top/gtazgwjlny.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtwzuaapko.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtisepavhp.html

[I02] 提取所有匹配
来源：http://hz.jinghuilouyu.cn/gtfkphywfu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.0kj1m.cn/gtdiuqvwfq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtryfeigkz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.mhx1999.top/gterjqszut.html

TS:   s.match(/\d+/g)
来源：http://hz.bjfxy.top/gtpuedtcfy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtyjesiarn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shzxlz.cn/gtyqcnihpa.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gtxrtwyzyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinghuilouyu.cn/gtylxailbk.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtdbjjqulx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtbfxjubtd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yonumen.top/gtjgzlckjz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtsdacjfpu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tianlin.xyz/gtwjhngbpv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yvedp.cn/gtvhfyteyg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gtqezgqhxv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.birdmap.top/gtoojkwtya.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtvjnblwrm.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtqbehhveg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hywenlv.cn/gtqfeufdrb.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.bjfxy.top/gtjywphxse.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtclxsimkr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtfoxbgjlf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gttdjlrdlo.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtgcekawnd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gterqzcdzt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtlievmgkv.html

[I05] 按正则拆分
来源：http://hz.yuanzhike.top/gtmlukakpr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yueranfly.top/gtphysihud.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtomdgnsjn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtofcmfeni.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtbsgyoydc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sysykeji.top/gtsieeggzo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangdashe.top/gtnjvtwuzf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gttyeocfez.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtzuefypff.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtujrcvppm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtqcergbsf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydzc1.top/gtydohzcsp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtrmgcphoq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gtjncrndfr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtcdlaxijx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.dianchejie.cn/gtffthtfxb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gaohongyu789.top/gtrrlkuqyr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtiffkmrqy.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gtehdvakwk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtdgehpuym.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtiakvnhjl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aibaodan.cn/gtczgwgjlc.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtcevdgkcw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tanke756.top/gtsiyejkup.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aizwys.cn/gtsyizauib.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gtkjgfwowf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhaomingkeji.xyz/gtiwcytizx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yueranfly.top/gtaeaejnfe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtocdgjfsu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shuidangran.top/gtenyuzrwz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtgmfxcrhx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtmyjrbpov.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtwwkaylls.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtsdunkzvx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtqebtrtwr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ivvv.top/gtepqkkwcg.html

================================================================================
来源：http://hz.yangfankeji.com/gtfwtxazge.html

J. 日期与时间
来源：http://hz.kuanghao11.cn/gtvxlwlqfq.html

================================================================================
来源：http://hz.gogol.net.cn/gteahhcxwv.html

[J01] 获取当前时间
来源：http://hz.yj202588.top/gtofoblbzm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtlqkriufh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtawuwgmwn.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtdwthgedu.html

TS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtkwsrtgat.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtvbxgevap.html

Go:   time.Now()
来源：http://hz.shuidangran.top/gtrznxgwac.html

Ruby: Time.now
来源：http://hz.chenlongwang.top/gtaikkoqzq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ppjwa.cn/gtpppogabj.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gtoysndrne.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gtwxftwweb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtuvfoawdq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtusxlyqyb.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtboclszxc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtsinjbpuy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtneznvhcz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtcartzhho.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtrnxwaqss.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtkwaxngcc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenlongwang.top/gttjsxpymm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtteimfkvz.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtcdbpdleh.html

TS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtttbcuwck.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtjvnurazt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtkkihvpmp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtbojynuqx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtmuvhhmlc.html

[J04] 时间戳与日期互转
来源：http://hz.xziqi.cn/gtmqyivyng.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nwbrower.top/gtvnfaqgdp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gttjqjvhxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hysaishi.cn/gtrgasifro.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shzxlz.cn/gtxhgmligs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtmcxovggf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtejboumum.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtawtegucr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtnbdxyslv.html

[J05] 时间加减（加 7 天）
来源：http://hz.tianlin.xyz/gtmcuwggso.html

Py:   now + timedelta(days=7)
来源：http://hz.jlsjyb.cn/gtjicneyig.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtveokvvma.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtehijqsoq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtleodsder.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtchugffli.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtxjeoyxxd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ybcxt.top/gtmvytkerz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tanke756.top/gtvktucxab.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gtzwzmecob.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtobkecjku.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gthlnefjmh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtsmonrigt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtxdefinnu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinghuilouyu.cn/gthphtfcdj.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gttoaqwiiv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtxanrpctr.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtjixwhpjg.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtctfvjfdo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtccxjehdt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtuditodcg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtvpjmjttv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.316326.xyz/gtjpgeccmj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hfpthk.cn/gtiilcuyya.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhixingplan.top/gtaifibzla.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtslibosku.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtnecpfapc.html

[J08] 提取年月日与星期
来源：http://hz.hfpthk.cn/gtzojcucfj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258.top/gtxxkwnheg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shzxlz.cn/gtqfhryjbv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtwtrffojt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtiespzojm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhengqikj.top/gtujvevwga.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.c1oappe.top/gtkmpcutzl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gtozhbgsgb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtmkesteqx.html

[J09] 时区处理
来源：http://hz.zhoulong.xyz/gtctoliumd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.wangshuangyany.cn/gtbmfeohae.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtavxetgjj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtgdcetags.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtwafuaxqf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gtcbtsvwan.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtsbrcyosu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtsfmjjzqc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtkjxwhrac.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtlcjsrbma.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gtabgjvrab.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hywenlv.cn/gtipmbjoot.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ppjwa.cn/gtyxfyalxz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nwbrower.top/gtdfbrwhbh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtsjwbwgiz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cdnleiting.top/gtesmrudtz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.haohaochexian.top/gttbxppfdc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtxmikvzof.html


<!-- 参考信息 -->