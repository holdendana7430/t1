代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtrlqyacxb.html

Ruby: def to_s; @name; end
来源：http://hz.316326.xyz/gtsqhaasho.html

C#:   public override string ToString() => Name;
来源：http://hz.andypj.xyz/gtejhkkdsx.html

[G13] 判断对象类型
来源：http://hz.tian-w.cn/gtbkuisbad.html

Py:   isinstance(u, User)
来源：http://hz.redwolf501.top/gtyqihonda.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gtcehgthoo.html

JS:   u instanceof User
来源：http://hz.yuxming.cn/gtyneuvwbe.html

TS:   u instanceof User
来源：http://hz.wangdashe.top/gtfuyblvuv.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtmqqoczvw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xuanzx.com/gthdprrmji.html

Ruby: u.is_a?(User)
来源：http://hz.jqgfzy.top/gtktkfstvg.html

C#:   u is User
来源：http://hz.guowangkeji.top/gtrbckakmj.html

[G14] 数据类 / record
来源：http://hz.sysykeji.top/gtqywlnzfi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yueranfly.top/gttzzfuohc.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.xziqi.cn/gtcsybsujb.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtnxhoslmx.html

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gtezxrwiif.html

Java: record User(String name, int age) {}
来源：http://hz.shzxlz.cn/gtrjnzcozm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jianghu66.top/gtjxcxwcqj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.quarkkingdee.top/gtgzrvojja.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gtnfkegwig.html

[G15] 枚举
来源：http://hz.cheryme.top/gtsjkrjhln.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhongyouzk.top/gtuqarofqb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gtsowqccrj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtanzfefcr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yangfankeji.com/gtmjobrowj.html

Java: enum Color { RED, GREEN }
来源：http://hz.pycfn.com/gtznfwjwlj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ivvv.top/gtntqlmkdo.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gttinsqgav.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yj202588.top/gtmtgongab.html

[G16] 对象转数组 / 字典
来源：http://hz.hnqzz.top/gtwrheedak.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj20258.top/gtetxvvyfe.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtfhzcilux.html

JS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtyqenrsui.html

TS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtsqykykif.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gthsmmwnyy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.svipenyu.cn/gtrmexyoyn.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtdowvjcnr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtimnomuoe.html

================================================================================
来源：http://hz.nanxinkj.top/gtilwnytyp.html

H. 异常与错误处理
来源：http://hz.sxryk.cn/gtzgkrhrqr.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaefxskkd.html

[H01] try / catch 基础
来源：http://hz.yj202588.top/gtpfwobrfq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.daxiang520.top/gtgbsgcybh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtmuzolvss.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhongyouzk.top/gtexphjxgs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtwytkyldu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtcatgksrv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ybcxt.top/gtwixcytcu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtydhmfhly.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtcfiveuld.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtkykjcnyb.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtiyxthwgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtkrrwpibz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtxnagzezr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtcafygthl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtkdkpvpqd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.meibo888.top/gtyendwqrf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xziqi.cn/gtpbppxuaf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtpmgzbfms.html

[H03] 主动抛出异常
来源：http://hz.yangfankeji.com/gtdyjzjwnz.html

Py:   raise ValueError("错误信息")
来源：http://hz.aizwys.cn/gtfouzltuw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtvnfbbwuh.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtrcsqosco.html

TS:   throw new Error("错误信息");
来源：http://hz.gogol.net.cn/gtgdzovymy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zycfv.cn/gtzoxydnvw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtgkyphset.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtitlgwfxk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gthhzthnbw.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gthftbmmvy.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtfjpvynsd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daxiang520.top/gtyepcjpvj.html

JS:   class MyError extends Error {}
来源：http://hz.xuetiantiany.cn/gtuilsbzwx.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtbovnimwb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtbpcoijcr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gttcjrdzqi.html

Ruby: class MyError < StandardError; end
来源：http://hz.mhx1999.top/gthgbqnyui.html

C#:   class MyException : Exception {}
来源：http://hz.meibo888.top/gtlkwiffjr.html

