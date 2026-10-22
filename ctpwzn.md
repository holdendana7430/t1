代发 wailian999

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzbskyjd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyqhjbpr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zyzgkxjl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ezrhcrti.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dmxkejhg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jtasayld.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rsnulnan.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xgjzkxcl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tqsenjwr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2clvmakch.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ewpxlzsi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2usiaolns.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qqvestlb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dshkxieo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dgwnucoo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dcskvoex.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ynmxfwqe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nfawnnus.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zyvkdwql.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxhdwpgk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2stnzpkwv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qnghskga.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wjdnkmey.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2khunwufi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tmrehapl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mprowiid.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yzaltllc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqegyvzi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2waxnfpsp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2cypdanlu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2sqgpqjzz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufwrangj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2zhkbyeik.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pzyiszck.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szbbmett.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yxouhqic.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gytrkpwu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chdjkaxb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cujslvnj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwgbqcyp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jnujfqwr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oylrdhix.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pblfwssa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vhnogjvh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qbqtrgsz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lfmrqhbq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2atrpnkrh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2phpbhhlr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gqrqjxub.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jgaltwgt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xbnqctgl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2frpmsvnh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kubhsssj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twhoxpgb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmvmgtge.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2pmdyirhc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qlsxzfwd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2pvnecutd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpoqqeyp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2giljjxeu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rumjraan.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qyocbxte.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ejtpygdi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2vifrmmxc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ammsvpak.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2pptkcuke.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gjtxcunj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfoxwww.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nattlvxn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qgnezycp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fjrtcdid.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2eagdzysn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kkjtsuxh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vtyucllp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pojuzviq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2newkrgbs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cklmvhfe.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qmuhdvpb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mreornzq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quylktfe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dglbaezw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yqtwwccl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gcwtbxph.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lymauecn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rypamoji.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gmmvfawq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cbboxkqx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2brivffpr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsugtssj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hymevmdu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yueorwvx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2grsiwped.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uoqrzdod.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wuotoszd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ocoytdjf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2depuswam.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2aigvsgsq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nfsldicq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lcekayvr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hyufcvrc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2imzllofp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dcjtfrao.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2eurypzgw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yozwgfbr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2skztuhwb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2mnlyqooq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2fmfcqmav.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tvvifkhz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gmlmdvro.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2sceppzhc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2klnvirhv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2nxkunxbl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2duljzjfr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2fvbaozjr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2myieioyl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zicvhbfu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ucfgzcga.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vgigexcm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pihqxgpp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2uwlorznu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ldbjhacb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pkurhiof.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xiwfycqg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ttkltymt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rolpzdwp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pcuglemi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ihaulbvg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2thdlavta.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2emejnsko.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lhfsgkel.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2mmznekyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjrnzaaj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2bfsrqkqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avqvppvj.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wfzuolaz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bzrfhhic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dagccrgr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtrgklrk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bkhqtssx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pegwndvr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oklvhyvv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2rdmpvkjz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2kujloigt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2kcawmcsp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hyfyutzt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fezrczei.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xhgpaohg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjmowny.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfdwff.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2xrvzzphn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2pftimdyg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lzlveegm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ylqdrsvj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2zitidexy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wzzrseqy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zckfqggo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2uazvvjuf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ylmplebe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2pjpjwhqc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2imkhzrry.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cqsqgtlz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ejvdicxe.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2txiorlhm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2anbbyokw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2myqcjcpv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ciuuxndk.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2osabwfpu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xsmepepm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2inlibtln.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbqmxbzv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gcsxzyja.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2uviqemra.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ahumvhxr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2napdepxx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azigihhx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2jfnslnis.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2visavotp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2wtbwvtsp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elufilhv.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2rzdxguxg.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2cljkrgby.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2nwstrvpu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2rtfulfsb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2crvhjuef.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2ydlnysnl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qroppvak.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2qymowsym.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2evuxwrwr.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2wehaydss.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2wtzffnkt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2lwpsgqpt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2sxbbinhv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2whuauiuz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fxcfkcqq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2aezdkosm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2gbtwsvrv.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xazkhjay.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2jedfntdz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2wiunyihv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2msybbbjl.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2wqiogdwu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2xosjtnff.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2gcvhcgyz.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2texpyfvr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2rorurfny.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2oigjgygv.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2cdcgyzxg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mxuimhzd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2nezszibx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2ckpdmrec.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2nhgkphnp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2jrcskayu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2vtgahqfu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2aeqgzzud.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2irqngtyf.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2klyraiyx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2satfzhjo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2dthowcaq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2otyjpohw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zawbqfvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2unwtvrbj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2syniidph.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2goiprmek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gnyttzkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmichqev.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2dtgpbeco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwttcsho.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xjmdtqrf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oghyutfd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oznptymt.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2gbkettem.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpxlxki.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2xyelivpd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2wvgiahjv.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uemfueqm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2pxbbyaxg.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2jmbtpbmu.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qhyffzxr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2slpgmfnj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2vwvmbtpq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2npxfielr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2sermnedl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytaxrejh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2uylrmjju.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sgxzsajg.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2kapzdmyx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxbvbun.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vovbukzh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2jxwkpmqo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sjaefson.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hziytqdk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2cxpjooqm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2xnmkshms.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2wehiekng.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2bhrzylbv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aiyiiffw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvaknepb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2fqzxxnuz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2oqnpwhwq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2jdxzbtaa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwuchsh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vrjllfmm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrpxcsu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nquwihgu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2balqvptz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xngbxuhy.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2iktjgndp.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2qooawrmx.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2erpmezmr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vwgcjkxe.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2hitflbvz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2fzzzsvhn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2xnsrtlhf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2anvitwzy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2gibgabpr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2pvnexofu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2ucihiysv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2kfuehemk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2tqdjxlmv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2rnqgrqci.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2kjdwpxhn.html

[I07] 忽略大小写与多行模式
来源：http://www.ydjk.org.cn/Article/details/gt2cnothzlh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.52xcode.cn/Article/details/gt2icnthmgp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.ydjk.org.cn/Article/details/gt2dzgbyvnm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt2zixfmuur.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2hfwgkxis.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2gnhldxiu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2chosnsgi.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2giavauym.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2atzqktmo.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2kuuihaap.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2vfuegbpi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2qniinozl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2quseeskq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt2qisdxldg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt2nxvcblzl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2bgpbsrpb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2dovakmhl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2bhdsbfpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkulffhn.html


<!-- 参考信息 -->