代发 wailian999

JS:   super.greet();
来源：http://hz.wangshuangyany.cn/gtpwzwseyt.html

TS:   super.greet();
来源：http://hz.zhoulong.xyz/gtyskcvrpx.html

Java: super.greet();
来源：http://hz.zycfv.cn/gtghkfhwur.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cqqwz.cn/gtqtoyyotf.html

Ruby: super
来源：http://hz.c1oappe.top/gtwktkyqjv.html

C#:   base.Greet();
来源：http://hz.tianlin.xyz/gtvzoorhvq.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtxxuhzfln.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinghuilouyu.cn/gtqpcfjnbg.html

PHP:  public static function f() {}
来源：http://hz.zhijiandao.cn/gtywuxljlx.html

JS:   static f() {}
来源：http://hz.yuanzhike.top/gthyssoavz.html

TS:   static f(): void {}
来源：http://hz.cqqwz.cn/gteuvugsbj.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtbxkyzkty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtdigtbiwg.html

Ruby: def self.f; end
来源：http://hz.9152youxi.cn/gtfxlqcntj.html

C#:   public static void F() {}
来源：http://hz.pengpengdd.cyou/gtbhhbwasd.html

[G09] 接口 / 抽象类
来源：http://hz.jqgufenzy.top/gtmfvfrnvc.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.iojbl.cn/gtwefsdvfo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtazqdclgq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtmolraslg.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgfzy.top/gtnpvltyvp.html

Java: interface Shape { double area(); }
来源：http://hz.gzhubu.top/gtanejjhqw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zycfv.cn/gtopgdbxch.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gzhubu.top/gtikjvlyxc.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtnyrqgmlh.html

[G10] 访问控制
来源：http://hz.ivvv.top/gtgbjnclfu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aibaodan.cn/gtdvdydzsk.html

PHP:  public / protected / private
来源：http://hz.jqgfzy.top/gtacnppedb.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtwnxbftgx.html

TS:   public / protected / private
来源：http://hz.ydjk.org.cn/gtijayuikr.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gtetcjuydn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.guowangkeji.top/gtwcpcunbx.html

Ruby: public / protected / private
来源：http://hz.yvedp.cn/gtytdqzvpn.html

C#:   public / protected / private / internal
来源：http://hz.snrcjt.cn/gtlzvwfiya.html

[G11] getter / setter
来源：http://hz.shanyushiyangtech.top/gtuushmiko.html

Py:   @property 与 @x.setter
来源：http://hz.xingfuxueyuan.xyz/gtajkafihs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtfmmunlse.html

JS:   get name() { return this._name; }
来源：http://hz.yueranfly.top/gtpjbhaiqk.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gttwepexfc.html

Java: public String getName() { return name; }
来源：http://hz.zhijiandao.cn/gtbhpyzlfz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtegmysyjq.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtlctoywqg.html

C#:   public string Name { get; set; }
来源：http://hz.smart0.xyz/gttsiyvlvw.html

[G12] 对象转字符串
来源：http://hz.ybcxt.top/gtwujvvamw.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtfgpzzaps.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gtxfplhebg.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtwhlcqaoz.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtmjqaeqlp.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtpaqcuzgg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtjmokscqt.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gtsujyphdm.html

C#:   public override string ToString() => Name;
来源：http://hz.zhoulong.xyz/gtxvkzgcsi.html

[G13] 判断对象类型
来源：http://hz.yvedp.cn/gtedgprwcl.html

Py:   isinstance(u, User)
来源：http://hz.nanxinkj.top/gtqmljacrn.html

PHP:  $u instanceof User
来源：http://hz.yangfankeji.com/gtlwdljyhf.html

JS:   u instanceof User
来源：http://hz.tianlin.xyz/gtpfkmwjqj.html

TS:   u instanceof User
来源：http://hz.gzhubu.top/gtyrylwtfg.html

Java: u instanceof User
来源：http://hz.sweek.top/gtxkxzohad.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtgugfpkvc.html

Ruby: u.is_a?(User)
来源：http://hz.nwbrower.top/gtdifiiyss.html

C#:   u is User
来源：http://hz.ydzc1.top/gtrhqbabhv.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gtjmswzfpz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gteufeyiey.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtswqtrdhm.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cashguo.top/gtpszjryou.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gtztpkzpie.html

Java: record User(String name, int age) {}
来源：http://hz.jyoumei.cn/gtimajhirq.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ivvv.top/gtexutufth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtcltgrqdl.html

C#:   record User(string Name, int Age);
来源：http://hz.sysykeji.top/gtzfbmcesg.html

[G15] 枚举
来源：http://hz.zhengqikj.top/gtdmptmyly.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hnqzz.top/gtdmmevcjd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cdnleiting.top/gtnylldvcq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangdashe.top/gttqcfcddp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sufxvd.cn/gtgjxpufxb.html

