代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yongpay.top/gtzrcxuiqu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.c1oappe.top/gtgaxtzmhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shangyingyoupin.top/gtpjipjzfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtjrzlhfmw.html

================================================================================
来源：http://hz.haohaochexian.top/gtsmnazsmq.html

G. 面向对象
来源：http://hz.ydjk.org.cn/gtshrapakf.html

================================================================================
来源：http://hz.ivvv.top/gtngfevpnn.html

[G01] 定义类
来源：http://hz.ivvv.top/gtfstjejmu.html

Py:   class User: pass
来源：http://hz.yvedp.cn/gtyaqltitj.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtwjcxnpvu.html

JS:   class User {}
来源：http://hz.fzhhl.top/gttargerlz.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtepvxrsmt.html

Java: class User {}
来源：http://hz.feifeiyinyue.top/gtqqudyqqo.html

Go:   type User struct { Name string }
来源：http://hz.chenjidiqi.icu/gtwatnnvzb.html

Ruby: class User; end
来源：http://hz.gotoacloud.top/gtuzobeonq.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtztjlqlgv.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gteeaibiyb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shzxlz.cn/gtdcayxndx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xuetiantiany.cn/gtaowwbvzv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sweek.top/gtmvsqyaju.html

TS:   constructor(public name: string) {}
来源：http://hz.jyoumei.cn/gtqysrsnvc.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtlupxnqgz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.haohaochexian.top/gtodbxbexc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.chenzaomai.com/gtxnnfclqb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgfzy.top/gtgbjblwuq.html

[G03] 实例属性
来源：http://hz.iojbl.cn/gtcmsonkrk.html

Py:   self.name = "x"
来源：http://hz.xziqi.cn/gthbsqgbxw.html

PHP:  public string $name = "x";
来源：http://hz.meibo888.top/gtdbqusrna.html

JS:   this.name = "x";
来源：http://hz.daria6918.cn/gtdqkpjeia.html

TS:   name: string = "x";
来源：http://hz.kuanghao11.cn/gtvglbqumc.html

Java: private String name;
来源：http://hz.zhoulong.xyz/gtzppykimn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gthcevrgfv.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gthumgszxr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yueranfly.top/gtiggtxvfw.html

[G04] 定义方法
来源：http://hz.mhx1999.top/gtadtosfkt.html

Py:   def greet(self): return self.name
来源：http://hz.jinghuilouyu.cn/gtpozctcei.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtdclnvvee.html

JS:   greet() { return this.name; }
来源：http://hz.daria6918.cn/gtbvvypiol.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtmwzgsczx.html

Java: String greet() { return name; }
来源：http://hz.chenzaomai.com/gtxhfekvge.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yangfankeji.com/gtzaeefbcp.html

Ruby: def greet; @name; end
来源：http://hz.jinqigufen.top/gtinqdwmoa.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtpobilsgb.html

[G05] 继承
来源：http://hz.hfpthk.cn/gttqecujat.html

Py:   class Admin(User): pass
来源：http://hz.cqqwz.cn/gtjtanffmo.html

PHP:  class Admin extends User {}
来源：http://hz.kuanghao11.cn/gtmxtyfdoz.html

JS:   class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtsyrembtb.html

TS:   class Admin extends User {}
来源：http://hz.jinghuilouyu.cn/gttekkefoz.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtxwtlhszw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ywan-chungtsiang.top/gtspsoplhv.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtubnvebkf.html

C#:   class Admin : User {}
来源：http://hz.snrcjt.cn/gthnejpxxk.html

[G06] 重写方法
来源：http://hz.snrcjt.cn/gtrhhyumcm.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtsidljidy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhoulong.xyz/gtvegpdcfm.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtwofzubzx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtzfdbtkxt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.snrcjt.cn/gtnjwnegde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhijiandao.cn/gtpalvurni.html

