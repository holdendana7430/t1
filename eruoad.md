代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aezoovpl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kkisgubj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qvgyjimu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ncirebzf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bxhgkntp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lgpgvspu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2bjrqeftr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fhxcrjje.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hgvkcaky.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ieggbeyh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2seufwcqv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2txfxcaup.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lrjemoct.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mqqtmyyg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2rgwvrhlp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zaeovylo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fzukeesu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2suieridj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yugawpqs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyvknwiu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dbuvjqkp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xbchtjno.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bipouebc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wbdaryff.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rrnmpquv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rklkhsaf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zzmoumnp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uxhjxeik.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbmtmqyj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2baxzxkow.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qktquqkh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fhyfuges.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dorhblwg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gbaaquco.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwwqgppw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fwykolos.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmzbbwxj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xweyeguf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hrdltkys.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilxbmxbg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tauwpcej.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2tyncebov.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2luiivkpa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pofddbxh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kkkayvok.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uokfsepo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lkjqrspj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iabpcyqf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2gmnhbvaw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gupomovb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2axlipooj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hfxnhzvf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ladxsjyg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivjkyomd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ogfgvykw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhfwvhun.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2zynnenes.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jtczeppc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kkhnhqop.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2adzhtqtl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rudhwzev.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2kgtosslb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nrtkjbyj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiotskcj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndeoynjf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wltqbzto.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rjwttnxs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qcwkqlbv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2hrfbdfnl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2vjybuzah.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hxfuhmfz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2apcnoppx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bywviayv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qkktsjrj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pciqjifs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ijqdlbph.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vzrwmpsj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rypicvtl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2umgpotmg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2idhjzsai.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkevoxgl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzvbggm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iwqbdbpj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cfxynrwk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mslmqvxh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ruyqmgus.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rzsvgnyg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2brmuowfp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xzhxbuqy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnwipyqh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hqgvebme.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hgiqbaeq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wxzrfndj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ldcxccxv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xvdhckkq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hxfhvnpb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rjdvkohl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tqrgkusc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oqxckeuw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wxsztrng.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vfdvajpk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rlnrsaqg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pbjkxtys.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eqipjvnq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2ihxdulfn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2exvfppzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nqzbdbap.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vhwkggmb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2zuerwjwq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ydqeqsbi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uicwyajl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2aggzyuiv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2mhitlvae.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fxwejscn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jrvkpowr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2malmsruj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2yasaxmxj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rbhibwbm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcehglq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjkyamm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ytmxrepr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ehuqjnkl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mwtesnmq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ulfwxezv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xjkdllnu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2igmatafw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tagcjymr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mxqlspup.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2cykokmie.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bjrsminh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dwcwsxnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzbftwaf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2wufdgvft.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfgjhfuy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2epeaalxd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pnfjfhnq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nwyjceda.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2focojewy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ylvoangb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jwhbmqwt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kxrddxlq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2sgnshosx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvgawqdo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2pipyopbv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wbsaqgho.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cgjlsyek.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eifoqlsg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ufynrslm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tecdiqel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xlwkhiaw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zobovpmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tychxqxt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cvusqdpu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rfcpofot.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jtjwnuqj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zfubrivq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wibgorhu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lqmzcaia.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uquivdlt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nvewkauj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2rgxdmzyh.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2xovfxhil.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2joqubxme.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlbgejgt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ytyhpzvn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcnbfcxr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdxdjccj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wjwhfqmi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2woygudly.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cwxdtyam.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wnqglpss.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2sspdwybq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2jwgshbgf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fjzgwrgh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2irlbouxc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2xzyiokxo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xuulmsdh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2suamedcu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dabthbhv.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2avqqmjri.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2afebkdhr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sflxyrea.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jdvuzeuq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2usomafku.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2piitkiwm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hfvjscyi.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2laqmvbie.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2iiffplmw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2weebbzfe.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wpnqrsje.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2chldazlf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2taapyxkt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2saceuria.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2opdxgxie.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2gmvyneux.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rwrjfzzg.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nsvbtgqi.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2arcaqnof.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2igfhngdr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2rbtssgvl.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2sejipncz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwoldew.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2iudxrqcx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nfvgguqp.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2stvwoyyg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2piagpifp.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2pgbgwubq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2pznmwxwu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2klexhomg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rnrixzui.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2grdlirgr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfgrugld.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ccnixkhv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2gyjrycuz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2uyriryda.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2xoodvvck.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2yevmsdzw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2mgzuehlf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vjibfumj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2qvzxelxo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2aeckbcbs.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2oawsjkgw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ygxkdfrz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rzcswfem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyuxedtm.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2rjbilwbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfbyefbs.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2aynlznga.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cojohpmp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybtrxwxq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pzhktpht.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hlrlwgmw.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2mjgkggkn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycdgrore.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzqiogr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2cksmgrwk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wqiepcdd.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqotcon.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tnaqqhtr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2atrapvst.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2dticrzyv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oufzxxfe.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgzjdvah.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2szdmzdbv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bxziejvt.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2wlnwkvww.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2bjnnvfsu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjblzeqr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2gyetsmzq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sfpejjof.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2kioynzjf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2odyyamqy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2khawjbhu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2vyijgqlu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2lghalggx.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dmafadsx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2hgngmfwd.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2znybfvzm.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fbzkjnsq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2aojktkwe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2jwvevmlz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2scrkuzwn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2hhxnjtvk.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nbnixafm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2phsghqzs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xsqoecau.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2bjqhbvbo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2eofmwncj.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2lqyganmk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2kapaeqei.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2zkxgyddu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2wtngxyxn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2nyirogwa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2nveunowx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2xinehvxi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2gbrpqsti.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2braaijjd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2bwaczgrn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt2hrqorlxd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2osndeqxf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kifkbtrq.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2ndkszhxd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2kbtrlpef.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2nvvrtkfz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2hvddsglh.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2wmprbmrd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.52xcode.cn/Article/details/gt2rlcngbuf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2iyttwvlv.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2nfjvvozu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2qmketdoe.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2uuysuape.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2zwyekoto.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2xehmuahl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ythcatak.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2veqyohen.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2goavodxk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2qompqckm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2fvbliuvd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfqrseb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cssljvcg.html


<!-- 参考信息 -->