Java: enum Color { RED, GREEN }
来源：http://hz.xylfe.cn/gtvlrdarbd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.mhx1999.top/gtyghoqthx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxuanxn.top/gtcmnxrfpe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.birdmap.top/gtjwxgvuah.html

[G16] 对象转数组 / 字典
来源：http://hz.cucudq.cn/gtyurohsqn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hnqzz.top/gtyujiadye.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtsydfbspl.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtazndkvwa.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtslksievn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxinkj.top/gtjqpvecuh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtcxnoraxd.html

Ruby: obj.instance_variables
来源：http://hz.sufxvd.cn/gtrovxukge.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtuenvnehr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtyawkrwpp.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtwjdapnsa.html

================================================================================
来源：http://hz.yangfankeji.com/gtsvxgqofk.html

[H01] try / catch 基础
来源：http://hz.c1oappe.top/gtfagzhkyx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtcjbicwau.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gttfvbunfs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtpygkcolk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.feifeiyinyue.top/gtgatdsldc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.svipenyu.cn/gtyvoqemzd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zycfv.cn/gthvnxwoay.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtshcfeniw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cheryme.top/gtaapiekci.html

[H02] finally / ensure 收尾
来源：http://hz.xinyue.icu/gtqtrerumn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.gogol.net.cn/gtctlsdkzf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtkzifbian.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtbuevlorv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtryagzylx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gthgjksuit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtggqdgbbz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangshuangyany.cn/gtzuwyunyz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhoulong.xyz/gtgynhfmeg.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtgwbclrdz.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtpbtulydt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtkaxpljlw.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtbyofsjxv.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtlfjwppgt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtxzkkilwe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gteemaayvp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hysaishi.cn/gtipyegisv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtbietnlwv.html

[H04] 自定义异常类型
来源：http://hz.gzhubu.top/gtyljgjsif.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtmlkdljph.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yuxming.cn/gthezpgvqm.html

JS:   class MyError extends Error {}
来源：http://hz.jinqigufen.top/gtlznjffkh.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtqqfajcir.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtlswdeqre.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtehyrncjc.html

Ruby: class MyError < StandardError; end
来源：http://hz.svipenyu.cn/gtplxlwvfy.html

C#:   class MyException : Exception {}
来源：http://hz.hysaishi.cn/gtoybulbaz.html

[H05] 捕获特定类型
来源：http://hz.jyoumei.cn/gtmwluxcgz.html

Py:   except ValueError as e:
来源：http://hz.yuanzhike.top/gtpjqycabz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.smart0.xyz/gtqyjpeyiy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtnunhqxcd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gtlmzmweoy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gtqnwkvonk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtoujexgiv.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gttqxcpfye.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtcuvqunly.html

[H06] 可选值 / 空值安全访问
来源：http://hz.redwolf501.top/gtywivqpch.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtojitphpi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shanyushiyangtech.top/gtwponktkx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtneeuofha.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gtindxwtrc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.dashuyun.cn/gtfopyqqfu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtruackitk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gthnxxyjcn.html

C#:   obj?.A?.B ?? default
来源：http://hz.sufxvd.cn/gtellzirew.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gtjpdsdlso.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtswatnohm.html

PHP:  assert($x > 0);
来源：http://hz.ydzc1.top/gtpnqqucfg.html

JS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtouundisd.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtbyhfiqpw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtfadvzsvf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gtzummufhd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtulvwqfrv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj202588.top/gtgxzhetdg.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtfdapvaiy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtprlyjxqh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtjdtxbdda.html

JS:   e.message;  e.stack
来源：http://hz.kuanghao11.cn/gtsygaoodu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuanzhike.top/gtyvhrckud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sysykeji.top/gtrufutmns.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtehlwflrh.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtuyajhdqy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zdqjudy.top/gtmgjjggoo.html

[H09] 带错误码的异常
来源：http://hz.xziqi.cn/gtyegtxraw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yangfankeji.com/gthykbiivm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtaqeuyhit.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.snrcjt.cn/gtibcaxbuz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtrlgzokmk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gttiofsoho.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtkyxwigau.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yueranfly.top/gtzakxryon.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ywan-chungtsiang.top/gteabftlue.html

[H10] 资源自动释放
来源：http://hz.wangdashe.top/gtpipgxgtd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.9152youxi.cn/gtwwjaakoq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtblvoaknb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gtgrjofcdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtijwvmlbu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xinyue.icu/gtyocvrqha.html

Go:   defer f.Close()
来源：http://hz.sufxvd.cn/gtkknxnmnb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtxqbtmbyv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yvedp.cn/gtzqbpnofc.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtauibaoqm.html

