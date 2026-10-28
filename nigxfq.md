代发 wailian999

[G02] 构造函数
来源：http://hz.quarkkingdee.top/gtgshdhdkw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.hfpthk.cn/gtggwzbfta.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xylfe.cn/gtuoodpqyt.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtrzzyrdyx.html

TS:   constructor(public name: string) {}
来源：http://hz.jinqigfzy.top/gtxuzmtegn.html

Java: User(String name) { this.name = name; }
来源：http://hz.hywenlv.cn/gtrmmxaclt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.havefunace.top/gtcifpcxnw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtofhdxcnd.html

C#:   public User(string name) { Name = name; }
来源：http://hz.birdmap.top/gtvkasuotg.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gthdfefssi.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtyvjthkag.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtjbvectrm.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtrifntrpi.html

TS:   name: string = "x";
来源：http://hz.nwbrower.top/gtinmbcmpc.html

Java: private String name;
来源：http://hz.hywenlv.cn/gtssbeevjj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtxhqzxzkj.html

Ruby: @name = "x"
来源：http://hz.andypj.xyz/gtyjismpue.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hysaishi.cn/gtwugbvzlz.html

[G04] 定义方法
来源：http://hz.sweek.top/gtjfnwcsuv.html

Py:   def greet(self): return self.name
来源：http://hz.chenlongwang.top/gtrymwemnr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shanyushiyangkeji.top/gtuushcksf.html

JS:   greet() { return this.name; }
来源：http://hz.aizwys.cn/gtsynolqgt.html

TS:   greet(): string { return this.name; }
来源：http://hz.jlsjyb.cn/gtofhnhpdd.html

Java: String greet() { return name; }
来源：http://hz.yj20258.top/gtcpqwppdm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtyrqypbem.html

Ruby: def greet; @name; end
来源：http://hz.zhongyouzk.top/gtslslcmpm.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtwajvjhkp.html

[G05] 继承
来源：http://hz.smart0.xyz/gtmpooelrf.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtmhefolsg.html

PHP:  class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gthqdjopqv.html

JS:   class Admin extends User {}
来源：http://hz.yueranfly.top/gtsulzybzr.html

TS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gtetxrndoi.html

Java: class Admin extends User {}
来源：http://hz.yvedp.cn/gtjecbgncs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtukvfyyoy.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtvkcunmvs.html

C#:   class Admin : User {}
来源：http://hz.sufxvd.cn/gtqponneeu.html

[G06] 重写方法
来源：http://hz.dashuyun.cn/gtnvgarmlw.html

Py:   def greet(self): return "admin"
来源：http://hz.quarkkingdee.top/gtuhuogcqh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.xinyue.icu/gtdokgrocb.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtttiwgbfo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.aibaodan.cn/gtzcwfhmml.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtrngatfhn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtycsbivtn.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtaqvsvity.html

C#:   public override string Greet() => "admin";
来源：http://hz.zdqjudy.top/gtvmxlucpd.html

[G07] 调用父类方法
来源：http://hz.zhijiandao.cn/gtmfweiamk.html

Py:   super().greet()
来源：http://hz.shangyingyoupin.top/gtqpfmkmji.html

PHP:  parent::greet();
来源：http://hz.nwbrower.top/gtjwsnarux.html

JS:   super.greet();
来源：http://hz.dianchejie.cn/gtgomjmcjo.html

TS:   super.greet();
来源：http://hz.yanxiufei.cn/gtaxefotkk.html

Java: super.greet();
来源：http://hz.sysykeji.top/gttuhibtkp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtyaoldidc.html

Ruby: super
来源：http://hz.sufxvd.cn/gtfcndvaco.html

C#:   base.Greet();
来源：http://hz.hywenlv.cn/gtqorxdacd.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtmvureoum.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnqzz.top/gtaashfwhb.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtiukgqmxc.html

JS:   static f() {}
来源：http://hz.nanxinkj.top/gtrayqracj.html

TS:   static f(): void {}
来源：http://hz.redwolf501.top/gtdtylufvh.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gtmkbcmsee.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtywkaujqv.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtikaxipft.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtixnojzix.html

[G09] 接口 / 抽象类
来源：http://hz.nanxinkj.top/gtlciiisyb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gteykwtsvj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hammf.cn/gtaotcffpu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.52xcode.cn/gtxezesgjd.html

TS:   interface Shape { area(): number; }
来源：http://hz.svipenyu.cn/gtuqvxmljs.html

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtxpmrjrxf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.tanke756.top/gtvrwtiijf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtsggsbtjl.html

C#:   interface IShape { double Area(); }
来源：http://hz.xziqi.cn/gtzpafvvda.html

[G10] 访问控制
来源：http://hz.shzxlz.cn/gtactoekuj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gthqzmwvak.html

PHP:  public / protected / private
来源：http://hz.ehwqpu.com/gtgqfwtoqc.html

