代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpcclxou.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkvppaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nhcnhemh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ujvbirxc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2matfenvd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fuqkimhq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ahqusjkw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jmpccyav.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fjvoojpu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ekgfuwcf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pxfbnrmu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nzdysxxm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zmcbtwte.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lfycvlvu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2skvcvhlb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vlwgdihl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uihbbtau.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agabwzlr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hdwcwvhm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xjnchexu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dpqprtnb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2muptbbkp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2anpagvwx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qbbapwrt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2htoywloj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdpgdvnz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2msgfvpuc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xxaqrysu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrggnevh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kbcmtdow.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jtrwofma.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2evzevxap.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2rqhahmxf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ptgeyhoi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vaxilnpe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2djpwreep.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdoqvbr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mvmhdqmx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gjyapuht.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2oeklmjcz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vnxygdqs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qzpbnghx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nbtwumcn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmoalcfh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lbronmlt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldyxmhnf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dqsxdril.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jnnvwjfo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qcoomojm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sclkdxvp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lpgppezf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ghaujpry.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2crpuxbjy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwccakpn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jkoirnax.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bjjslpni.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2eqmqztme.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jpxpozaw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzrlqzox.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ifxwilbn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yyhfqkrl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2grjdpxbt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2avonetsw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qdmdncxm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2queuchex.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlwidlw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2edveohhe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2seeicasa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2abwjylva.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ldltcwsu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hruswiue.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mvbznayj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dcjrlyti.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2byaejqjk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nersteyi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ojheaizw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vryplqmj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2wakeivhp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dqlshnel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmkutfce.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgrzuss.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwinhpii.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oofyyjov.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jnyllsoy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jzutavud.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2anpcdngk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jcplnuoz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dtdpyuhj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vntrikbt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ashoclkf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2suutujps.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rbhkzkgl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dvhugxun.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cesdbhkv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pheyhsmo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxbeljvk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gxjxymzf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qlbwovel.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2amxnyqxm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yrzbxbzz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ubuqitzs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2artypfll.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vyhhwrcf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xkhojzvu.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vvahatvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qxazdblt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xcmiiyqx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vqrmfijt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2iywvzzzq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mujyfyut.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzrbnmc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jtryquoa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nafqjtft.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2hjjdwkyz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fltllrsb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2rsrgjaoe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2uzeqrfax.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nlnkfdss.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dbtrbnqd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nlzrrjwf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mpwqdoza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yapixvgr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ulovuqxn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bigdysjh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jnbrvcyp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kourggro.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2stmdnuce.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2fgxmagsp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2pzixnnjg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ayebyght.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2apbfvynv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvygjieb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hcyuajjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laltlall.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dyrqujco.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2wkdfnnwa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jkatpjck.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qtfgnfzl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kxeawrel.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2btelmtkt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2krnnnpws.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2unxsrebh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aiacspab.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xgyaptak.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2khymgxro.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fztygubo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aemznmjj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbdarwot.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtohcpvj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jgvxbazy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2hdhxkyms.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dftpcqns.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2kaaxuseh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qsybnceg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qmfumejj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xmvhfglh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uxurslwc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pdrgpmdg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jogcmipt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2grltdgrf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xuaihjzh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nlnrhjtg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rsppubfo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oqagshor.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2juxkdzxj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wqadlmcw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2jnaeinir.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cqzkaarc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fotaylhl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvikrori.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xailjpuz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2urzsgwur.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2hleejloy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sszyswbb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awrlssie.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykdftktm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uiejussi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ycgstwzp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbubdgeh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2cpubgnvq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wcnbdkti.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ohakpwbk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2emkzjbfz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ravpbinc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2amoboybp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2lswnhwlt.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvkqorl.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tzylbltk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fwrugpjf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2vnhgsejc.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iszlsitd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qwcgbkvx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrenjvgf.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2ycaacccs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2rqhkwwij.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2fwyikgus.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2nzeceezx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2hrcomyhm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2hwhksqkf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2soihache.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2punowdei.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmykjeu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ieenextq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ycffugrn.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2vzxwjazk.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2kuqqdbuf.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ulddvaev.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2zmqfeuxr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2kpenknkr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2kbguiuxv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2ndyjrxzy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ytogtktc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2xlkxxhfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkxhwmh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2orvvebtz.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2etwzpatz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2ejpbzkhs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2ayqetjds.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qhvuzziv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wrbsttyz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2rrllabya.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rrnyuixx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2oznvljtd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qefjxwuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrseetbk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2sotqyrqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igmzdpte.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2cmxlqdyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhzpgdlf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ttjfwtox.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldpjwabl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cqcbxsfq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kdcjjhsh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqpqxub.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nemyyzzd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2xduvhfme.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gophuqey.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2opbietbr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2xmpfjhym.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2zsfvfwlv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2wwazuqlp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2jasvmoyr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctfmvgcg.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2owyfzhpv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iihpempr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2herlrrht.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcwjtbta.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zuqwvsel.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sntpkpkf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sspqboqs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2zhgyslny.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rnoreofs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mapwhune.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2nquairjv.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2sepwynmm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gqhewtmv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cebrbvzk.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2nbzjbasj.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2locpnpaq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ypnpnwgn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mrmygwsd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2weeegikg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vukqlqqo.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2wbzmnpaw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lpjjarsx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2knxwrcat.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hppedker.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2ieoqolqg.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2mpkmvnkc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dhougofx.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2qjcsrmls.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2trdtzvua.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2gsxmtyjq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2fwdyrprj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2yaiejjnm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zwphssmo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2vlxsbgxg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2munrohpj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2pmjjhfxv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2ngiglzpo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2eopoomwz.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2tnrhsdul.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2qyhpwbxn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2gaifcdtc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2qwzlfzqx.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2zuvxpxep.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2kipqyiwb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdurmcr.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2gcgjsqby.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2xzittfru.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2vpwdlevk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2uobbldjh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2epuxytev.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2eaazfewk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2hmmjxqvk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2meuvghfg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2zbjqpjfw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt2evvkjrjv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2mtnqpbqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsouxtfr.html


<!-- 参考信息 -->