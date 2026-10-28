代发 wailian999

JS:   this.name = "x";
来源：http://hz.daxiang520.top/gtzitwqajw.html

TS:   name: string = "x";
来源：http://hz.sxryk.cn/gtqyexfead.html

Java: private String name;
来源：http://hz.ivvv.top/gtaxbcoluw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.nanxinkj.top/gtaqkdbkif.html

Ruby: @name = "x"
来源：http://hz.zycfv.cn/gtcexzebpc.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shangyingyoupin.top/gtceqzplgd.html

[G04] 定义方法
来源：http://hz.jqgfzy.top/gtajqcoqcg.html

Py:   def greet(self): return self.name
来源：http://hz.meibo888.top/gtlzkospdv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.redwolf501.top/gtrrhqnhrf.html

JS:   greet() { return this.name; }
来源：http://hz.nanxuanxn.top/gtgqodqcto.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtmogfscve.html

Java: String greet() { return name; }
来源：http://hz.hywenlv.cn/gtfkkitcmi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtuwakenbh.html

Ruby: def greet; @name; end
来源：http://hz.fzhhl.top/gtjmgkavph.html

C#:   public string Greet() => Name;
来源：http://hz.yuanzhike.top/gtkokonblh.html

[G05] 继承
来源：http://hz.jinqigfzy.top/gtxfotdzkx.html

Py:   class Admin(User): pass
来源：http://hz.sysykeji.top/gtbjcxlhrw.html

PHP:  class Admin extends User {}
来源：http://hz.ydjk.org.cn/gtbnjpvjvl.html

JS:   class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtybtiueca.html

TS:   class Admin extends User {}
来源：http://hz.9152youxi.cn/gtgmiavlgo.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtwnfsounk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yj20258.top/gtokigchbt.html

Ruby: class Admin < User; end
来源：http://hz.hnxiangtu.top/gtolefdobr.html

C#:   class Admin : User {}
来源：http://hz.yvedp.cn/gtwhzuzyok.html

[G06] 重写方法
来源：http://hz.cucudq.cn/gtriuyfmwf.html

Py:   def greet(self): return "admin"
来源：http://hz.zhixingplan.top/gthvpuhnfj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.cqqwz.cn/gtielvlbkw.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtmmnrvqwu.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gteefccfea.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hammf.cn/gtzkzpgxcn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtzybxxtnt.html

Ruby: def greet; "admin"; end
来源：http://hz.yueranfly.top/gtygueciet.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhengqikj.top/gtnqokhrdu.html

[G07] 调用父类方法
来源：http://hz.zhixingplan.top/gtwmqalwar.html

Py:   super().greet()
来源：http://hz.nwbrower.top/gtvnprgzsd.html

PHP:  parent::greet();
来源：http://hz.birdmap.top/gtxqmeqjxz.html

JS:   super.greet();
来源：http://hz.zhoulong.xyz/gtqibnvuqs.html

TS:   super.greet();
来源：http://hz.pycfn.com/gtivbuduxi.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtpjkmqcjs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daxiang520.top/gtiqeadtvx.html

Ruby: super
来源：http://hz.tanke756.top/gtuwzzgdky.html

C#:   base.Greet();
来源：http://hz.aizwys.cn/gthidqgpaj.html

[G08] 静态方法与属性
来源：http://hz.zhiwuduotai.top/gtjlfvtevi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.tianlin.xyz/gtqcvauzyl.html

PHP:  public static function f() {}
来源：http://hz.yuanzhike.top/gtwcakignq.html

JS:   static f() {}
来源：http://hz.guowangkeji.top/gtmofciyzf.html

TS:   static f(): void {}
来源：http://hz.snrcjt.cn/gtucendlsa.html

Java: static void f() {}
来源：http://hz.hongshengwenyu.top/gtucvsptcu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.vqdsnc.cn/gtqylefgcj.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtlrjzdcnp.html

C#:   public static void F() {}
来源：http://hz.zhixingplan.top/gtanqkjfsg.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtzsdtbjwu.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtqjkfsdbr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tianlin.xyz/gthlrklbty.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtpiwjevzq.html

TS:   interface Shape { area(): number; }
来源：http://hz.hywenlv.cn/gtrphpcmhj.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gtuktigrjy.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.kuanghao11.cn/gthqlmzzlr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ehwqpu.com/gtdhlnrtry.html

C#:   interface IShape { double Area(); }
来源：http://hz.jiagoushi.top/gtjueyznzf.html

[G10] 访问控制
来源：http://hz.cqqwz.cn/gtkggenixc.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.daria6918.cn/gtzxurlihs.html

PHP:  public / protected / private
来源：http://hz.zhoulong.xyz/gtvxzeobub.html

JS:   #private 字段；其余公开
来源：http://hz.fengsongda.top/gtdgaykacs.html

TS:   public / protected / private
来源：http://hz.ydzc1.top/gtsfckkodi.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtnblhtqnm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtcdfrtwim.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gthbdzgrum.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtphnssnjh.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtplxkltzd.html

