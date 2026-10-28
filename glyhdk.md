代发 wailian999

Py:   class User: pass
来源：http://hz.hnqzz.top/gtbyhuxnpj.html

PHP:  class User {}
来源：http://hz.hongshengwenyu.top/gtcgspxbux.html

JS:   class User {}
来源：http://hz.snrcjt.cn/gthsuaqyxq.html

TS:   class User { name: string = ""; }
来源：http://hz.chenjidiqi.icu/gtydacnwda.html

Java: class User {}
来源：http://hz.hysaishi.cn/gtyqgyyxgc.html

Go:   type User struct { Name string }
来源：http://hz.9152youxi.cn/gtplbzawml.html

Ruby: class User; end
来源：http://hz.sxryk.cn/gtlidgnjwe.html

C#:   class User {}
来源：http://hz.gotoacloud.top/gtvolgltey.html

[G02] 构造函数
来源：http://hz.guowangkeji.top/gtdhwijtob.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtzagrkqdg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtiynaxgeo.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtvjsniylu.html

TS:   constructor(public name: string) {}
来源：http://hz.wangdashe.top/gtsvuqwkrz.html

Java: User(String name) { this.name = name; }
来源：http://hz.cqqwz.cn/gtxgczetuv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtctvnffbc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jqgfzy.top/gtqdellupm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtqmpckuhi.html

[G03] 实例属性
来源：http://hz.dianchejie.cn/gtzbicakui.html

Py:   self.name = "x"
来源：http://hz.shzxlz.cn/gtvoqelius.html

PHP:  public string $name = "x";
来源：http://hz.ppjwa.cn/gtrwizpvjx.html

JS:   this.name = "x";
来源：http://hz.xinyue.icu/gtrduimiju.html

TS:   name: string = "x";
来源：http://hz.yuxming.cn/gtbxpkeokl.html

Java: private String name;
来源：http://hz.fzhhl.top/gtcgqeoqgy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yanxiufei.cn/gtmxdummmy.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtkniewaju.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtabigpbzl.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtewdnvrcg.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtlnqjliul.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.jianghu66.top/gthzjguxbo.html

JS:   greet() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtnmyhrovr.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtzjgnczkk.html

Java: String greet() { return name; }
来源：http://hz.tian-w.cn/gtdgpydgpy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.smart0.xyz/gtkmwhbaba.html

Ruby: def greet; @name; end
来源：http://hz.chenjidiqi.icu/gtomlnrhzu.html

C#:   public string Greet() => Name;
来源：http://hz.aibaodan.cn/gthyrqkxbq.html

[G05] 继承
来源：http://hz.hfpthk.cn/gtexwumvgj.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtrlumjmbi.html

PHP:  class Admin extends User {}
来源：http://hz.wangdashe.top/gtzhvmmmki.html

JS:   class Admin extends User {}
来源：http://hz.jyoumei.cn/gtbavpxlmg.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gtvcbmqpra.html

Java: class Admin extends User {}
来源：http://hz.zhongyouzk.top/gthhwfqday.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.chenjidiqi.icu/gtbghonwnl.html

Ruby: class Admin < User; end
来源：http://hz.jinqigfzy.top/gtrlynkyzy.html

C#:   class Admin : User {}
来源：http://hz.xinyue.icu/gtpaursvbg.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtfjixuwad.html

Py:   def greet(self): return "admin"
来源：http://hz.zhengqikj.top/gtcyuqifcu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtsovidyns.html

JS:   greet() { return "admin"; }
来源：http://hz.cashguo.top/gtqdzmqmnk.html

TS:   greet(): string { return "admin"; }
来源：http://hz.0kj1m.cn/gtsxvsaxlw.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtwyvynyop.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.smart0.xyz/gtdvspsxnz.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtncugppyr.html

C#:   public override string Greet() => "admin";
来源：http://hz.sufxvd.cn/gtyqrugnnq.html

