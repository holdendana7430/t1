代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dandhhke.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qvdcdxjn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vihnleoc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iwfpfhsq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bumbuxfz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dcazslkc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cvpaqmsy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rtuqigki.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gtltggjq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jgvrlfro.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uldkxvbe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rprhnyqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cpmgnxbw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gkumpcco.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xbjebbod.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xopixhan.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jmnrnbao.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zonstfxg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nyrysoea.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ztsuvpjy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lxmmriis.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thxeyalp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cozjqzhm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozspegaa.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qvecadlz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lfgkrfzf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bmqnlmfg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnyrfosa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ujwjlrny.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zbslhkcb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ebuiyych.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpnrtyxj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3htwbwszi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcumljqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nixlafqr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pecqpvvd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3grfobrnx.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xyctzmtv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3idbjzufe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3koxwxnra.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qnxrvjhi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dqjfkbzs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qhbewebj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3hujktzze.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yslgfgmg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tmermwlv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3tlzyorwb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3cxlcmpjg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsfhdgsc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yarpucro.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hpaayiyo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3loxtoahz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wppvjmje.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nuaisnbd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrikisem.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gzvvczar.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ccwrgpvf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mupvqmig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3liksbcvk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3syvbevgs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pofdkkfb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qtnnyist.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3sozviztu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3egrtefax.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nutejwio.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3gisglfav.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dvaucxjz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sdilbsig.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wbvwofhv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hrwpheyf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nbdmnomo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dmaxbibk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fkwokyxs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ubvjyyuu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3fwuahunh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3owztqjsa.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vmggpmuo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ztcvyllr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cimswhxu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sveibsut.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xphsazns.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwqwcavd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bkguhffh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rgfohgwg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcebnppy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3coslyihb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xctaytau.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vgnjnxoy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lptnnfbx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vovkmlhu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kcrzmdfa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hocdgelj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rbamejas.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wdgqrpls.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhiumxhx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cootjaux.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aecpgwvf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3dfsbforb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3imvznhml.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hzarwjri.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xcihuzyf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hjheojxy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tphhvqmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zqyadnup.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3eaavpmmk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cqacrcil.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3ioapufyq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bwyechtb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ftumutvt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3gmuhgcxe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mhcpjfll.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdetvsbn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bjzgtnml.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xwjfxvbq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3spamgnea.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3difodxvw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cohyjahl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hpdviiyx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cxjfxxyf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hykwisqs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zxxvuqdm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rbgvlsxs.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3feypbozk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3sudkztab.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dbyywdcg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3hwrtsypk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3eamxdvaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxyfsfcf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3swwfmkmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mdqhklps.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3gplltvub.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xlofipdw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uftlxxdb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vulmxscv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fscsxmwd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jinojnzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xsgsxsmt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gqikxytg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wiesscmd.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nalihhuw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qwgidxgp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jdhhfmou.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdndgzwl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3figajpqn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqxknugi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xywyvdna.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3swjqybno.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kssnupyr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3leinledh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rhgjcmor.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wnkngibp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vtuanhdm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3owfjdbrx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ykvanxsk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3vwjbpfcf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qevegidb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lbmzuymv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xmlhsudc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yvpaveeq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzshtzwa.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3laprztlz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogcwnovv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxwtmnhe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3czhuxywi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3evdwsegq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3igutsrut.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3wglarnjv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zzlvkxuf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3sqnuaddl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nuiyhfzq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnmmvpeh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3cjpusgqi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3jzznlrcp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iagmrjvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwtjtxgu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3qbqybumw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3muvtlsqj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nersgizi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zclshojf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ytigzhuq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hauvrjgs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3tnfpoijh.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbcczsbz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3haxjzmfs.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dseillxp.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vofuhwoi.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kvskxscx.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rzpfzwbp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3whlmnjak.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3onetwisw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lzgtljuu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3wzghgnis.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jplbndgw.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xcqoocub.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xdyllgym.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3qsyppgvn.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xehiwrkx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3wzgwlbqi.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xtcenruq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ktcivwyq.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xszeyawf.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3zvkunnmy.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rpzwyefn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ozmhnpna.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3wvivrrhc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3uvkjnlla.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mhbfglko.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3vpvpplam.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3jymwqkay.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bsdbvzaq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3hqddfgak.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3krmmehrb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3euveamjt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwzkww.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ihdwruyy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3eqmaavgp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3czctkfmv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3gdwaqace.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvohyqx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pteymkcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hzsxazoz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3zywcrsir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alqzkpnx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3toywijgc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3uebyjxlc.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lzkhsgre.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmqkasjl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ywphlsnm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3qjfueouz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nvfvvlvz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3kecmrjrf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3ixqhrles.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ywxpweny.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3eiarfnrv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3fbglwtkt.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3iekjaxkq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hlxbptob.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3smqxgfgz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3amdbxzmv.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wzuiupdj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zjnhvnah.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3iwlttjlz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3zvporgpv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nxbnzeql.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqnxpsar.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3paypveni.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3ztvmnqcv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3boxzvlxz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tygfsvzx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3bdyooxwn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3teaviyaa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxrdwqyg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmhlvtka.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3yxzvlqkg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3hegeafda.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uaerpeka.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dpotvqsi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3uxtspynk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3sjwssvhy.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3axprgtvd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3wrivmdfa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3vmwzklmb.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3dyqsllax.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3estwhfyn.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3jgdfmasy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3lrbgzahs.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3fspcyvbi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3osedyivk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3njfjvnyk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3mmhvhqgt.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3bnqutpbr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3fmrwxars.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3nqpcmjmz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3zhltlpri.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3jhqpmkxe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt3qqufkgqy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gjzjyqgk.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3aqvtjudo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3xqvesglv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt3dgyrumbh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3idtligtf.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt3wsdmowgg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3ovlbszvj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.ydjk.org.cn/Article/details/gt3qqmplugg.html

Ruby: s.scan(/error/i)
来源：http://www.ydjk.org.cn/Article/details/gt3rkeorimr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt3fnkqkddo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3sduxrsii.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt3rccbhrgc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3gktumsrx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3agrymxll.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3uljylqna.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3enadaynb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3aquwyity.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.52xcode.cn/Article/details/gt3zkpcqmvr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3noeuhtll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iqqygkcm.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3khmuwskj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orahegdk.html

[J01] 获取当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3umcmondc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.ydjk.org.cn/Article/details/gt3mbylhyvs.html


<!-- 参考信息 -->