Py:   @property 与 @x.setter
来源：http://hz.hfpthk.cn/gtweqwssbf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhixingplan.top/gtwpbanlgd.html

JS:   get name() { return this._name; }
来源：http://hz.hongshengwenyu.top/gtlqgabrth.html

TS:   get name(): string { return this._name; }
来源：http://hz.quarkkingdee.top/gtffdlwvav.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtdfswmvhj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hnqzz.top/gtcpwukilk.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtxerazskj.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtxwbiykze.html

[G12] 对象转字符串
来源：http://hz.chenjidiqi.icu/gtyfxjoojr.html

Py:   def __str__(self): return self.name
来源：http://hz.pengpengdd.cyou/gtzgrtcqwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtgbinjpdt.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtmdnzmfbo.html

TS:   toString(): string { return this.name; }
来源：http://hz.hongshengwenyu.top/gtgnpzssdy.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydzc1.top/gttkxzxaix.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gtduvnmnaf.html

Ruby: def to_s; @name; end
来源：http://hz.shanyushiyangkeji.top/gtyqhoouzo.html

C#:   public override string ToString() => Name;
来源：http://hz.sxryk.cn/gtyidebstl.html

[G13] 判断对象类型
来源：http://hz.chenlongwang.top/gtgytsxuty.html

Py:   isinstance(u, User)
来源：http://hz.smart0.xyz/gtnoawyesj.html

PHP:  $u instanceof User
来源：http://hz.cdnleiting.top/gtghdpkmfh.html

JS:   u instanceof User
来源：http://hz.yj20258888.top/gteosmwzsx.html

TS:   u instanceof User
来源：http://hz.gotoacloud.top/gtxbcjxlix.html

Java: u instanceof User
来源：http://hz.cucudq.cn/gtifrofqsr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.haohaochexian.top/gtplsxnamc.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtmhpnendq.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtbxvnuquh.html

[G14] 数据类 / record
来源：http://hz.52xcode.cn/gtomakcjlf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.316326.xyz/gtydeawjng.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gthalactxn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gteaojnpch.html

TS:   type User = { name: string; age: number };
来源：http://hz.hnxiangtu.top/gtraasjjtm.html

Java: record User(String name, int age) {}
来源：http://hz.ehwqpu.com/gtydrdzkif.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gotoacloud.top/gtfkuzqxyz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhixingplan.top/gtbprruyin.html

C#:   record User(string Name, int Age);
来源：http://hz.aibaodan.cn/gtwzjenjvj.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gticprbvpr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgfzy.top/gtcocktjzc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cucudq.cn/gtbdglujlr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jiagoushi.top/gttebosrsy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jianghu66.top/gtpbojcscc.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtdcgglfgj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.pycfn.com/gtjenhbqcf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.feifeiyinyue.top/gtbtvzvnlf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jyoumei.cn/gtyftdzrbl.html

[G16] 对象转数组 / 字典
来源：http://hz.ydzc1.top/gtochygfxt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ivvv.top/gttyvjswri.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtfrjvnqbt.html

JS:   Object.entries(obj)
来源：http://hz.52xcode.cn/gtrrqskptb.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtyqscjhmf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtuajgfjbf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.birdmap.top/gtnowsgspx.html

Ruby: obj.instance_variables
来源：http://hz.hysaishi.cn/gtlkswmams.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yuanzhike.top/gtznerfryl.html

================================================================================
来源：http://hz.zhixingplan.top/gtstccgvpy.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtxwesjogz.html

================================================================================
来源：http://hz.smart0.xyz/gtxqjlzfbj.html

[H01] try / catch 基础
来源：http://hz.zycfv.cn/gtbbtzeeaa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gteljcqgwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jqgfzy.top/gthkfjayaw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtljkdcvlb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtbtlqtzlg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.guowangkeji.top/gtwiymisbb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xziqi.cn/gtufjqldik.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtlrvgxryh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtuxhqkqhz.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtrixftbnj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.vqdsnc.cn/gtrhcsykwy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtkontdbmw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtlfjmmrrm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenjidiqi.icu/gtykqolxgq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtpgrqguay.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtiboniyet.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxuanxn.top/gthgnonbqg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.meibo888.top/gtknszkxaf.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gtcztoxnrj.html

Py:   raise ValueError("错误信息")
来源：http://hz.xylfe.cn/gtoomehyhq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtdeviwlbs.html

JS:   throw new Error("错误信息");
来源：http://hz.svipenyu.cn/gtukozkibn.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtdrzkddfw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtnlsfdqig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ehwqpu.com/gthodcqpjq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhongyouzk.top/gtirpkohrp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtffsqmtee.html

[H04] 自定义异常类型
来源：http://hz.zhijiandao.cn/gtnbajazyz.html

Py:   class MyError(Exception): pass
来源：http://hz.zhijiandao.cn/gtxpdeefrl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtzeonydfn.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gthxlmyqct.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtwuikhuvo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtrxlvhmzm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.redwolf501.top/gtisubcafv.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gttlcnlrve.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtunzrrpzn.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtbqlmiovq.html

