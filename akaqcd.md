代发 wailian999

================================================================================
来源：http://hz.ehwqpu.com/gtbptmqurq.html

G. 面向对象
来源：http://hz.zhoulong.xyz/gtubzrokmn.html

================================================================================
来源：http://hz.tianlin.xyz/gtthffpctc.html

[G01] 定义类
来源：http://hz.zycfv.cn/gtlvqgxrkc.html

Py:   class User: pass
来源：http://hz.yj20258888.top/gtefwvlugk.html

PHP:  class User {}
来源：http://hz.jinyuanbaomall.cn/gtkjommuie.html

JS:   class User {}
来源：http://hz.chenzaomai.com/gtpkyrrbcf.html

TS:   class User { name: string = ""; }
来源：http://hz.dashuyun.cn/gtpnufhroi.html

Java: class User {}
来源：http://hz.xinyue.icu/gtmqwszxsm.html

Go:   type User struct { Name string }
来源：http://hz.pycfn.com/gtwixqqbrx.html

Ruby: class User; end
来源：http://hz.shanyushiyangtech.top/gtdpzejzdo.html

C#:   class User {}
来源：http://hz.nanxuanxn.top/gtpeutbcij.html

[G02] 构造函数
来源：http://hz.mhx1999.top/gtxgyfbjbz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtotzaznxj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hnqzz.top/gtbzuxwjhw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuanzx.com/gtfknuavff.html

TS:   constructor(public name: string) {}
来源：http://hz.fengsongda.top/gthmnfxxcr.html

Java: User(String name) { this.name = name; }
来源：http://hz.jiagoushi.top/gtdidkrzff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtxciagemg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cdnleiting.top/gtcmmigdfu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtadikszne.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gtauqpbehm.html

Py:   self.name = "x"
来源：http://hz.guowangkeji.top/gtavisvfeo.html

PHP:  public string $name = "x";
来源：http://hz.zhixingplan.top/gtcgfiiohi.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtnqfjxhzu.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtxvwvzcfx.html

Java: private String name;
来源：http://hz.zhijiandao.cn/gtrwtbobyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sxryk.cn/gttevxuykr.html

Ruby: @name = "x"
来源：http://hz.zhoulong.xyz/gtqtdfkden.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yj202588.top/gtaqfwwabe.html

[G04] 定义方法
来源：http://hz.hammf.cn/gtccajrimz.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtarlmmlim.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gtaiilekmg.html

JS:   greet() { return this.name; }
来源：http://hz.sufxvd.cn/gtneqpqvme.html

TS:   greet(): string { return this.name; }
来源：http://hz.gotoacloud.top/gteseprdmr.html

Java: String greet() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtostpkswt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.0kj1m.cn/gtsxabhqnc.html

Ruby: def greet; @name; end
来源：http://hz.cashguo.top/gtseszeiyn.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtiswztffa.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtpaagcazy.html

Py:   class Admin(User): pass
来源：http://hz.zhengqikj.top/gtmuzshkoj.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtzqtkyfso.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtopdhncec.html

TS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtlyragckj.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtbzikxvck.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxuanxn.top/gtflqlogcl.html

Ruby: class Admin < User; end
来源：http://hz.ybcxt.top/gtpymdzbct.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtteglbrxr.html

[G06] 重写方法
来源：http://hz.vqdsnc.cn/gtnjydhmzm.html

Py:   def greet(self): return "admin"
来源：http://hz.kuanghao11.cn/gtrowshwfa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gogol.net.cn/gtdfpqkjst.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtqaccbyyy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtmgzaftmm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenjidiqi.icu/gteewxsgag.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.daxiang520.top/gtilaexloi.html

Ruby: def greet; "admin"; end
来源：http://hz.jinqigfzy.top/gtfkztnlwz.html

C#:   public override string Greet() => "admin";
来源：http://hz.dianchejie.cn/gtlsohdfjk.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtjsjdrymm.html