[G07] 调用父类方法
来源：http://hz.cheryme.top/gtwnyvymyz.html

Py:   super().greet()
来源：http://hz.gotoacloud.top/gtajvuiheq.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtsbtbfdef.html

JS:   super.greet();
来源：http://hz.redwolf501.top/gtioczbhpu.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtbsbsjsyc.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtiozukjzl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhixingplan.top/gtajgybpgm.html

Ruby: super
来源：http://hz.zycfv.cn/gtfcnlxqmn.html

C#:   base.Greet();
来源：http://hz.yueranfly.top/gtmfngeywp.html

[G08] 静态方法与属性
来源：http://hz.zhaomingkeji.xyz/gtpixgmasr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxinkj.top/gtlzosdqmp.html

PHP:  public static function f() {}
来源：http://hz.yanxiufei.cn/gtctvhcmwx.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gthjbtwnlo.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtxlcalfyy.html

Java: static void f() {}
来源：http://hz.ybcxt.top/gtagkmgntf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258888.top/gtypdonbnp.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtjvrurapv.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtyaorwkov.html

[G09] 接口 / 抽象类
来源：http://hz.shuidangran.top/gtdcdpgody.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhaomingkeji.xyz/gthbulxxhy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhixingplan.top/gtrhezmmld.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shangyingyoupin.top/gtgtodyalv.html

TS:   interface Shape { area(): number; }
来源：http://hz.hnxiangtu.top/gtgemrtmqu.html

Java: interface Shape { double area(); }
来源：http://hz.yvedp.cn/gtixwdaeit.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gtulqwfmrs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yonumen.top/gtjxgykyab.html

C#:   interface IShape { double Area(); }
来源：http://hz.redwolf501.top/gtgdblfkbx.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtsunfloyu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.aizwys.cn/gtucdkdmtt.html

PHP:  public / protected / private
来源：http://hz.sysykeji.top/gtgjfrkoaw.html

JS:   #private 字段；其余公开
来源：http://hz.c1oappe.top/gtpacwmymw.html

TS:   public / protected / private
来源：http://hz.chenjidiqi.icu/gtqrnbvctv.html

Java: public / protected / private / 默认包级
来源：http://hz.bjfxy.top/gticzielzp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtnqeilswd.html

Ruby: public / protected / private
来源：http://hz.yongpay.top/gtsdvpiapg.html

C#:   public / protected / private / internal
来源：http://hz.jianghu66.top/gtdjohivjn.html

[G11] getter / setter
来源：http://hz.zhixingplan.top/gtbcfzijgh.html

Py:   @property 与 @x.setter
来源：http://hz.jlsjyb.cn/gtunzgfvxi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cashguo.top/gtbraecxlv.html

JS:   get name() { return this._name; }
来源：http://hz.xuanzx.com/gtahmiutsa.html

TS:   get name(): string { return this._name; }
来源：http://hz.jqgufenzy.top/gtsohomvyf.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtmzfaqtis.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.9152youxi.cn/gtgwtyguvp.html

Ruby: attr_accessor :name
来源：http://hz.yj20258888.top/gtcfghzzzn.html

C#:   public string Name { get; set; }
来源：http://hz.zhengqikj.top/gtpjtdaare.html

[G12] 对象转字符串
来源：http://hz.fengsongda.top/gtyoevhkkb.html

Py:   def __str__(self): return self.name
来源：http://hz.52xcode.cn/gtxsdlinxg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtxkptscsh.html

JS:   toString() { return this.name; }
来源：http://hz.guannengcc.top/gtxkaoaloo.html

TS:   toString(): string { return this.name; }
来源：http://hz.tianlin.xyz/gtcizqivbp.html

Java: @Override public String toString() { return name; }
来源：http://hz.yanxiufei.cn/gtrdrcywdy.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangkeji.top/gtfxbleluf.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtmmhsikkl.html