Ruby: def greet; "admin"; end
来源：http://hz.52xcode.cn/gtkcaaxbne.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtvoimzzvy.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtaodtfthn.html

Py:   super().greet()
来源：http://hz.iojbl.cn/gtlynkozzg.html

PHP:  parent::greet();
来源：http://hz.kuanghao11.cn/gtcovyxzbc.html

JS:   super.greet();
来源：http://hz.yongpay.top/gtcuiwtwwz.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gttktirxeh.html

Java: super.greet();
来源：http://hz.gaohongyu789.top/gtvqitrndz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.daria6918.cn/gtodyuuzur.html

Ruby: super
来源：http://hz.sufxvd.cn/gtwgbotzoj.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtaifjlzyy.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gtdmwqfcfa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nwbrower.top/gtbntsxgpb.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtedkzpdoa.html

JS:   static f() {}
来源：http://hz.nanxuanxn.top/gtzwfwinlp.html

TS:   static f(): void {}
来源：http://hz.jqgufenzy.top/gtvswbryef.html

Java: static void f() {}
来源：http://hz.ppjwa.cn/gtsabeemwa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.hnqzz.top/gttlyxiuag.html

Ruby: def self.f; end
来源：http://hz.xuanzx.com/gtliemiedw.html

C#:   public static void F() {}
来源：http://hz.jinqigfzy.top/gtimxrpdfq.html

[G09] 接口 / 抽象类
来源：http://hz.nanxuanxn.top/gtdxdiigjq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.aibaodan.cn/gtitqepezt.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinghuilouyu.cn/gtqagdhoxb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.vqdsnc.cn/gtvedakjxz.html

TS:   interface Shape { area(): number; }
来源：http://hz.shzxlz.cn/gtdxpsnzup.html

Java: interface Shape { double area(); }
来源：http://hz.zdqjudy.top/gtnkbzkisb.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtjtcbcxld.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gtydkozvud.html

C#:   interface IShape { double Area(); }
来源：http://hz.cucudq.cn/gtokjipzjn.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtnvsfkveo.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hysaishi.cn/gtebhagpyl.html

PHP:  public / protected / private
来源：http://hz.pengpengdd.cyou/gtzsrhiqjp.html

JS:   #private 字段；其余公开
来源：http://hz.havefunace.top/gtbpldbyky.html

TS:   public / protected / private
来源：http://hz.iojbl.cn/gtsgrwjzqv.html

Java: public / protected / private / 默认包级
来源：http://hz.jinghuilouyu.cn/gtypssruly.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtxwrvjewl.html

Ruby: public / protected / private
来源：http://hz.hnqzz.top/gtxkppbmcy.html

C#:   public / protected / private / internal
来源：http://hz.hnxiangtu.top/gtcymojmbg.html

[G11] getter / setter
来源：http://hz.iojbl.cn/gtvibdhzee.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtookwlszu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtwftotxay.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtuupajier.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtbsmgrzpx.html

Java: public String getName() { return name; }
来源：http://hz.cucudq.cn/gtjkhwqtbq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenzaomai.com/gtaqidnenx.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtmymlnvee.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gtrilqormj.html

[G12] 对象转字符串
来源：http://hz.zdqjudy.top/gtgrblnixz.html

Py:   def __str__(self): return self.name
来源：http://hz.andypj.xyz/gtblrymwhg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.wangshuangyany.cn/gtjfacxvdf.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtmyomjqfn.html

TS:   toString(): string { return this.name; }
来源：http://hz.aibaodan.cn/gttgcegbrl.html

Java: @Override public String toString() { return name; }
来源：http://hz.ydjk.org.cn/gtlgkpvykf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gteonvxnzk.html

Ruby: def to_s; @name; end
来源：http://hz.jinqigufen.top/gtmzrunnfg.html

C#:   public override string ToString() => Name;
来源：http://hz.ehwqpu.com/gtttuqlvpl.html

