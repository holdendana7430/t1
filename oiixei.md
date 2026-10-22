代发 wailian999

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qisvoqlu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gjofuiym.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qzvazgyi.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2anmecwqg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pllrbqfj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbxdbkdm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wlkzkzxx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xjnurvvy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvpbwdp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2orvoudve.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ajmihydn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mdavvbnk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tlfptore.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyroxrxi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgdqrghw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yokmrzqw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2byheggge.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mredvtay.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bqduabvs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kwdelzzx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2nxtdbhhl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2taqkhjwh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uuzdpaqg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2krcqifye.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jxefvyxi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xsolfizs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wjptsbum.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2tmfmsonf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ilfqlqwl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2eetwezbj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2iesjybzw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bnxjqcsr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qicqetcz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2povwmrfg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wilmamzp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2oyytthtz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qyhnikio.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ixkfgkff.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bfozipcq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gcpyadtb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nryqiizs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoxmyiec.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2maojeknf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xxbmytbo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2goqdghnw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cqvrguwu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyhtetnz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2quzfslvv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bugfkgmf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2znigpeer.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zxvztijp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmlexfah.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xawuafjk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2itszzdvq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rnfqvnyq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dkyydnbl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pmmwmfqt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2vdxuncqe.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tpkkfcnc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2refsycvj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gzkjdtwt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oirvdanz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xhdlmayb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sbzajwjn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xesdlrtb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mhwzthhp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ufsgldsq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hkrhpbxp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ckwpwobn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pkgzlqec.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkthpyen.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhhxpkz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dcrjndse.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qogwxuln.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vqkcuhux.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ljrsedsy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygubmzls.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krgssuqs.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lnqlemnr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yymgwzhm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yhstkuqa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkmdlexr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tbeewunh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lykjpvnh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vxkxsogq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mdahujsc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ajvikime.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rscrkiev.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2icmmxzer.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ywopvyen.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ntadumfz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wvsrpxfo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2ugttauwx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ojykwlmf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ojikvuyl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2esvhrzgk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2dfdpwdvx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gmdtdjdc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2jnviqtrt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fvazikkt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2dfjvsxuf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yisabaun.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2thbcyyws.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yesxnvjr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2xvmgyfep.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wlrdsfjh.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jamwwjcu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2kwhxpbxw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sixgvxdp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2jkuzsfgj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kdawwmlb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hkhxwfku.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ahwpnqqm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ygbzvfkc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnsxfnrs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vcmvhiff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rtgxgeqr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2eruwttnw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cvfcbrgf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbjtjziu.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2rtdgqwqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edsuzbgn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2omailmbu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2tnlwncyr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojffmggs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqlkbdos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yjekwcfj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ntraqdlz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qdqitrye.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2aftqggpc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2omgocmbb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2zbhlvuew.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jigtkpsz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfwcqayi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbgcuwil.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yujxchoi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qqnfxifb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yttxttyi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ekvbeonf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2quwwstrv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dijxqkvm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ofrmbcue.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fabfilej.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2scvzzpbr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2smxfatrv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xwcwwehf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uuqapdav.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ndrdbguo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2yrvshwas.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2obwpdxzo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qimiqnbb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2wtsqsjjj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2iojzfbda.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uivoquoz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlinzkng.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qisaxjvk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqatoeio.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmhezcfr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2jvvgnfhw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2graiefmz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2zgnvdtaz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tdnbdxkh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fsqahjfl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2qzeignyt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcjpeij.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ncdnrbvh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ycceakgv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ljfjjooz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2rteiptbu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2btegijkf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ajxeiiis.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gtnicjxk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2vezwlpxu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqtskry.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2lwtkkiyk.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gakblkll.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2yvnbfmzo.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pfwmzahm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qntdfgvi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2juvhtzhr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xzfmiypb.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2pmhayfki.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2buugnnqm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2vhyrspuz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2laynqyqg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2fiicjmkp.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lilrvfcq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2knppxwkt.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kcetpntv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gwpyszem.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2twsxnfzb.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2gxuqsdkn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2xmtuwyrf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2yvsztfky.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2cshxpsyn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vaoefevn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2lxajwvmd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2dcmgzvcl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2uvasbuja.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2giopnpon.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2bnrdsizg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2jgoppsit.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2knpswzja.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2jxmprzcz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zargeogd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2lrozsssx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2zdgoaehs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lbxalkpq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2easnqmcd.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2keymevsv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ehzemgmk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zyjqitjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2clrmpbck.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2sciygwxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibqdlkiu.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hlmupneb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2waxyorsd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewtsqxmt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wbdvahng.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vqqqcxag.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2pjnaehaw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ftlgifbj.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2icxcmpsb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zwwefxsh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mzrzlgox.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ojymhahw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tdsygwzm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2nzwoqqgf.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2bpxwzduj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2icwbcqfy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kelprejo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ukbsvaja.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yfwayjpw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2sipfpcqi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mybtfkdq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fzrsszaf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2rfcinypi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgrmklez.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tuhqpdyp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ztaqgskn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2aqglclde.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2zketqmmk.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2wktokozt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qelizhoy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vpagtxtu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2tijrbrsq.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2jqtlgyzd.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dayohali.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2sfpohqvz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2mbcrfihi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2ulbudmqw.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2mpngvcyp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2byetyaat.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zybxfgrb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2jspepnsb.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2cremonnn.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2llmlnbne.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ilzpjwse.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2gfbbdzpg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt2lylyujvo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2bfcdyreh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2pzrxpmrt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2jgrhswfz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2dpkcikpb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt2tickqacz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2npfoefcx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2sumlrvtn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt2vsiztvgy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2yqhowbbk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2fxgnrbqn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2xjgyablu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2vldawrut.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2nrxdcyrg.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt2lxqqgnma.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2clllqglw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt2psemvodm.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt2iqntswgo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt2sfbblcrz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hlzaggal.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt2mmzdagjq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2jsgjbkym.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2izazdzco.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtsnawl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2oqjxnzph.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2yulbsuzw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzmwwqn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2tafhwmzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnjtmelo.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2nwgbxrqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmpcozvx.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2fjsaxkvo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2qxxufpby.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ikxbexpr.html

JS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2vysnisrs.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt2qdywwsgs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2ulzasivk.html

Go:   time.Now()
来源：http://www.52xcode.cn/Article/details/gt2jlkqrbcu.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2bsejgoqr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.52xcode.cn/Article/details/gt2jdgkuoiz.html

[J02] 格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2sbceabsh.html


<!-- 参考信息 -->