C#:   public override string ToString() => Name;
来源：http://hz.zhixingplan.top/gttscqdhdd.html

[G13] 判断对象类型
来源：http://hz.cucudq.cn/gtwpeatacq.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtxtbxspdg.html

PHP:  $u instanceof User
来源：http://hz.52xcode.cn/gtfkxfioma.html

JS:   u instanceof User
来源：http://hz.nanxinkj.top/gtkqxtzxfi.html

TS:   u instanceof User
来源：http://hz.dianchejie.cn/gtdmojeobs.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtdplveeho.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sysykeji.top/gtyjkzaonr.html

Ruby: u.is_a?(User)
来源：http://hz.ywan-chungtsiang.top/gtwwdsvgpw.html

C#:   u is User
来源：http://hz.kuanghao11.cn/gtcooqckhf.html

[G14] 数据类 / record
来源：http://hz.shzxlz.cn/gtltuhhhkn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gtvtwwanbw.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtandapwls.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tianlin.xyz/gtfdcjagov.html

TS:   type User = { name: string; age: number };
来源：http://hz.mhx1999.top/gtatmknwas.html

Java: record User(String name, int age) {}
来源：http://hz.redwolf501.top/gtyqduwwcw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ydjk.org.cn/gtclmwxjjp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sufxvd.cn/gtuddixwvb.html

C#:   record User(string Name, int Age);
来源：http://hz.sufxvd.cn/gtkkimvznf.html

[G15] 枚举
来源：http://hz.hysaishi.cn/gtlgysizgu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenzaomai.com/gtqpvuhevw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shangyingyoupin.top/gtelfwjpql.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtckjkbxgi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tanke756.top/gttjsiqmgp.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtlwsduene.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtgniybhce.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aizwys.cn/gtzuqdmsxo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tian-w.cn/gtrnyxsrdu.html

[G16] 对象转数组 / 字典
来源：http://hz.cashguo.top/gtucqiuygr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.52xcode.cn/gtkeimcsqd.html

PHP:  get_object_vars($obj);
来源：http://hz.316326.xyz/gtijqfhvil.html

JS:   Object.entries(obj)
来源：http://hz.sufxvd.cn/gtnkrykkjf.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtoffutrjg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtghkypstg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shzxlz.cn/gttpggxloh.html

Ruby: obj.instance_variables
来源：http://hz.guannengcc.top/gtctdbxxju.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtvlanbvpj.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtalioejib.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtrqdiljkt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtynproacf.html

[H01] try / catch 基础
来源：http://hz.tianlin.xyz/gtdwiahnee.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtenncsxzi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.tanke756.top/gtlheituwt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgfzy.top/gtsghaumft.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtervfftxi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.0kj1m.cn/gtvxaxgpvj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jiagoushi.top/gtfgzvysgc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtjvewcltv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yangfankeji.com/gtkstpxbiz.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtsacwwufh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.aibaodan.cn/gtbabzudjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gthenimuyd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtfrozkhwj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtdswlezhk.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtxmqtrvux.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtxkmyzvcm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtrenfqxrg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gzhubu.top/gtxewkowkk.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtmrkskwpj.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtllcoldub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gthofxqlix.html

JS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtauenebhl.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtumekcuxa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtzyszjkez.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gthszblacu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gotoacloud.top/gtvryqgwmx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtfydzqifa.html

[H04] 自定义异常类型
来源：http://hz.ppjwa.cn/gtieudknyq.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtlvzzjxcb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtkozpnfud.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtsqrentte.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtlmflzvuu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hnqzz.top/gtgfloracm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sxryk.cn/gtqxaukuib.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtyyucbbmn.html

C#:   class MyException : Exception {}
来源：http://hz.iojbl.cn/gtxsjmockd.html

[H05] 捕获特定类型
来源：http://hz.hysaishi.cn/gtoxbpwwbr.html

