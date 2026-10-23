代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wobkedng.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vxkpdhsq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qtghwipv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dqtkubcc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ivciprdl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3olerphjk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zumzbmco.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3forfqtom.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kwzpmwpy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bgwfwlnt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3umbiompz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3niugnfzt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zwtfhipk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rxlaxtvk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pavnwjqq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzxfkyxe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3swhcoarj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ljkoremj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xnoyyzaf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tdoxguop.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fjxxuswz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3blrlzcal.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnrafwox.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezgmfwuu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgyeyigl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3alzwcktl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztlinuja.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aevxxcav.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aivkddcx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mmmcetnd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvsoyfia.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ythkwwcx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tincdpqt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fcazevtk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mjyitygs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3yifptjwh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zplpvmnu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ilmaujjq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zvsyeqgy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwkmcxjx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yruaxqhi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zcxrwmjc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tuoimpkl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3houzyxuy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vyzubfrt.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ounutitd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3shkdpeny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3utouekqs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gwrtaoyc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ilexfleb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ajmhrael.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qqakytxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kowwsoyn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cucignfv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nymbirda.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ecepvdgf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nnotocyp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbeoxagj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rtyukhue.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsstqwfk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkgnhsmp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vrxtzkhe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kkujhscd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3blvqvugo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3sgvtwjfv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3mwppnpcw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jytdudqh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3tdmmdpty.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3izmssczw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aquzjqjp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jmlmjepm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ditgdpqi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lmzzehxi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dshejrft.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xlbxhfih.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3whytjiei.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hujukmda.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xvkmnptp.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3maygewne.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3omewrbaw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mjkmpwty.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggangpxm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lrryiwad.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gqhssmwa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3skouiifg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swsdtacp.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqyjnwli.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbarabvt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pymrlozb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qxrralyu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mhcnbvxa.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aloiomhn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mbojhogu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3klgpcola.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fxmgjzci.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kuvvbcjg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xkhgldpy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3maoqnvlp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3tbmedysp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yzbtieji.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mxytqhav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3tmgsnsmh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cyyugvzu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3kjkuiupe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mdkgteyf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ouoiyonl.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dyxichum.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tuvyendt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zgfloavk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lxtgslbl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3fusgyuke.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ooexbwhz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kjvlpvha.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3qnaggjfn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lcuamlol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wgqdgjij.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dfvdfccr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rhoizswc.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yqladvaj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3uejrsaqt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jczyiyxj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3wkoavqet.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kgjfbkhe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3eamivjyn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3qmueweoe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3tadscvgz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3llxzkzxi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgbbheoh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gathogyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcqymigc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eotuleic.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zlomacgr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3igqmxzum.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yobxoaxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pufkzbys.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivrtevky.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ziidowqc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3yifhwkgt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3apdcktzt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3cshpzzyd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3nxdirnqc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ljnxbypm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rvkxuwgq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3doaivrhi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ckoozwmc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3maowvnpb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhozrovw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ahyedyfl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3eucwdmwt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rgvhqesg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qmrnvpfk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xgbwyqpx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rldbypds.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sbhpzwgo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3hmodwvvu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mrwvggpv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jucuijot.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3oogzbxcr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fmisdjio.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3iigvqssx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuhrkbcf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqggbobc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vysiencu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ujfiodml.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pemnpskw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3trrgrrfq.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wnzlhdqm.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vznzwolc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3uiwoqjqr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3aidaylww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zuydohwl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrfyevty.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvwovuq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3uxcmnyjs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3bujdbfbc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3qlmcjfqs.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kzovisnj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bhtybbev.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ahazekem.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fhjumomn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nhvkxvzw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gsmjamrn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3auppjwbm.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fxnecmfo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gxnqoezl.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rfoffwzj.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvslsmv.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ttdjacst.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bfsqadct.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3pxlgobwp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xdiptsca.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3jibwngik.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3sldfkuis.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3gopujwpz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bwdonjkf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3cveqzmah.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kcauxosl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cmjqynle.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ovgxsvww.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3tvwoitls.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3ehmymjsp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3zrghzifc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3raslebrb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3zsyghuia.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3egcexyoj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3dyqjjfgj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxinvay.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3iopkocnu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3prdhixqy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3nxikpnlv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3wqnwwsdm.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3satebcss.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3uhkoawxh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ufkqmoxu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3nvubuupu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3waezdwjs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3qftxetok.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3jibdshwd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vbbcvreg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kstrwmtc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwnmnkdq.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3qeinksdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3btfpsibx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ntwsfjfd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3irskjnsn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vqutdfxa.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqqxzske.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvyyldtv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3atfpgbmr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3guioadry.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kocfuadj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pepdwlmx.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ludpsxyv.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcswdgjt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3nftpolgg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3wvfxuxaa.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3zvglkjxp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tryufavj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3xgbzquki.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3unntunlg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xgbwqblj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3ywimuvjv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3sufxsjyv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3jemduxmv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3rrlqebwa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wkwbqrcb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwykhpd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3dfeqthvf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iguqdjgw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3jedxxnow.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3qrtrdiig.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3lsmfhxua.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmjugvmm.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gbqubuuq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nwrzfoeq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vpudzenr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mjebvfbu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3kwcvhwns.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zobxtxxz.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tglvtmiu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3pxvogaes.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3irlpxjgj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3iljaldrm.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3atahrhsl.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3kncoljtd.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjnjvxuc.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3onjgdlkr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3wqenmzid.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3aqkjxewp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3tvsasadl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3gukqgieq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3hqzzjmiu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3ttgccwhx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3rdirnzfl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt3fmyezcef.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3hhqdjswh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3sqttdint.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3rvvkbgzs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hqyzcxrb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3wzzwwayx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt3iareqwnf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3gwdpjqbb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt3ecmmqhan.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3htjgloas.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3dgtnmczg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3ncmzmofj.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt3estkoomd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3cutjtxrx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3fvjqpqml.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3mtszsahb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3yusgvorw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3klbhuxtf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt3ofumkxdx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3lwzeuics.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3pruzlwbb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3salixojo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3vwpypvkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ongmxrnf.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ofpbtqsf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3rimlyqmi.html


<!-- 参考信息 -->