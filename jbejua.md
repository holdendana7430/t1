代发 wailian999

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3aljpepun.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bcfsohjt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wswruaqz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3akrldflc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xppiueli.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqsxlemf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vovswfda.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3twdelhla.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xanwrdla.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3aoxmknfr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ekldveql.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nlcmihmv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fgjnwleh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jiexdjvw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3kbnvlxof.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3obwzkykj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pgvjtfxg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tnvjbcsk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wukujcsl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gcbiuvwk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cymwxtyn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybhowhex.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vtlqryih.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckupihtm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nraasnzi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qyfxspov.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wyphwwpp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lncftzxe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3puacsmyy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxykbpvr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbsdaguu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yehpszmg.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzftuecz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3byyzefmp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nmfyfbhg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pxskrhcs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rqxmaizw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jsddjjry.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hzrfexge.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whhoghqa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfhoklzu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jreutekn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rkeopkro.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3mysrdate.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oftvvruv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tcuimdzg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vycnnyse.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bbatijul.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pmxinjyp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nyuizswx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3agzvixsw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3eqgsealv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xymncezf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cwlwibkm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3iewixdth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fstebgpq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qbntecis.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmmauzaw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3klrywhal.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3myrqtumc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rmagsoxc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ngwteyqx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jqcxudsj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nxghtmwf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jngjsyrh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfmkjqx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3falzjkky.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvijdfko.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3akmvrjgk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xkutiaux.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jvtlwleb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkghgurx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ayodmtye.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hkyghupj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fevfrkcy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wnqmbmic.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ieutbyco.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qnhagrgv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3fepuhupl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zhqpfyur.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3rcmcumzf.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hvidutib.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kmkjxqvq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaalzeir.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqxhrtxy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vebpbudn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xomcqyjb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ebaxpywx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nhnhmlol.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3txugvqdl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umfpawoc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zjoirmeq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hjvilyvx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwkxelid.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ualsilsx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtciaxmv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mtlooirc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3howjkhaq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3reilnwaj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwduuqqa.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ejntazfa.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zzbmlnsg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jmspswju.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nkhszkim.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cnefjzzu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iqixfufd.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mkqfyseh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3huquipho.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dsmsrbws.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rwlspzqt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3xhysyvhi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3pmfyjcqt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gjqczdex.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vksoweze.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hrrsmyda.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iuwvrkax.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3djtodbur.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nwewaafz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3stvrgerc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxisryi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3glytlqbt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbqzvgkj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3vxyqtsba.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cfcqdqle.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ixccjoso.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3emhxsmmz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3znzkhvhb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lyaeymyk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3twujqgsk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kebcyqmv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqcxjrlq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ylearsyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ieevyyoz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xolivcze.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3epvgxfaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hcvbtzas.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kboedvql.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ueqsqxuw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3pgnbwevx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oprxkbmd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsppysum.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jascqwot.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zxpjucev.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yqfkaexk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3aldufetv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mzrnboav.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wevnlohj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qnwthxgh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3kawpdwkj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhauzjxt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3renejohb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcvuhdpj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxanedho.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3fxmxjmkz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3idxxslda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mzztjcxr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3tehyymqs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3tqyzutuu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dagibcto.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tnekuiip.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vpjqlkgk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zhglmglf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3slswccin.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3oudluuob.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3urgkxwvt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3xvrwpzic.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3dglnncww.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nekymqia.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkucnvuf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpminjhr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqlewqos.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fgkivhqu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnipcvwm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3qdkxozhv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3khgeewmk.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3txuglmxu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ceigukvt.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3daltpixg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pveqhlxa.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkmhthij.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3rzswemyc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3opweiuqu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfdbjtpl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bkzdmvan.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qishvvsv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3eduspsip.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3muwjmssm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lnectrvc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gctcnqvj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mznonihv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gophmail.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3vphnrdjd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qesfzqyw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3gexljule.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qfruoshn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jhhuasja.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eagtirik.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jkyjsdqn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3wlahfgft.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3mywqdwgu.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bdrnfavw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3ldonoqsy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3mnrzsrtl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3krkbvmdk.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3syvzgqqz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3huvjpnnv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ikcmajps.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3jpuajzkn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3yctbtaxs.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3rcdvcqjq.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3thcadtsv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3hyevclit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3bifhinnp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3puaghvln.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3coetwcln.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfzplzkk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3utcvmina.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nffaherw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3sqjmnxvr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3wcnymslq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3rsqvpqmw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3pvbolnrl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3wkipvqva.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3oevwxdcg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3crdrdkvy.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mlrknvtw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tiqmamjm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3umthlpry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3automwuz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3awslltbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3beyfqtpt.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3igxertmp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3smkptptc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hrfgnsms.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urekmkvg.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbbaqol.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3abdqnqfb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3mwtpqlqq.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3bfvseowr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3vshwcodh.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zlkpswfn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uuultjib.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3edmlgryu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3rulbykvz.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3rcywzpsu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3fldkhxpj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3yvbefvub.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vfkcktex.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3erubcbpx.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3mmumgysj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmicxtm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3mziwozku.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wqhbbggq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3xsdfcayn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3tfecbfsf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3qrntmcyp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mthhkgak.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3izbahkma.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3cbrdajut.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3ehgjqwzs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3tydsfkfy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dxyhrore.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3xfcdyhzm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qgalfaym.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3hwbnokwc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3agvpesel.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3phquwpxo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3wzvaawio.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3aobdtclm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3blqpykjy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3eptcslwn.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3pofhjdrt.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3dguoggyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsohipq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3lkmowwkr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3mmcdrqhe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3wchpibuo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3hlnfhbyj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3agwfysrc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3tkewhbdh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3mstolwsj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3aitxuufp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3vgqyntpq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3ghvijusu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3jweeqwew.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt3duzjxvpg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3qegawiwi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pqnzkfiv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3ajuxtkma.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3ttwsnooy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3qxgdkvgh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3smnkhdan.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3pkanxpcu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3lbqtmjnx.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ahnkkwmj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3mwcnhaoe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3xuskcuji.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3cdbhypja.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3emkgpwxc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3qskrqyoi.html


<!-- 参考信息 -->