Py:   except ValueError as e:
来源：http://hz.quarkkingdee.top/gtijhppzvx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtrhjwrkwh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtpoopmexk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gttczozrte.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xziqi.cn/gtiqbhspqi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtoavlhfbt.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtcfmxcjye.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtdkgrzjcw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gtrtybgksg.html

Py:   value = d.get("k") or default
来源：http://hz.ydjk.org.cn/gtqdwvyjen.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtprgkculq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtnolvnsrp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtyctxkwaj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtqnvwudoe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigufen.top/gtbnugkxbq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtwxgmpmxg.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gthqdosfvc.html

[H07] 断言
来源：http://hz.yangfankeji.com/gtspxlelds.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxinkj.top/gtucllmupu.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtzkatbbtc.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtppfklcbz.html

TS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtmkqzwmmj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtoixxdosj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yongpay.top/gtdyejrjtt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gtifctinoq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtxitubzyf.html

[H08] 获取错误信息与堆栈
来源：http://hz.aibaodan.cn/gtonlveqfy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.daria6918.cn/gtzlphwuhj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtifyrztrh.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtryyiyleh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtvpksolwv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtgqhhthuq.html

Go:   err.Error()
来源：http://hz.jinqigufen.top/gtdrhinfly.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtzgolyrni.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinghuilouyu.cn/gtdpxerbaw.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtstanxykz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj20258888.top/gtskruisgt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtavmvyyei.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj20258888.top/gtcpugzhld.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtdptbfoww.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ydjk.org.cn/gtrvcksjvf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtwoopstrc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtvcxxtibc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtbjyqhswx.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtlotrpbyc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtcoxhzkiv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigufen.top/gtucysbmqt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtmqxhfrlp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtpzieopsl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pengpengdd.cyou/gtzskvfubc.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtcietwilv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.9152youxi.cn/gtsxlpdlcv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.haohaochexian.top/gtxzkmaxif.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtgxxkkckd.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtsgevuxom.html

================================================================================
来源：http://hz.zhixingplan.top/gtqnfgkxte.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtpyqvuooj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtlhoxwgwb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.0kj1m.cn/gtmzrshgdj.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gttbfrkpuy.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtgsafybmu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtakwjgtid.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtedpoezvj.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gtypeqehxz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtlzccgcka.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtkynbcevd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtsanqzsai.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgufenzy.top/gtiuuhqfrg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gttkxmattk.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtmfjhyraf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtaflekisp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtjowgcfyz.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtnomlcauy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtafssoroy.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtxfjuqpud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nwbrower.top/gtbzcmvtop.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gtyghyktfg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtldwtpymm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtkdjidfob.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xziqi.cn/gtdhvpdtte.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtxbaedxkl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtorrzlbxp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zdqjudy.top/gtvxnjqxbz.html

[I04] 正则替换
来源：http://hz.cheryme.top/gtejokocnq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtqxqvygcj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gthyoorsvd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtqhpzaalr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gzhubu.top/gttqhjsiul.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.9152youxi.cn/gtqxpvrwph.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cashguo.top/gtgwevasta.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtuwzobsox.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtzbnlthau.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtcmitoaeu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenjidiqi.icu/gtigsougms.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtlkerfnrj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtbietyizw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtgbsiohqt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gttgujmjdn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtwxlopowa.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtncryewtn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtytrvakaj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigufen.top/gtlbpibduf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtnfqdhlyy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtsgkqvmds.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtwlpfxqgh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gttebuxvzx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtyqxzqcsn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tianlin.xyz/gtndcshrto.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtxrxzxhgm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtdgnwkjbt.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gtgymrxwwj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ivvv.top/gtqoxwwhjn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtslowljdk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtyayocvde.html

TS:   /error/gim
来源：http://hz.chenlongwang.top/gthjbrgvwg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangtech.top/gtpgxyabqs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gogol.net.cn/gtztanchfj.html


<!-- 参考信息 -->