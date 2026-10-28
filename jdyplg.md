代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.yuxming.cn/gtawnajfcd.html

[G03] 实例属性
来源：http://hz.nanxuanxn.top/gtxejbococ.html

Py:   self.name = "x"
来源：http://hz.yj20258.top/gtodycujat.html

PHP:  public string $name = "x";
来源：http://hz.xylfe.cn/gtegntxfrf.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtajxftdir.html

TS:   name: string = "x";
来源：http://hz.shangyingyoupin.top/gtbdcjusak.html

Java: private String name;
来源：http://hz.hnxiangtu.top/gtzzcvjebk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.haohaochexian.top/gtjvldwxcd.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtirgvmdzd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.meibo888.top/gtsasxpfyx.html

[G04] 定义方法
来源：http://hz.gzhubu.top/gtynmutyqq.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtwrgtuiwc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jqgufenzy.top/gtrfundzia.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtpnvflisf.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtbrwlukik.html

Java: String greet() { return name; }
来源：http://hz.c1oappe.top/gtoplzxaqd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtiapdebxn.html

Ruby: def greet; @name; end
来源：http://hz.xingfuxueyuan.xyz/gtimejmmfq.html

C#:   public string Greet() => Name;
来源：http://hz.jiagoushi.top/gtwwdlzpyp.html

[G05] 继承
来源：http://hz.nanxinkj.top/gtlbsvtdfr.html

Py:   class Admin(User): pass
来源：http://hz.daxiang520.top/gtykapspwa.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtdecmcidp.html

JS:   class Admin extends User {}
来源：http://hz.redwolf501.top/gtqwqylxyq.html

TS:   class Admin extends User {}
来源：http://hz.tianlin.xyz/gtykplvrjl.html

Java: class Admin extends User {}
来源：http://hz.tanke756.top/gtrjwibqii.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ybcxt.top/gtwchtxwpt.html

Ruby: class Admin < User; end
来源：http://hz.wangdashe.top/gtyegyteoe.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtceluotxh.html

[G06] 重写方法
来源：http://hz.jiagoushi.top/gtqpzqclob.html

Py:   def greet(self): return "admin"
来源：http://hz.aizwys.cn/gtiauziznq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ydzc1.top/gtulaffmig.html

JS:   greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtiwatnhra.html

TS:   greet(): string { return "admin"; }
来源：http://hz.iojbl.cn/gtdbyuwqar.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtaznzkvcd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.wangdashe.top/gthldphprx.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtfcghfbbw.html

C#:   public override string Greet() => "admin";
来源：http://hz.cucudq.cn/gtzqrcvwxi.html

[G07] 调用父类方法
来源：http://hz.yj202588.top/gtldlkbehx.html

Py:   super().greet()
来源：http://hz.havefunace.top/gthibfpzpi.html

PHP:  parent::greet();
来源：http://hz.wangshuangyany.cn/gtsjaxpffn.html

JS:   super.greet();
来源：http://hz.yonumen.top/gtcukfuoob.html

TS:   super.greet();
来源：http://hz.sxryk.cn/gteinfymdh.html

Java: super.greet();
来源：http://hz.daria6918.cn/gttuinnpcd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtojmkulhy.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtpwnsvxtw.html

C#:   base.Greet();
来源：http://hz.ydjk.org.cn/gtfsrypuck.html

[G08] 静态方法与属性
来源：http://hz.feifeiyinyue.top/gtbowbngth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.c1oappe.top/gtxeqsctyk.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gttakbgoug.html

JS:   static f() {}
来源：http://hz.zhoulong.xyz/gtiqpnzyki.html

TS:   static f(): void {}
来源：http://hz.jinqigufen.top/gtowwkrihb.html

Java: static void f() {}
来源：http://hz.ydjk.org.cn/gtcgvzsfwv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.fzhhl.top/gtftzvozsm.html

Ruby: def self.f; end
来源：http://hz.zdqjudy.top/gtyrdxrmqs.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtfyswwflt.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtpcxbegqh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hongshengwenyu.top/gtlvxdwjie.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sysykeji.top/gttagjipbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.gzhubu.top/gtwwcmvzqb.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtlzndpoxw.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtpumycghi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.haohaochexian.top/gtrdcrgdzx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.feifeiyinyue.top/gtegvhxveu.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhoulong.xyz/gtmnlkxbkn.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtvdzjaipi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gteaxrfpvc.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtkobqebak.html

JS:   #private 字段；其余公开
来源：http://hz.gotoacloud.top/gtfshsysrw.html

TS:   public / protected / private
来源：http://hz.xylfe.cn/gtaaxqppdu.html

