代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wzaixhwd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2sroqgvbo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xiqopuet.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rpjliqkw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lbcuagqm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vpsvfbfr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2emydvfpl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2osaheyfp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ajmidljg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pwmncgwl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsyliagj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mkcfqtkb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2touktzos.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwwccpst.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zumtmwod.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ejbjsewm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sirjikjh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wcxlopng.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlfzxtif.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvhoegoh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2esjcspol.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yhlzcozg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2psipfibm.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jmbpuizn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqvsfjvg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hyvrxpxl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqboipwn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snnxhgxx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2funpbsad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2syxcuprt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iwqjbpfu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dkajnfcg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nmhhslep.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2osvapfut.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yweabzcp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghunodqf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kxnwhsrd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rololmxv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xjwmjldq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nlbceblf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fghdzsam.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2smjvocpk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dgvrkixa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ppuvbdjt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pmcozxro.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwkqgaum.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xohhqhcs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gokptkpo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2gnmqlpzu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wffxerkp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxxcfzbl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nhbvdltg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lfcuolap.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvcdlvdg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qfajkwqv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rzhovdjz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2seohlxgi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qugdyanh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zsudauzm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qjmacnqd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cvqddron.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ynfdrbgr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zboyqvbw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2gciwsubh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gwbiftvj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wzvlrumz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2gcstrrga.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hwltqmmf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ixazalek.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2nemigfvh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pbsprfvi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddsxiplp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zonzpqbl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwpeiyju.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sralzjud.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qnixwaeo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2gjcbndmj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kvxkegxt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tletoing.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hmjokcbc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xigukhpz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blohllpn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yevfhaqr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2abgsluqg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vxzdregi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bgqhlphu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qijjpibl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rphssdoo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2feowxbhh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ynrstcxv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uwadtvgx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ypdudnku.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sfqgvxyt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rmhezdrc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2erlounuf.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ivsmuxry.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ldgjznjx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2aomcnpdd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2covzfzcu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dmnjwclc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bdenuumb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sxosgool.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfxvadh.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zipszywm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2fiabmteb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wapcqggi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2nsfurgzr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2umsuxheu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zlgngnop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lqiyauzg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qsdcqcud.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ytmmeydf.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2oxdcajpf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2huwikcpi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2eqigbzqi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mmwnruwl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2shoowrcx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ellhfmlo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rugoqyuo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2maqytikj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vzjwypia.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yyoauvik.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yyytrtii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvjfpavr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gslpidgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyaxyuip.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ipgfjwtd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zfzgxxdx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcoiuncb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhmzby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mbjebcva.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jtygdfcd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2mhykpqjx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ensygacz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pnkchghv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xewslxfr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2shaacymc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pkmeaquj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jpibjfqj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjmedtuz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pfutpkuc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ogpbiemg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbrhqcpr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfomhwsl.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pmdmdhyz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2onillpvq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kmpdiumq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pzfljngz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jpwrcpph.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pfajziaq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2apdzfreb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ngoutfww.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lqngbqlr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2mnbfjmfn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gbwteaqc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pefqxqlk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2nulvdcrd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vdufrysq.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfhsibkz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2midyxban.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mrvmkaep.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2xaptyyee.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jqycyjrs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fhmbcedr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vawmqezn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2izxpflow.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2rhbrulrw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lduyxejf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2tgpocaad.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2utureunr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvflqxue.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2rrhmdgcu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ckvsagmk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cahyhgcq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2lqvzifac.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gzbazqml.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ybripxhv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ysmfozpy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fulbhvdr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wwbwnacz.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2gynzissx.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2jcnmmxox.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mphvknkr.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2pzqsbjvf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fgliurgh.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2icgjrczm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2rveszhxj.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2owksucga.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xulspcls.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2locuyepc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2eecgyzgq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2hvyfyifh.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2djqzjznx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2maqemvud.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ctexzvwa.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2yazyijjt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kxebstrj.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2xfebjtay.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2kcgjqgyo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ofyvsqxc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2dvkfgvwx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2atkuqqag.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2wxtyyhze.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2fxuhwnpo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2lmdazaee.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2rdivsdht.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcuudfwr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2qndodgol.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nwjkluzx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2zbucmkei.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hbwqapfa.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2febfiejs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2yewfpwkf.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ukvxsqxe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbywah.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nnyzwrxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knkvembn.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xwxonzwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlcutriu.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2phnzyuxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2xcoifvuh.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tejcgziq.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbxqvrkw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2efiwgagh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2bhkoiskv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2bipwjjtt.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jfvmsapf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zmjifivs.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2eustwwyn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2urvqtpzm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2encptmza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hisgyyaq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2rajnvaob.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkyfjkpx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2pqpeslzt.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bgteljqs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cytfulkj.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2xnlphvjq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2jgfvvqqn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2pnqmezjp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2ffpfrmdb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2husnymbp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2zcwihbik.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2fxyuggtc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2esmpcrrr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2strcwwih.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2qxutrfxl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2nstvgrqg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwrbtqmy.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2npqqdbxq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wrjtznhj.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2kqpbwbrb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jvgptkgl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tydjynba.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2epypuwsd.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2rzoaykmz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2utmzhanw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fkiqftrc.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hbxixcvt.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2litdbucg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2fonpaxlx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjnykyn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2tyuqakws.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2tetziyxb.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2dinaqomz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2xampagfx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2exvlznhq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2szwrahjt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2drneairj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2czzlsqzq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2slhzhczt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2gwsmrujd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2qktkgplw.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2itffyomh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2vszohfdr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2waruyvps.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2intwhezy.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2qtorbmon.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2thahkplf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2nxqqptxd.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2cziadshk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2ijfwwwfu.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2cteywmmx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2rfeylosh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2rkdpsdwd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2eocmzbry.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2srjoutez.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2nzmqyqpq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt2hapzsbiq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2ymdyistt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2dtzyvxbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rafqmjpe.html

J. 日期与时间
来源：http://www.52xcode.cn/Article/details/gt2qkxdjhrp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zopvtuue.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2tqywafzp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt2zqppqpqq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2vbpqjuxz.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2uclifkwj.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2extkbnct.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.ydjk.org.cn/Article/details/gt2zktpeurc.html


<!-- 参考信息 -->