JS:   #private 字段；其余公开
来源：http://hz.hammf.cn/gtlpdqhvxu.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtanbkkqtu.html

Java: public / protected / private / 默认包级
来源：http://hz.shzxlz.cn/gtvurixukp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zycfv.cn/gtipibyqmz.html

Ruby: public / protected / private
来源：http://hz.9152youxi.cn/gtehfpopqr.html

C#:   public / protected / private / internal
来源：http://hz.sweek.top/gtvryctvfl.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtrahqxqun.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtixgxhnjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtaknpdnai.html

JS:   get name() { return this._name; }
来源：http://hz.xylfe.cn/gtzxrrtmyk.html

TS:   get name(): string { return this._name; }
来源：http://hz.guowangkeji.top/gtefwmktvj.html

Java: public String getName() { return name; }
来源：http://hz.aibaodan.cn/gtxidfjqqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.fengsongda.top/gtxelobnvv.html

Ruby: attr_accessor :name
来源：http://hz.ywan-chungtsiang.top/gtnocsjlsi.html

C#:   public string Name { get; set; }
来源：http://hz.chenlongwang.top/gthahaostm.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtazferdzg.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtltdcwwdu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigufen.top/gtzzrqhqwj.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gtozqbhchj.html

TS:   toString(): string { return this.name; }
来源：http://hz.guowangkeji.top/gtbvvxtfug.html

Java: @Override public String toString() { return name; }
来源：http://hz.yuanzhike.top/gtqjmedykp.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.guannengcc.top/gtwmzbgmem.html

Ruby: def to_s; @name; end
来源：http://hz.chenlongwang.top/gtqtjgokms.html

C#:   public override string ToString() => Name;
来源：http://hz.meibo888.top/gtnkhovvqu.html

[G13] 判断对象类型
来源：http://hz.hammf.cn/gtvaskvqhq.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtnhfvrkhh.html

PHP:  $u instanceof User
来源：http://hz.jinqigufen.top/gtlhgrodae.html

JS:   u instanceof User
来源：http://hz.fzhhl.top/gthvjrqcin.html

TS:   u instanceof User
来源：http://hz.hysaishi.cn/gtsqrrgrak.html

Java: u instanceof User
来源：http://hz.9152youxi.cn/gtetfhnrdi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.wangdashe.top/gtddinhxgs.html

Ruby: u.is_a?(User)
来源：http://hz.redwolf501.top/gtmlrwsgfx.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtylivxoyr.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtqusfjcav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.birdmap.top/gtcsrrdldo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.tian-w.cn/gtlpgxmlwa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtjxjlikjq.html

TS:   type User = { name: string; age: number };
来源：http://hz.fengsongda.top/gtpujxmpgx.html

Java: record User(String name, int age) {}
来源：http://hz.birdmap.top/gttkosqscf.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sysykeji.top/gtwmzwvund.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ppjwa.cn/gtoalkjxoa.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtducjryid.html

[G15] 枚举
来源：http://hz.yangfankeji.com/gtmovfrnsw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.chenjidiqi.icu/gtsyhzjbtl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gtsinqviqk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtjagwotnx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtbgknwejz.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtnfctkitp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhoulong.xyz/gtdtxezrbl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtmholwrvn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gtwgzvewhe.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtgcmkwxma.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jiagoushi.top/gtecvycahu.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxinkj.top/gtfgmnobqr.html

JS:   Object.entries(obj)
来源：http://hz.ydjk.org.cn/gtzpqlwkhb.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtnycpzjiu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtgslbtcsx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtyevrhnxc.html

Ruby: obj.instance_variables
来源：http://hz.pengpengdd.cyou/gtyfjawpvw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.daxiang520.top/gtijxpbkdy.html

================================================================================
来源：http://hz.yonumen.top/gtyaugxkff.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtromofbim.html

================================================================================
来源：http://hz.ybcxt.top/gtedzhzgku.html

[H01] try / catch 基础
来源：http://hz.sxryk.cn/gtppqiepiq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.smart0.xyz/gtfeezfnpi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.dashuyun.cn/gtnbhsfawp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtxxpaqluk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtwtxhtukm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gtkhydfxcv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuetiantiany.cn/gtiteoaalg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtlwexjbgv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtpxfyjbfa.html

[H02] finally / ensure 收尾
来源：http://hz.yanxiufei.cn/gtpkqxvwwk.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtyiswfkwl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtzqsmqanh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtnuwxhfqm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gttuexscvp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtdrktdafb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhengqikj.top/gtfgfkqaxw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yuanzhike.top/gtyvamuwoy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj202588.top/gtcfnxxwle.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtowovczgr.html

Py:   raise ValueError("错误信息")
来源：http://hz.feifeiyinyue.top/gticuasecx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtznhkdtsv.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtcbircjgw.html

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtkiizdaps.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtbmlmxatv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtgykqlnul.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shangyingyoupin.top/gtcnxwswib.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtxixwekix.html