Py:   except ValueError as e:
来源：http://hz.ywan-chungtsiang.top/gtjytbeudg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtkxfwcuhe.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.aibaodan.cn/gtjbohbehv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtghsenbwg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zdqjudy.top/gtwuxqwldf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pengpengdd.cyou/gtqcmqivva.html

Ruby: rescue ArgumentError => e
来源：http://hz.ppjwa.cn/gtgktyszos.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gzhubu.top/gtaavwvqzm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnqzz.top/gthfrnnlzc.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtrxezwmmi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gthttobigi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gttoppurvf.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtvwlnowtt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuetiantiany.cn/gtfmdosgth.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.svipenyu.cn/gtdlxjguvn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xylfe.cn/gtguapkrxg.html

C#:   obj?.A?.B ?? default
来源：http://hz.hysaishi.cn/gtaenivwqf.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gtjfvrlkkw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtnmcfcjkc.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtyhnqrwdz.html

JS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtgfobkgrc.html

TS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtnwzyavep.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtauxhxsdm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jlsjyb.cn/gtfrtwagvo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.haohaochexian.top/gtrsnybblh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtjfvdfdrf.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtbemymhgy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtcswohvyl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtxlcoxzry.html

JS:   e.message;  e.stack
来源：http://hz.jqgfzy.top/gtztwtdixk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtpmuntjjo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guannengcc.top/gtxnfqlfgk.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtmjprjcod.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gtuhxqeqyf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tanke756.top/gtytdpnduj.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gthebtjgfz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gthwxnuxqo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nanxinkj.top/gttmhvdxpr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtarjqurmv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gogol.net.cn/gtjskkcjza.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gtscckpynh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtbdvywdew.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtrtfrusxw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gttdarcmyc.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtkhwqbrgu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtmaepkbfn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtkwkcofan.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtqwzbnujo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtaoltiwqu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtipkuqqbm.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtxyczzzcf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtysblufwt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtnzemdvco.html

================================================================================
来源：http://hz.jiagoushi.top/gtycckjapu.html

I. 正则表达式
来源：http://hz.jinqigufen.top/gtmnpfrahj.html

================================================================================
来源：http://hz.ehwqpu.com/gtqotbdeie.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtgqpffspw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.haohaochexian.top/gtbicvgjft.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258888.top/gtodfftukn.html

JS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtuemqrter.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtfkvdxmxr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtwqsljyfg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtdnjepfio.html

Ruby: s.match?(/\d+/)
来源：http://hz.ppjwa.cn/gtqsekawfi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sysykeji.top/gtjmvfmhxd.html

[I02] 提取所有匹配
来源：http://hz.guowangkeji.top/gtrhdynczs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gterrhysqb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtfdsgswbl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtyytpvhwe.html

TS:   s.match(/\d+/g)
来源：http://hz.nanxinkj.top/gtjhbuvsgn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shangyingyoupin.top/gtlhifeqyd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxinkj.top/gtlxukauiu.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtcztnosuc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gtlebdcxhk.html

[I03] 提取捕获分组
来源：http://hz.quarkkingdee.top/gtylorjiii.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pengpengdd.cyou/gtsijoqqzx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gttcvlzqxj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtwdrwsizh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gtbmxciooj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.mhx1999.top/gtfwqpsbez.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtvrthegrz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtwjjrhjul.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.smart0.xyz/gtqtnlpcvv.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtbkbghfek.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gtxxkzpfhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ivvv.top/gthkvhmmrq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtjxojqfib.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gththbkwnm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtdfjpkxsd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.316326.xyz/gtckpdbbgk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.mhx1999.top/gtabwcedes.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gtqfnnfzll.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtdxuidvql.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtkmnxfqsf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gthzxgxjbf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtaiisludw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtliuemujm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtwefbiewf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtqoxixvkm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtxqucrpum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cucudq.cn/gtkpxefzxq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.daria6918.cn/gtpgfojvbo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.quarkkingdee.top/gtvtrqpjee.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtyqjqtjez.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtndxohhmh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtediqqbnq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtcuhxgmdy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtddmpplro.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cdnleiting.top/gtzdnjzdyc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gttggvnejs.html

[I07] 忽略大小写与多行模式
来源：http://hz.yuanzhike.top/gtoivfezxr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cdnleiting.top/gtbjwhguti.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtmvkgddwh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtmudcnewm.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtjyraovbn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtllacctvz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtozpixbpo.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangkeji.top/gtmebxhjvp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.snrcjt.cn/gtwkxlrufb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gtitehbxxv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.iojbl.cn/gtsexpxzfl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hammf.cn/gtkfmnocol.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtwzpfawld.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhixingplan.top/gtkvnfsepy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xylfe.cn/gtadyyntlv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gtntpdgxso.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtkyvtjgxj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtgdptwbjz.html

================================================================================
来源：http://hz.havefunace.top/gttiwocqdq.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtrspxqvud.html

================================================================================
来源：http://hz.cucudq.cn/gtehsgeupm.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtdxidhtur.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sufxvd.cn/gtoowrfxbl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtiqyqnsli.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtycqkfqsf.html

TS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtokahpkoy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.bjfxy.top/gtzmrcblni.html


<!-- 参考信息 -->