[H05] 捕获特定类型
来源：http://hz.smart0.xyz/gtplkltzhn.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gtcfladhnw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtpprcmbnb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtkiibphiw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtfrlxgxfg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtryazaduz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj202588.top/gthklyxsnq.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtbvgcbjwb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtepugotkm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gteowgmonz.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtifbawphz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtqovqfywq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtaabssnhg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtguzhsgmo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dashuyun.cn/gtlyyjbybj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gtzdxzpxku.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtzgwmhuij.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxinkj.top/gtiwtulwhr.html

[H07] 断言
来源：http://hz.sxryk.cn/gtxtihisqw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtwegrakac.html

PHP:  assert($x > 0);
来源：http://hz.jyoumei.cn/gtcizforlh.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtclbtihyq.html

TS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gttxxlpjnx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhaomingkeji.xyz/gtrubhrkgt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtujgtmemn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtsxnnwhla.html

C#:   Debug.Assert(x > 0);
来源：http://hz.guowangkeji.top/gtkjrbqlgn.html

[H08] 获取错误信息与堆栈
来源：http://hz.daxiang520.top/gtdehplult.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gzhubu.top/gtnmqecbau.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cashguo.top/gtiwdnpfss.html

JS:   e.message;  e.stack
来源：http://hz.pengpengdd.cyou/gtchwcpjzb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtfipejqhz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtbchypuwn.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtygprlqfg.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gtlfebodkg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtebibmnyk.html

[H09] 带错误码的异常
来源：http://hz.sufxvd.cn/gtemypznfn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtrhyihqsx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtyyyfxkrj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtbfnukpox.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtzlndejoy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtayielepj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigufen.top/gtiatutexv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtflnjdndm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtbmmygkcl.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtsdddjiod.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtbnleemla.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.316326.xyz/gtddaduehh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtgufgjpuf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtrmjveyvy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtksokckvs.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtiansbjat.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gogol.net.cn/gtkmnqybyx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhixingplan.top/gtfrfawzqm.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvkrujtrk.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtwwnlpuyg.html

================================================================================
来源：http://hz.pycfn.com/gtpptgtujd.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gttaiaerrc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtdxouoyng.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtewmwgskd.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtrcvjrvke.html

TS:   /\d+/.test(s)
来源：http://hz.meibo888.top/gtfrbxkdop.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtbvlsacmq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gtqobouyle.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtutjywczy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gttnfiqdcx.html

[I02] 提取所有匹配
来源：http://hz.zhoulong.xyz/gteiikfykp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daxiang520.top/gtdjmsvvad.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtxtkulqgd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtkjofwegu.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtnoxgiexy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.mhx1999.top/gtjbaqzath.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tianlin.xyz/gtgqnbtkto.html

Ruby: s.scan(/\d+/)
来源：http://hz.jianghu66.top/gtgkjpmscy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yongpay.top/gtdhkfdosf.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtsxdlnaty.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gogol.net.cn/gtcbusngzi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtjhcejgay.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtltrhqtes.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shangyingyoupin.top/gtkiaeokqy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtzspmvgfh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shangyingyoupin.top/gteczxsbmw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtwrcxmfjx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtauohnpva.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtjjcbfzcy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xinyue.icu/gtjasgxgte.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtsalzjcde.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtxxzphtsu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtfdpgeqco.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtjtbyythl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yueranfly.top/gtdfcxglzt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gttwccdgbj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtbqepnikv.html

[I05] 按正则拆分
来源：http://hz.yj20258.top/gtgmvvuxqt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtyrfifedj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hongshengwenyu.top/gtrzisxaja.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtopdzalfi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtryectaao.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuanzhike.top/gteoihqlch.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtpetpblnr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtsvpikzhj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtestfhkaw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gteuxgqzwx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtberkzvvr.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gotoacloud.top/gtwijkgebe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ivvv.top/gtdtgabgwg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtffrbqzld.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtapkokvvi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtyodyfwpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jlsjyb.cn/gthfvikmkb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtxhwitkfx.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtjnkdyllc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtpljozbbc.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtbqwwwqvn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtkbgveazc.html

TS:   /error/gim
来源：http://hz.yuxming.cn/gtbteigjna.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtkirkkbla.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtoydtirpl.html