Py:   super().greet()
来源：http://hz.zhijiandao.cn/gtmjqrwdvp.html

PHP:  parent::greet();
来源：http://hz.jinghuilouyu.cn/gtlpuaxair.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gtsefmyxlg.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtlhtaznep.html

Java: super.greet();
来源：http://hz.jqgfzy.top/gtjoezjyxn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xinyue.icu/gtolnrbzkb.html

Ruby: super
来源：http://hz.xingfuxueyuan.xyz/gtgkhvzlri.html

C#:   base.Greet();
来源：http://hz.guannengcc.top/gtkwtheaex.html

[G08] 静态方法与属性
来源：http://hz.jinyuanbaomall.cn/gtuokmabat.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuetiantiany.cn/gtzuqnysmk.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gtuyxgoodx.html

JS:   static f() {}
来源：http://hz.sxryk.cn/gttskefyte.html

TS:   static f(): void {}
来源：http://hz.dianchejie.cn/gtdrlklhjl.html

Java: static void f() {}
来源：http://hz.hfpthk.cn/gttrdhwjqc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenjidiqi.icu/gtcjdafnuw.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gtnavrfwct.html

C#:   public static void F() {}
来源：http://hz.iojbl.cn/gtksdbycia.html

[G09] 接口 / 抽象类
来源：http://hz.svipenyu.cn/gtbndbprhz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hnqzz.top/gtihftawob.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jlsjyb.cn/gtdvglspky.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yonumen.top/gtukbmijxv.html

TS:   interface Shape { area(): number; }
来源：http://hz.fzhhl.top/gtkeibilso.html

Java: interface Shape { double area(); }
来源：http://hz.shzxlz.cn/gttkkpnhkg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtglvcjrtt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtfrvjoxgp.html

C#:   interface IShape { double Area(); }
来源：http://hz.wangdashe.top/gtaxyzqimq.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtpepfeccs.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.fzhhl.top/gtpxwlvnca.html

PHP:  public / protected / private
来源：http://hz.0kj1m.cn/gttfuvlveq.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtrggzajmg.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtsurbzoui.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtuifwqgbp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gaohongyu789.top/gtswethsgf.html

Ruby: public / protected / private
来源：http://hz.zhongyouzk.top/gtrxjepqbd.html

C#:   public / protected / private / internal
来源：http://hz.birdmap.top/gtkpcwitpp.html

[G11] getter / setter
来源：http://hz.sweek.top/gtfpoiqvoq.html

Py:   @property 与 @x.setter
来源：http://hz.bjfxy.top/gtpnatvoel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gttknspqni.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtyrusknew.html

TS:   get name(): string { return this._name; }
来源：http://hz.shzxlz.cn/gtanaaztod.html

Java: public String getName() { return name; }
来源：http://hz.xziqi.cn/gtmzcitfyt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.cqqwz.cn/gtnrhqjifj.html

Ruby: attr_accessor :name
来源：http://hz.shanyushiyangkeji.top/gtntlkeobw.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtrqtxgxty.html

[G12] 对象转字符串
来源：http://hz.svipenyu.cn/gtcwlstlfg.html

Py:   def __str__(self): return self.name
来源：http://hz.yvedp.cn/gtxxazwpzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtedbegkif.html

JS:   toString() { return this.name; }
来源：http://hz.xuanzx.com/gtpnqinutc.html

TS:   toString(): string { return this.name; }
来源：http://hz.jianghu66.top/gtpziinify.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtepaswbrz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guowangkeji.top/gtjomqhwir.html

Ruby: def to_s; @name; end
来源：http://hz.hywenlv.cn/gteuvureck.html

C#:   public override string ToString() => Name;
来源：http://hz.yonumen.top/gtnrrozxpl.html

[G13] 判断对象类型
来源：http://hz.yj20258.top/gthdrzsvdd.html

Py:   isinstance(u, User)
来源：http://hz.fengsongda.top/gtekdypnsi.html