[G13] 判断对象类型
来源：http://hz.kuanghao11.cn/gtlrpmibwl.html

Py:   isinstance(u, User)
来源：http://hz.hywenlv.cn/gtqasppppb.html

PHP:  $u instanceof User
来源：http://hz.gogol.net.cn/gtpmlehizy.html

JS:   u instanceof User
来源：http://hz.aizwys.cn/gtnwikggxe.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtvsknphlt.html

Java: u instanceof User
来源：http://hz.jiagoushi.top/gtpjmodjlv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yanxiufei.cn/gtxflcmfho.html

Ruby: u.is_a?(User)
来源：http://hz.sxryk.cn/gthpwrwczc.html

C#:   u is User
来源：http://hz.fzhhl.top/gthpgwfefy.html

[G14] 数据类 / record
来源：http://hz.svipenyu.cn/gtkcdgxtqe.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtplwkypdz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.haohaochexian.top/gttccczuiy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ehwqpu.com/gtmbjknhxy.html

TS:   type User = { name: string; age: number };
来源：http://hz.sufxvd.cn/gtufledyry.html

Java: record User(String name, int age) {}
来源：http://hz.hongshengwenyu.top/gtubtosvmk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinyuanbaomall.cn/gtwzjjswgz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.mhx1999.top/gtcdkaddly.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtttmjnwst.html

[G15] 枚举
来源：http://hz.zhoulong.xyz/gtslfgntxg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fzhhl.top/gtpqxsrtzq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aibaodan.cn/gtdpoxfjws.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gthqajibmr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtajkijrhz.html

Java: enum Color { RED, GREEN }
来源：http://hz.fzhhl.top/gtncoewqmj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhixingplan.top/gtcnqqswxf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtawrevugl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.sweek.top/gtauwqzfsx.html

[G16] 对象转数组 / 字典
来源：http://hz.zhaomingkeji.xyz/gtynwjaaow.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xinyue.icu/gterunawqp.html

PHP:  get_object_vars($obj);
来源：http://hz.c1oappe.top/gtskydqbak.html

JS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gttblszhrg.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtyiqpwxsv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.andypj.xyz/gtmvnnyjaq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ppjwa.cn/gtpgjtgvge.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gtnkwsrows.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hysaishi.cn/gtcfrghdto.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmxqtvkut.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gtdbkhqjiv.html

================================================================================
来源：http://hz.yongpay.top/gtgohkuaxd.html

[H01] try / catch 基础
来源：http://hz.daxiang520.top/gtequitaux.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtlqacyxyv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.aibaodan.cn/gthdzysmxy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dashuyun.cn/gtpkkbtycj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gteykcjhyk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hfpthk.cn/gtxxgntcia.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtdyaqttgo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenlongwang.top/gtjvtundfw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtznruqtfv.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gtdxqltezr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtnuhstjyk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtetxlfgig.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtzdfrxjps.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtlgazyqzx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtpbzrivhu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ehwqpu.com/gtvhsstmyz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinqigufen.top/gtjjikxlfx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.daria6918.cn/gtjiwzziic.html

[H03] 主动抛出异常
来源：http://hz.cdnleiting.top/gtgkahkans.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gthivzlatp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtourrebve.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gtvfncobma.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gttmkharzo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtotcjmmuh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.svipenyu.cn/gtiaeibsah.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtynssstsu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtwuqhsaiv.html

[H04] 自定义异常类型
来源：http://hz.hongshengwenyu.top/gtqgvtzflw.html

Py:   class MyError(Exception): pass
来源：http://hz.ywan-chungtsiang.top/gtkfillgfx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gtihdotxhe.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtwzqvayuh.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtkhcpswxp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtswelfwfy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtsfhzzpmp.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangkeji.top/gtpvizdypj.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtvsdoztcg.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtlzidcgjv.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gthduuelfb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigfzy.top/gtxuqtscfr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtjdcuyrce.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtecnewdoe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gthjyniaiy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtsoizppzd.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtrgzvqejn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtzctfypwz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gtpkcebper.html

