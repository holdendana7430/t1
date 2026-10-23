代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trtyhrkf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gxmkwqtb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lwrylucu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqkijskr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cmkytxwd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nfukoqeg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zzqlwxii.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3buswwuzn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3frllidrq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ugsvnths.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ibwbbvec.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3hcwlzxry.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsiwftv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3usdvavkj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lyltfzwh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwmudafi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xjrepxef.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jikwupue.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tzrhcpzb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xjtwggqy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vykjorxc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukqtnsgv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hlpxgwwm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fyfdknyx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3btyhubgh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3affxuftg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lysdizyl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eauuhtog.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sqskruep.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3aodnvbvr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhzuwjda.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrwclitg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3facsvsbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cojsozjw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rytyllcf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jtfhwsdr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zccjdcoh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lyduwlhx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kgpundlr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3onaxbhae.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xghxsvyq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exaxpnzi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iomecvfb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cvzmtlir.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rdederym.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eewcppli.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3suyufbzz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bbkugkul.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hgtdcwlj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cfuiicev.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dkdhfxue.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wetcnkku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vajxstsx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fzlycfpf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3epyijbtu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qgzjqycj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gnbpsfwq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkqicdhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pkdcijzp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gnvmqrts.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xojisydh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bcbejorf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3klhlufeq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygoadagi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ghxelnzd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ghytmxwh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3astefefs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jwvaadlx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ztmtubqa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3mhyawzml.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sjnpslqt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pjfsgphq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zscrexbd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mjcavltu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3djolgsta.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dbbgvpdr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bizhoocz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztponios.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3naxwhpjs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vfsteeau.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rgenbzjo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jhqbrsrf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sqrnsrco.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jdmrsnug.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3isicvkmi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yvkhwwrr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qtclfgrn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tymohsxu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3llnjmjeb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3llwypksy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dhaswwbn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivxfhezz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dtpgbsfe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vekeffzs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhfathzx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3powvsojo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dklycjyy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3sftkczfl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3sdcbbngk.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3roybymba.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ikncygqa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3pzmytdma.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zljtcela.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wigppgno.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3aaxpeneu.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cgziamon.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sguzjvha.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ifegadyo.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bnrsaqow.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nxlvhmig.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbqqhqoj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3vnytkamx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mkvrcnid.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gcuqcouj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3brletxle.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3aoxxkhgb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3sotfukna.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iogcamfj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ymvgcjck.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3iamzlwaj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jeauahua.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pymozyog.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wyestiak.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ihcbnzjw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vncvqlvn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mgpswkcl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3emazqvoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ytmxyzbn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3timrnhhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwslrjrl.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rlsnvpdo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3acssmmqy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qlrtqine.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xiwozwmc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ntpphzur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dcvqpyvk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3pekneewt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wcxayaum.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3iouahwlg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3byffttou.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cvsermjx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uldcllop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ilujdydn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3taymeicv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkrsjhoo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3akoadvfe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrgdlxsm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jepwmlnv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ymxefejx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vbeaefhu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wxuvhkya.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nrxpifmq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qflraioi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zzlgfsdk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3izexrjbd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3dzircivc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sjqpbhde.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bxjknqik.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xqmsdzqr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hebnhosk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gdmxcmmh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3okhtimxl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3iefatgbe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3lrzjdfde.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kalveavv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3grydqyfj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jzmxzyog.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3adecpkof.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3wimxbmdn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bfjlrtqs.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxnwhhfh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3ztgyayiy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3otsvrprj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kcirwleh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3rghnfngy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3gnvbsxpe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fhdpkrwm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fctzjohb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ksfayvnk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hqyxrbde.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3xyqwmxwy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zfwyfdee.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3uubczgyv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tmbfgdlj.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tslhhord.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3zewbarih.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dritbmqy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gigkmyar.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3zrtbrfvv.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3aygakuig.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3dqhfbhmi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fnsxexnm.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wuqkwhlc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3mflyqhmh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3eiwoixnn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3awfbgynb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3csocpxmt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tqxqpdgm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zvndxzbx.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rqbcqpto.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3aypeutqi.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3hjjzmbrt.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3cwzvrauh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mrnngfts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qaismqqo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3jldsbyiv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xkmhfufi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3avbtkxyn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mdzdfyvo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3infaukeg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3bdyqvlvg.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3quzwnjfk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gyycgcop.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3bfdlzazv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcrold.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3dehepayo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zvlikhit.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3htfdyswr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3sxosityv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bwmzdamk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqdtbybq.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fqbxebeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phpejrnm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3lcffmidc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3tivxozel.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3idvmouva.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyitbsli.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ezgyzhpx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3sdkbfdkk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3aydmorry.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vssfxgod.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qonenrfl.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3fhgirrtu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3vclbqgmv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3polcjiej.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3yhdinluc.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3fewhoxex.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3scengufz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3hjmqcjnv.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qhyvnzlu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3oximidmd.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3yvvvhntl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlzldgee.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3nohhmfyh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3cmwffuqj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3pjpokemg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eumfduae.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3ydnnjuem.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3mkqqefqo.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3udkrqeey.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ketseizn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqygpite.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3ueftyxbb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3mmlmcluv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3afitumcl.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3tkrfrhtc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3mgikfwsd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3uxfjlqxq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3nrigppxx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3fykebott.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ryoamjtf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qkvcziev.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3poctdebu.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3waunotyf.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjvxgzk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3cgrerozn.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3utwxxchw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rpbnbvmw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3harqmfcn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3duqklhmz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3udnadaxb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3zztpfasr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3gtvhfibu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3diqhauvm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3monjimuc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3ikljbikm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3lvrtovyr.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3alpfbyfv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt3hbheopow.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3ncudqata.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3qrrboduc.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3puinqpyk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3kejuhbvn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3yrjfreoe.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3fzoqvagc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3sjnokkbh.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3qpynlvyx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3xmvvzrli.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3htaxjcln.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3fcdyanjz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3qvxucujp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3zvgnzmbs.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3elgocmcn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3mmydywfj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3vzogbtsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpovbfcy.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3nozmepsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unvtwsrp.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dihlsfru.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3qvjxtopu.html


<!-- 参考信息 -->