PHP:  $u instanceof User
来源：http://hz.hysaishi.cn/gtssszugbv.html

JS:   u instanceof User
来源：http://hz.pengpengdd.cyou/gtwsklykmx.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gteetuyczk.html

Java: u instanceof User
来源：http://hz.jinqigufen.top/gtkbevgeqw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtjistonfp.html

Ruby: u.is_a?(User)
来源：http://hz.ehwqpu.com/gtofhseafl.html

C#:   u is User
来源：http://hz.cashguo.top/gtrazjeuxa.html

[G14] 数据类 / record
来源：http://hz.zdqjudy.top/gttsauogqh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yj20258.top/gtkrhtzyvv.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sufxvd.cn/gtxwjetjnv.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shanyushiyangtech.top/gtwcekphnx.html

TS:   type User = { name: string; age: number };
来源：http://hz.sxryk.cn/gtiilfisja.html

Java: record User(String name, int age) {}
来源：http://hz.jinghuilouyu.cn/gteylhvonl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangshuangyany.cn/gtswcrhqmu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jianghu66.top/gtwjueuznm.html

C#:   record User(string Name, int Age);
来源：http://hz.yueranfly.top/gtdhynqhtx.html

[G15] 枚举
来源：http://hz.0kj1m.cn/gtrqhqcfub.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtdkqhypoi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtxcytwcqz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtalqhffgx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxuanxn.top/gttgoorxkq.html

Java: enum Color { RED, GREEN }
来源：http://hz.hywenlv.cn/gtpvirlodv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258888.top/gtncdvnjmg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtwkfundhi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hywenlv.cn/gtzqglmytc.html

[G16] 对象转数组 / 字典
来源：http://hz.wangshuangyany.cn/gtqujtucdy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtirlwauhe.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtihithwgp.html

JS:   Object.entries(obj)
来源：http://hz.gotoacloud.top/gtqdmlkaiw.html

TS:   Object.entries(obj)
来源：http://hz.mhx1999.top/gthdbjglza.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shanyushiyangkeji.top/gtoygnavhq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.c1oappe.top/gtcndyqdoi.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gtyasmcjdb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnxiangtu.top/gtibkonauk.html

================================================================================
来源：http://hz.zdqjudy.top/gtvweviucs.html

H. 异常与错误处理
来源：http://hz.sysykeji.top/gttaqjduwd.html

================================================================================
来源：http://hz.jyoumei.cn/gtsdtrjsrd.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtfcwaltya.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtdzicnuti.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydjk.org.cn/gtwuexceny.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtryrbrkwz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtkbjoplss.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gzhubu.top/gtutbflxem.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtltcrtmvl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtmqnkzgol.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtndydnnmc.html

[H02] finally / ensure 收尾
来源：http://hz.sufxvd.cn/gtisudjzha.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jiagoushi.top/gtsmjbjnzv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtyrufjbgw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtkfqmgras.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtdwrhrpfo.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtiqlpavgs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhongyouzk.top/gtixubnmhr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gttzxmwgum.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtxphnoovz.html

[H03] 主动抛出异常
来源：http://hz.mhx1999.top/gtmucjgrgx.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtxcdlhely.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtqcacbxpw.html

JS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtknrevlev.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtbmvwrjqj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtbrebfwpb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shzxlz.cn/gthfpasvyo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.pengpengdd.cyou/gtxpkpopou.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gtuqbwcwct.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtvanlbsqr.html

Py:   class MyError(Exception): pass
来源：http://hz.0kj1m.cn/gtgqouyjnu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gteeemdcra.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtgqfffqan.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtwcwnbzwf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.vqdsnc.cn/gtjjayoivz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ywan-chungtsiang.top/gtjyxywdtx.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhaomingkeji.xyz/gtyrmlvfob.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtpnkxaovj.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtwqgfrubl.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtcmaoqwdb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.0kj1m.cn/gtqtxkydpf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtqcmjijgd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtvaswicyq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtsblticir.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenlongwang.top/gtuhawiggc.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtjgznffpc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gthrxpjpnt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtcpvqnsjm.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gtmcqspett.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.iojbl.cn/gtydoovjwr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtwbjarvcd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtomrkvtdf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtgxxefqls.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtenfycmpt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhaomingkeji.xyz/gtynwqatrd.html