Java: public / protected / private / 默认包级
来源：http://hz.feifeiyinyue.top/gthokekcxh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.svipenyu.cn/gtxhaunhpf.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtakaployl.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtxnfmrema.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtqwlsqcue.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtpjwsfzao.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.ivvv.top/gtxilfwcid.html

JS:   get name() { return this._name; }
来源：http://hz.shuidangran.top/gtwtncwweb.html

TS:   get name(): string { return this._name; }
来源：http://hz.jyoumei.cn/gttqcgnyjq.html

Java: public String getName() { return name; }
来源：http://hz.zhoulong.xyz/gtygnmeboq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtihhhbask.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtvwsnldyt.html

C#:   public string Name { get; set; }
来源：http://hz.jqgfzy.top/gtstflojyv.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtrevfjyyx.html

Py:   def __str__(self): return self.name
来源：http://hz.fengsongda.top/gtxcmbtybk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtofyxhgft.html

JS:   toString() { return this.name; }
来源：http://hz.hysaishi.cn/gtqupqobxy.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgufenzy.top/gtctuttbwo.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtcappgvob.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yonumen.top/gtcoebrjjh.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtujvvpzco.html

C#:   public override string ToString() => Name;
来源：http://hz.tianlin.xyz/gtjmazuyhf.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gttjrzmlti.html

Py:   isinstance(u, User)
来源：http://hz.hfpthk.cn/gtmfyzxjhf.html

PHP:  $u instanceof User
来源：http://hz.c1oappe.top/gtbbotvkaa.html

JS:   u instanceof User
来源：http://hz.ehwqpu.com/gtahagsvyl.html

TS:   u instanceof User
来源：http://hz.hongshengwenyu.top/gtciqwvupi.html

Java: u instanceof User
来源：http://hz.fzhhl.top/gtvyjsznve.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtcrmmdcgt.html

Ruby: u.is_a?(User)
来源：http://hz.zhoulong.xyz/gtzrclijts.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtlxmgmpse.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtrxverrbx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.c1oappe.top/gtswiblwpw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtoxbmftkd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yongpay.top/gtevkjzfgx.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gttyroqtvr.html

Java: record User(String name, int age) {}
来源：http://hz.yj20258.top/gtavobyvfv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinqigfzy.top/gthdwqkzra.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.svipenyu.cn/gtjcuoknkr.html

C#:   record User(string Name, int Age);
来源：http://hz.zycfv.cn/gttlzwodfv.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtxktgtcrc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.hongshengwenyu.top/gtwshtesds.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hysaishi.cn/gtcyxcqkdf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.9152youxi.cn/gtclnzjdfl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhixingplan.top/gtortivoxr.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj202588.top/gtvwkzgghg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ehwqpu.com/gtppfpbicz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtvqkimqcm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtscrnnjbn.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtlfyhyhmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtwzfwdrbo.html

PHP:  get_object_vars($obj);
来源：http://hz.ydzc1.top/gtyumvkdir.html

JS:   Object.entries(obj)
来源：http://hz.316326.xyz/gtfchknihk.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtgchphnxp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gteyftsdww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gogol.net.cn/gtblmgnbdc.html

Ruby: obj.instance_variables
来源：http://hz.hammf.cn/gtpmfhynuj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtbnlnpydm.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtnkakzaws.html

H. 异常与错误处理
来源：http://hz.chenjidiqi.icu/gtdnjjmorf.html

================================================================================
来源：http://hz.sweek.top/gtverjgdxv.html

[H01] try / catch 基础
来源：http://hz.cdnleiting.top/gtonhxkpta.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtbcntejsj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xuetiantiany.cn/gtgmzxdudc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtywuttrso.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuanzhike.top/gtgkmaxyiw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangshuangyany.cn/gthgkeamao.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nanxinkj.top/gtvfnhgbdt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gtfadthhre.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtkifnzigz.html

[H02] finally / ensure 收尾
来源：http://hz.gogol.net.cn/gtgeqnxjpm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtjfbekkpu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtznaiwkcj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtzkmuxqgb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtiefnpbkp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtvgoadmzv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sysykeji.top/gtkpmkhcxf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtytjdnrcq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtnddwipfd.html

[H03] 主动抛出异常
来源：http://hz.xylfe.cn/gthtgfvzsl.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gthroyiocx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtjhxgszaa.html

JS:   throw new Error("错误信息");
来源：http://hz.kuanghao11.cn/gtbimivmyr.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtxfuatsuy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gturbxpsal.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jqgufenzy.top/gtmtpcrvgw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yuxming.cn/gtgxjzrgcb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtaxirbihm.html

[H04] 自定义异常类型
来源：http://hz.cqqwz.cn/gtczktjrpp.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gtuhvojake.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zycfv.cn/gtmlcrkdyr.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtojfwnweq.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtnfpgwbat.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtxqsohugb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtddqxxvfp.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtupetjlrf.html