Py:   value = d.get("k") or default
来源：http://hz.bjfxy.top/gtcwqwrkjl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtyjfpzobh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtxvkerhgv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gzhubu.top/gtfnmbpdkd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pycfn.com/gtmgkhendp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhiwuduotai.top/gtuhylbqzg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dashuyun.cn/gtruknmaih.html

C#:   obj?.A?.B ?? default
来源：http://hz.jqgfzy.top/gtslgftcma.html

[H07] 断言
来源：http://hz.jianghu66.top/gtzvmvzsfb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtduolyury.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtysdwtnah.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtrhlcfdvn.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtzwvyahxy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258.top/gtlqecdosn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtpuhhlran.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cheryme.top/gtyyvevmno.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gtkqluypab.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtggrmluxd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtstmydckv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pengpengdd.cyou/gtjyxxusxy.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtyoehfbzn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xinyue.icu/gtbxxndvqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sxryk.cn/gtirnnbvep.html

Go:   err.Error()
来源：http://hz.zhengqikj.top/gtvocmapad.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtniaiutbr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ywan-chungtsiang.top/gtezrgvuxw.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtvmrmyndg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtbhzifath.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtxezfrcho.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtjmqxyqzn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtjhdvqjek.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hywenlv.cn/gtakjlysfw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtnmetwyrw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.52xcode.cn/gtpndyspje.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.kuanghao11.cn/gtehdojmsu.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtgbdzbnay.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fzhhl.top/gtdrbfyjyg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hnxiangtu.top/gtnoxrxtbj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tianlin.xyz/gtzwiktsst.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtxtcfdcxq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtutibqest.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtyxgikqps.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.smart0.xyz/gtqtoyxgta.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinghuilouyu.cn/gtrncgisum.html

================================================================================
来源：http://hz.gaohongyu789.top/gtinlljcfe.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtmhixotgq.html

================================================================================
来源：http://hz.xylfe.cn/gtaumtpivk.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtogokewob.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtzqshxkwb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.havefunace.top/gtfghgmgfc.html

JS:   /\d+/.test(s)
来源：http://hz.jinghuilouyu.cn/gttxtjpcff.html

TS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtwolwckfq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sxryk.cn/gtupsddubz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ehwqpu.com/gtmjtluhjw.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtbypawzjc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.svipenyu.cn/gtrieevvow.html

[I02] 提取所有匹配
来源：http://hz.jqgfzy.top/gtnwrwqbru.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ppjwa.cn/gtjfehvldm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258.top/gtgetsxuza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtowujxodl.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gtjksztqvm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.fengsongda.top/gtxodqudap.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtrbuhsukp.html

Ruby: s.scan(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gtiqljqvoo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtulqykabz.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtkjinebig.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtxihlbzhn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtevajlysv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtpxetcttd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gtnseillrr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jiagoushi.top/gtcgfqddxf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yonumen.top/gtuwjnibou.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.0kj1m.cn/gtjszlvmlg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtetvwjevq.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtgmimitkl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtaziklelu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtzkwdklaa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtbzkerkhe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtusesyupr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtoupdsyvi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gthgjlupny.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtntasiakm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cashguo.top/gtwxkrpcyh.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtrxjkuuni.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.meibo888.top/gtnwdkoiag.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gthzcbippn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hongshengwenyu.top/gtlpburmpx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtuetkmsxk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.feifeiyinyue.top/gtouwjyxzx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gtzkkiqfde.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtuzjkrmdu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.wangdashe.top/gtbdfyntav.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.smart0.xyz/gttwddkrtj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtghutihmg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.birdmap.top/gtemxcbsbr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.iojbl.cn/gtbvgvddru.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtczxoidqy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtdfakisxw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtazdgdtig.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zdqjudy.top/gtvdstuxmt.html


<!-- 参考信息 -->