C#:   obj?.A?.B ?? default
来源：http://hz.yvedp.cn/gtruougzkm.html

[H07] 断言
来源：http://hz.yj20258888.top/gtxufhckhe.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtzzdvxxvl.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gtufmrtvto.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtanbytmjn.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gttmgnvcrj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gzhubu.top/gtqnechcpa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.c1oappe.top/gtfxuyeocl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtruchkdop.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hywenlv.cn/gtmymmpyxs.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtmhwxvbfw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yangfankeji.com/gthighrafp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.316326.xyz/gtakrxpzdl.html

JS:   e.message;  e.stack
来源：http://hz.yuanzhike.top/gttuqzhmkc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtqdsdmjqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pengpengdd.cyou/gtiuaufopb.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtjrfzywmm.html

Ruby: e.message;  e.backtrace
来源：http://hz.nwbrower.top/gtrndvyvcy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtmemfmxpx.html

[H09] 带错误码的异常
来源：http://hz.ppjwa.cn/gthimlqkji.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtybwtkqru.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hammf.cn/gtozcnycoc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnxiangtu.top/gtljljhfbj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtvaceadiu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtqsmvqqcj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtkvsxihpf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtlzmzrxyl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtfiozvyvm.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gttiuhzjkr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxuanxn.top/gtiecewdlt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cashguo.top/gtjbatmmni.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtgyfzebht.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gtuzkknczi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuetiantiany.cn/gtjevifhtx.html

Go:   defer f.Close()
来源：http://hz.cdnleiting.top/gtjgzrhvcn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtpteavxag.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtafitcied.html

================================================================================
来源：http://hz.yonumen.top/gthhjhwhpt.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtkdooutlw.html

================================================================================
来源：http://hz.ydzc1.top/gtlgwilyhi.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtnpvxzvyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sxryk.cn/gtbjwesjon.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtcmjtedzy.html

JS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtdmsczorq.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtaehowjmn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gtyercnjpz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtvyjlkxlf.html

Ruby: s.match?(/\d+/)
来源：http://hz.pycfn.com/gtmimakgnm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtpcorrbcz.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtcnldmwma.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtabgknhqa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gthsdiilxf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tianlin.xyz/gtrmhijcbz.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtyxivtmuc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtkwmzzlbr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gtkdvwtska.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gtylgnruld.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtjdkcncqv.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtgmcaakpr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtxmeicmnw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cheryme.top/gtrafhmdra.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtaslskvle.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtpebxytfk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gteryeilri.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtcsaprtsj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtzteksggz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtbmchfetf.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtbvshysxp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cqqwz.cn/gtbnxwifxe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtjqowakzn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtofcvrgyj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aizwys.cn/gtebenfixl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtojbujknh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shanyushiyangtech.top/gtqwbvylzh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.haohaochexian.top/gtjvrcabum.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuxming.cn/gtjtwgouii.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtlapzvjpv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtonfdwguf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtifqaqfne.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtjzrsdeio.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.iojbl.cn/gtijgsjnoe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gtpvmgckej.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gteihhcxig.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtanglpvpu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gzhubu.top/gtltzkngod.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtwmrlqvfc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtieodgjpz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pengpengdd.cyou/gtplzdhomv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtutbzzdym.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtavczizkx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtjmcxgeyv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hammf.cn/gtfpnttgga.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.52xcode.cn/gtckoimekz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gtwdqcyvwl.html

[I07] 忽略大小写与多行模式
来源：http://hz.chenjidiqi.icu/gtvpbmxblp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtnyczugrh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtlvfoqbux.html


<!-- 参考信息 -->