C#:   class MyException : Exception {}
来源：http://hz.hysaishi.cn/gtwkflefcn.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtjvggeciw.html

Py:   except ValueError as e:
来源：http://hz.svipenyu.cn/gtfniceaak.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yonumen.top/gtyhqeoslz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtoaabpgqo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtqrgaarny.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinghuilouyu.cn/gtzoqwgsfj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gtuiyalhcy.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuxming.cn/gtqhmutwcp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.316326.xyz/gtidjraiib.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtbhrqhede.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtlyrswlvy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gteynlpeqd.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gttqrlqlhc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtusawxmno.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydjk.org.cn/gthopkajbk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtnuggqkvs.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yangfankeji.com/gtukullwnv.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gttowzikgi.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtiksgzurx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtwtqymizm.html

PHP:  assert($x > 0);
来源：http://hz.yonumen.top/gtfpsrcoyh.html

JS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtulxhcwzy.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtgrvzptso.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtrujdgnok.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cucudq.cn/gtszfhtlia.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtmsutgglb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gthpduzign.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gtpsgfkzer.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.haohaochexian.top/gtoxjdsbav.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.haohaochexian.top/gtgekwfrtj.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtojrwfnkv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtbfrlehav.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.birdmap.top/gtuqilfatj.html

Go:   err.Error()
来源：http://hz.zhijiandao.cn/gtjolbupei.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtquinmukn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtsiilbymd.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gtvsnupezf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jqgufenzy.top/gtstwkadoa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtlhxwvwwe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtftymuakj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtmxojvbdb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shuidangran.top/gtexttiucg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangtech.top/gtmnswszud.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtbnjkqdht.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gzhubu.top/gtyfekhknn.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtfruxqulw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtikcjizbo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtidoqjzsc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtrlhnayye.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtvdyjlxbt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtuogibgah.html

Go:   defer f.Close()
来源：http://hz.ivvv.top/gtgqzyezhp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtqtnkqnin.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtmgjqybuy.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtbffhjoft.html

I. 正则表达式
来源：http://hz.0kj1m.cn/gtagvaqjft.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtataipjoi.html

[I01] 判断是否匹配
来源：http://hz.yangfankeji.com/gtgmydvdkv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtstthrvnu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtmjwozjmp.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtomsjixog.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtprbrbmuu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gtamgeqeeg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.wangdashe.top/gtxqxfcbem.html

Ruby: s.match?(/\d+/)
来源：http://hz.tianlin.xyz/gtvqoeksrl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.guannengcc.top/gtjomffvwn.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtdbwkfdwt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtdwuucafg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gtwkbzjuol.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtqeemdfmi.html

TS:   s.match(/\d+/g)
来源：http://hz.aibaodan.cn/gtowucdtif.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtfrcgoycm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtfpkplony.html

Ruby: s.scan(/\d+/)
来源：http://hz.ppjwa.cn/gtfawcvaqp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtxtwuxwnr.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtkckaumpg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtrucwqwwk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtusrsuynj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtabonrasd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtyosqprhr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuanzx.com/gtqesufgrm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ivvv.top/gtidaungry.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.c1oappe.top/gttkjutdhp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xuetiantiany.cn/gtaoksfvmr.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtcbmffbcl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gtcaoipivo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yangfankeji.com/gtdsjbwmxp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtdaaanitz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtiutvniuq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shuidangran.top/gtgslhesdy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuanzhike.top/gtyyukobyh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxuanxn.top/gtrtzxseji.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yj20258888.top/gtrtzgvtqt.html

[I05] 按正则拆分
来源：http://hz.yvedp.cn/gtfooisvry.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtijedmtbg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtncgwnvbi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtpmrxkqva.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtdjpapbrw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jlsjyb.cn/gthhoszwum.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtjlzepkbs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtwqunduos.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gttgfhzdrs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtiucxbbak.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtedbogirs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtgixeowwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtarquggnz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.smart0.xyz/gtohqxdryq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtoytfmpbg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtxqgmkrux.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtoxpkvhgf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xuetiantiany.cn/gtxtrfkvlg.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtsbyfsvul.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtoijrsjuu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtgzaijzjn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtiybppcls.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtdfmnorxs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtvvxtydnh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtakorhllg.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtqwqelsqk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtcngboqki.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtpkepnboy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtncioglzo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtsjmttlxh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtlrkmsegu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtuzfnffzd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtpzuyccuu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtpxksyduu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtxzlzousp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtzetvlzut.html

================================================================================
来源：http://hz.feifeiyinyue.top/gthuyxssov.html

J. 日期与时间
来源：http://hz.vqdsnc.cn/gtstqhfihz.html

================================================================================
来源：http://hz.nanxinkj.top/gtnovxnymz.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtummwfsrc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtgjywaopd.html


<!-- 参考信息 -->