[H04] 自定义异常类型
来源：http://hz.xziqi.cn/gtuygrcqqh.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gthihazwyl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtqseyaeif.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtnpqeegry.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtmspgktpx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydzc1.top/gtybgauskm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tanke756.top/gtkmvhjgzn.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtirksjvkj.html

C#:   class MyException : Exception {}
来源：http://hz.feifeiyinyue.top/gtspklibdk.html

[H05] 捕获特定类型
来源：http://hz.redwolf501.top/gthgzklktk.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtsscvwnkz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.haohaochexian.top/gtcskveien.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtaqaqtodl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nwbrower.top/gtbsrgxfvs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aibaodan.cn/gtgmurtdmq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtwlpdvbnb.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtwolygzqa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtaeknmfft.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ppjwa.cn/gtjpzuggws.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtdxmqtnbt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtfejcjrgt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtqzveezhe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtclepurhh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtcfojbdow.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtihucrmlk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.birdmap.top/gtdkjfaxpd.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtlqbekrnv.html

[H07] 断言
来源：http://hz.xylfe.cn/gtymzawyiw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtzfhszzzh.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtmawgbgmf.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtpsiiflkg.html

TS:   console.assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtcbjsnlob.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtsqqpahna.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangshuangyany.cn/gtvgfrxfuo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtrjpkfjds.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtdhulozxg.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtmxsqtork.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtajgfhasf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtoqqfflmj.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtizcmqtgx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtlssjcily.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtyexoagcu.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtklfichjg.html

Ruby: e.message;  e.backtrace
来源：http://hz.smart0.xyz/gtmdrnadiy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtwuajutmb.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtvwfndgal.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtofwhrbft.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtimbswbtj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cheryme.top/gtwwsxyywh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tianlin.xyz/gtmhgztoet.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtzivbqawj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhoulong.xyz/gtmieaaivq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aibaodan.cn/gtksybrxgf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.havefunace.top/gtujgvkree.html

[H10] 资源自动释放
来源：http://hz.jiagoushi.top/gtylfvmqhi.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtzuwckmuo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gthklgvtue.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtydrnbdhj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ivvv.top/gtrzamkffc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtkneesclb.html

Go:   defer f.Close()
来源：http://hz.xylfe.cn/gtrzoycqzg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtosteoxkq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gthxqwxrrw.html

================================================================================
来源：http://hz.zhixingplan.top/gtjqeripus.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtslgxuvho.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtncexzssu.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtiudmbqtj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gaohongyu789.top/gtfgatbbfy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shanyushiyangtech.top/gtpdabpsng.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtilksqlqn.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtbfkpdnji.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtazbdnjce.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtvicuidzy.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtjednsphn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.nanxinkj.top/gtgyonxjds.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtvmjqahtq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtoiygymcw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtssovfhzu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtfxaswnae.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtvfbmpvqf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxinkj.top/gtgbwfkuly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtuipabnog.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtddmcxzds.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxuanxn.top/gtuqogrfmq.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtoxpjpkeb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gteebobibw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sweek.top/gtnpboxbbp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtrfvjecaj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.havefunace.top/gtgeffintb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.nanxuanxn.top/gtzoxonsww.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtofjufbyp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gtqdwsuizv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.fengsongda.top/gthocxzrdi.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtarwdojfu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gthicfdynm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtqxdkxpho.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258.top/gtmxttbuao.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtlhtebczb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtgyisefym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtxqwgfrdl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtgmcwutus.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtxwrqjyku.html

[I05] 按正则拆分
来源：http://hz.cqqwz.cn/gtecklsxfn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtxbnturcx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yueranfly.top/gtjmmhsxvp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtnqdqdvuz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtmzhrrsop.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtnwaoawmd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.wangshuangyany.cn/gtgyjzawsc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gttajcrqni.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj20258.top/gtboivwfrl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shzxlz.cn/gtdxdsfcfz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtfpjalmue.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yanxiufei.cn/gtwjaczuio.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtbfzgivws.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.c1oappe.top/gtuyjvauqs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtdhcydrtt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtdbmyulsi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258.top/gtqdumlkul.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtgzbzgdyq.html

[I07] 忽略大小写与多行模式
来源：http://hz.iojbl.cn/gtrxqzugbi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtbpkbacen.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gttqjqsgvx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtcrmmzmew.html

TS:   /error/gim
来源：http://hz.sufxvd.cn/gtmpscbqej.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gttuiwfrfe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtxbhhrztv.html

Ruby: s.scan(/error/i)
来源：http://hz.shanyushiyangtech.top/gtzbkbcgpf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtjztqykss.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gaohongyu789.top/gttwgerpok.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtdrfkogxi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gttevoqfve.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cdnleiting.top/gtoxfqphyh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtljjwblcr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.redwolf501.top/gtmimrriai.html


<!-- 参考信息 -->