Ruby: s.scan(/error/i)
来源：http://hz.nwbrower.top/gtcxjanacc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ppjwa.cn/gtexyqfcho.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtxcrtklce.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtkvmzyjmv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.redwolf501.top/gtjxiaezst.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtfhrnjhht.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtexmwncbn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yonumen.top/gtcgsbgupg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhoulong.xyz/gtawrxbtyt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shuidangran.top/gtemngxvtr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtdxbrzgsl.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtyyylvcdg.html

J. 日期与时间
来源：http://hz.c1oappe.top/gthjeilbsk.html

================================================================================
来源：http://hz.aibaodan.cn/gtocprawok.html

[J01] 获取当前时间
来源：http://hz.jianghu66.top/gtqhoccjsa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj202588.top/gtqhqyfvaz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtbmiwdxwx.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtxslgxtni.html

TS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gtwrodelnr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hysaishi.cn/gtzcxwfhfc.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gtjashfcbc.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtsaauzvql.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cqqwz.cn/gtxsxjzeqp.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtfcghtfye.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtenzxgdbk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtynmbnykl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.andypj.xyz/gtxnhidawh.html

TS:   d.toISOString()
来源：http://hz.aibaodan.cn/gtlnkoftyt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gthwxkbidf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhongyouzk.top/gtdczojvyd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtzzlmnqzk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangshuangyany.cn/gtymcqazuk.html

[J03] 字符串解析为日期
来源：http://hz.havefunace.top/gtxmplcdge.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhengqikj.top/gtwqshrxvt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhijiandao.cn/gtyqctvggs.html

JS:   new Date("2024-01-02")
来源：http://hz.daria6918.cn/gtvxdaenik.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtobimlwsk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.smart0.xyz/gtckjwwkve.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gthljmuwff.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtbfpbqqyx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtdncakgrv.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtkufpiqle.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cheryme.top/gthnvpuxjs.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtymruacwy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtbdednhzq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tian-w.cn/gtvjcedeyv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhiwuduotai.top/gtbfqewxxf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtpmfgqwhx.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtjjedweng.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtwedboxoz.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuxming.cn/gtdzknwlwg.html

Py:   now + timedelta(days=7)
来源：http://hz.sxryk.cn/gtiezxixbx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtasyvobkv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtuxvbgnrd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gttktuntcm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cdnleiting.top/gtwemqpoop.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.sweek.top/gtizchladn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ydzc1.top/gtaohnzkbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gttgfdwcdw.html

[J06] 计算两时间之差
来源：http://hz.ehwqpu.com/gtwykdevku.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gthbqdroks.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtpzrfyijo.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fengsongda.top/gtrhvbeopw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pengpengdd.cyou/gtpokqdade.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yongpay.top/gtztnrmvyj.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenlongwang.top/gtevutkvov.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtwpoujuud.html

C#:   (end - start).TotalSeconds
来源：http://hz.tian-w.cn/gtucocpjgs.html

[J07] 比较两个日期
来源：http://hz.wangshuangyany.cn/gtibhtbvnc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yueranfly.top/gtrkgfrmcf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuetiantiany.cn/gtslkcqkzu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gttxqfrmhm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtffhmxwdl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtbgycgqta.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daria6918.cn/gtxnynqvde.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtlqwposfk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtsbwdavzm.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtesorbjpq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtrcbdkeor.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuanzx.com/gtylhlosrv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gturyjzguq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.vqdsnc.cn/gtaicnhhkg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtdapiolid.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sysykeji.top/gtnqlvvoog.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.haohaochexian.top/gtmevpntxz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj20258888.top/gtsfoqgjbm.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtxwkeqerl.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gtttnmoeld.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxinkj.top/gtehhcszdb.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtzjuyegsn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtufyxqmbk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgfzy.top/gtqrslrnxy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtybrmsygt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtyobzmwny.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fengsongda.top/gtwgdzpnut.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuxming.cn/gtvvsxuwja.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtraqeqjku.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gttwopjpwu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gttuyklyvo.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtxpvxueyk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.guannengcc.top/gtbtrztroh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ybcxt.top/gtjjexveje.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtlwwllxss.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gtfxqiptjl.html


<!-- 参考信息 -->