I. 正则表达式
来源：http://hz.fzhhl.top/gtexwdrevj.html

================================================================================
来源：http://hz.iojbl.cn/gtjmmmomma.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtylfgtfqz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtbewsdwoo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yanxiufei.cn/gttprsdyzp.html

JS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtlciufroz.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtcinwlaft.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtwsfjjxyl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hongshengwenyu.top/gtxkicgjdm.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtbqpemmuf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtdhyiyxhd.html

[I02] 提取所有匹配
来源：http://hz.iojbl.cn/gtftwoaegs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtkcgfynoj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtkjwnctxs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gthyiufkph.html

TS:   s.match(/\d+/g)
来源：http://hz.snrcjt.cn/gtbueqcqox.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtwbkdaspk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtntopmkaj.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtetvaaqcf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xinyue.icu/gtyxwrrzqf.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtvkbzfsai.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gtrmiijtqv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxuanxn.top/gtdfvyvvpz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnxiangtu.top/gtotkyndsc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtflxbysdm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtrkkuymqi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtzzokgkjr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tian-w.cn/gtbfefiivv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gttipzroey.html

[I04] 正则替换
来源：http://hz.sweek.top/gtovferixj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtdttrgwrf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtbphlgvyy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtcisqqmjf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtatcykrvx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnxiangtu.top/gtynmmltwl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gttbcsilgm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.0kj1m.cn/gttdqhstxu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtvlvngkdn.html

[I05] 按正则拆分
来源：http://hz.cheryme.top/gtgoeegbbv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nwbrower.top/gtzeufinwz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtjkwuosal.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtfsuyghjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtanzsjvoy.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtrgjfkggq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aibaodan.cn/gtihtobdjv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtjspfmhwa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtjzlbaaqr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtxwitdgui.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtbthbfxym.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtpusjbdug.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtaniunvwj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtvwzngsxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.svipenyu.cn/gtvddguhuu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cucudq.cn/gtdpgelgxp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtzebqnszl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtjujgzccg.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtreaoewiw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hnxiangtu.top/gtrzebwvkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtfnqsvnqj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tanke756.top/gtzayopzgq.html

TS:   /error/gim
来源：http://hz.yj20258888.top/gtownpzygs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtlbjolypk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gtsupmsfgy.html

Ruby: s.scan(/error/i)
来源：http://hz.ppjwa.cn/gtwdyevzxl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtenbudjmp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gthrytouvz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtphzehvje.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtngjpzmug.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gttpfrqeoc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtholtnepl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtfczbsztt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gthctjytea.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xuetiantiany.cn/gtoyimpzwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtxqwedist.html

================================================================================
来源：http://hz.aizwys.cn/gtjfpmjdyu.html

J. 日期与时间
来源：http://hz.guannengcc.top/gtzjvfahui.html

================================================================================
来源：http://hz.zhixingplan.top/gtrpjnkgpa.html

[J01] 获取当前时间
来源：http://hz.nanxuanxn.top/gtaqqmqjve.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtrkdibbbl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtuimbgyrg.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gteprpnrzr.html

TS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtkvmjdljz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fzhhl.top/gtvzgcixrw.html

Go:   time.Now()
来源：http://hz.xingfuxueyuan.xyz/gtibiupfel.html

Ruby: Time.now
来源：http://hz.jqgfzy.top/gtwjxkodcw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtwwpwsjnk.html

[J02] 格式化输出
来源：http://hz.shanyushiyangtech.top/gtfbsbwmtv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtwaqfrkbo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtgsychqyr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gterqycdwm.html

TS:   d.toISOString()
来源：http://hz.jinqigfzy.top/gtsrcnxytn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtsojmqyri.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtroizmsfj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtxfyqsdcc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jianghu66.top/gtssocdesv.html

[J03] 字符串解析为日期
来源：http://hz.fzhhl.top/gtpjmarhhi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gtnwkdjdiw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jianghu66.top/gtyemgsevm.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gthlhmhmtb.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtvblgeivu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhoulong.xyz/gtvwlcnjyv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtnxdupuym.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sxryk.cn/gtiinwxwtv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shangyingyoupin.top/gtavhcbele.html

[J04] 时间戳与日期互转
来源：http://hz.yongpay.top/gtbqfhbcdu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tianlin.xyz/gtysfmtbck.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtdnyricae.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtfhxmxxcl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtoehbpbly.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.meibo888.top/gtwfunkfoz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtuknskoln.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pycfn.com/gtkejipvhg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258888.top/gttmnvpfix.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtyizfsdbt.html

Py:   now + timedelta(days=7)
来源：http://hz.xziqi.cn/gtratfxqgj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangkeji.top/gtxupbwzbs.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtpeqhyxno.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtlblhdymh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ywan-chungtsiang.top/gtkbfseqfn.html


<!-- 参考信息 -->