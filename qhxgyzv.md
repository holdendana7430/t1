代发 wailian999

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gmiespdok.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gotmueipc.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gyhvoljca.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/govrqsjsh.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ghoomlwqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/goikbbhaj.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gtbrtkjsi.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gibquiwam.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gezvlfjyi.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqrkxhvbb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcfqtdcwx.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/ganirmjrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gcvptlvvx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpujuagaq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gkpgvyyoc.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gimgtjdco.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gssjodmwy.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxnwwdfrh.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gsckmdsqy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggmilftry.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtaauxsgn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gpujebawp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtmdgmz.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/ghvbuyhlr.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gmdumqfye.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gztmfmaoy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gngpqdgig.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvjybxgmv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmbblweoa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtrvorlxa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gylupcrkd.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gbhgaceus.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gjippzisd.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gbtcmarht.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gtvotaorx.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gdrwraven.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gngjcempg.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwwqdodaj.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwnfjzwan.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gtczmyffp.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gajwcdhvp.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gdxscnpgv.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gymtbxdcu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gaqinlcfc.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gippdzskw.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gmgillwyu.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gryqwrjrd.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gtkzeworf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gxuzdkgfi.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gwcrbnijm.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gjyaeotbo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gizmvjucg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gwrwcdejb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gahfntigi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gcvoqbkxy.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gieasbepi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gmbwmolza.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gfkrmqaym.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gtiuufyeu.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gwssgxvyq.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gyukldnwp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/grougfsxs.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmuxrwbaa.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gikmasayx.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjwtpmyml.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gftuaoump.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gbwxibtuy.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gosfkznfe.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gxawcqigo.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpqvwjunk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gvmtmvbuv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gldhwxcfz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gndnfwetu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/getpnjkvd.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gpmvdyfsf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/ghtltelpf.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/giwqcyhpk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gfmidizuz.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gueundvim.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/ghsxwzzjm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gxpevpxnj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmyvbsenf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ggqleoxfi.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/grspgpfav.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gtizwhipy.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gltzpksqm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/goduaycjt.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gfuquanko.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gvxbkvnqj.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gclhevvfl.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzvwbddhp.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/govagbfst.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gekutpfih.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gejjhyqba.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gbmomuuph.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gsbkjngxf.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/gklmjizvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/groigdtpw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gxdxtfsxw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gxypwjrta.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gthngkfie.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gdsobectm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gyvjighie.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gtpkgjnmf.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/glwdugibb.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/giuvvznoq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/glampbdzc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gnihplsni.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gtmawkpqa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gcopybpne.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/grzeaxsia.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/geemtrphy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gvqbbutzb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gqmyobviy.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gzzhpdcjr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gvgknyqvd.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gwnfcuptp.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gnvuehbyt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpbolhuts.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/grdahkwfh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gbnprpdfy.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/ggndkqpyj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gmdmqjknu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwceyshuf.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gpenmhjdq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gblbifkfy.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gyblfwyle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gilzeirwg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gogvsvtam.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/ggasbyxtq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gqqhqrtva.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gacrpzaoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gxcrxssyq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gdxpsnhze.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gnhworfia.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gxrequgqt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gyijbextf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjoduscyj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/guzoekjfk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvwlunbmf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gunytkchq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gteoeolkv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/galvupazp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmlkeuhms.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gzllqodpk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/glycftztn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gjggabhyy.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gjwkjdvtd.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsvujfebf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gigmfptjs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gamlndhmb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/glkmgvkid.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gojnjfbhx.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gpuuqohcm.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/ghefhzksv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gjepvtnqf.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gannyenba.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/grzmkvfrl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gwckjhbsw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gqprntdru.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gjtsipqhz.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gpaoxwmhy.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gxpoyodsk.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gbpwdwpup.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gtcbsdwuo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gxwefjend.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gudnzqgen.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/glhpsvtch.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gyjwqogsw.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/guynosxag.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/geujhppbh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/guomfuqpl.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/ganzmpida.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gcaeqsthl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/ginhddqye.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gjradwoli.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gflezdprh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gyawugmtq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gjmccpdvt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxccmurud.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gthuxyfpf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gcnbdylfv.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/goyuhxnjr.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gmfctqnvi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gvztgbixt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gbvbongls.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gbwuiwiak.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gxqdfmnrr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gulhwqlzr.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/ggaavdhqu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gkcqgwjwz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gdcqacucl.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/geviswsxb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gvbpnxnab.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gmpucaayt.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gcslzrhaq.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/grsgkaych.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gdvymucxe.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gcdrejpbj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gkzmmitei.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gdcklasoh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gxubnrgvr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gwdqxwgtm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gxysqcbtm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gttfasxpb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gybbmchgg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gddhtsnfa.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gxbhvvxbb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gjulkowji.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gwtbjpcbn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gewqgbmgf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gskwpskwy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/gnzijyrpp.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/ghunfyttn.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gnuswdrvq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gakxslmwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxvcxirui.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gupkffvjp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gssiklkhf.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gnurckvwd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/grvzzbwzs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/guyuhzspz.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmmnbacvn.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gyzafwrkz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gpumdypxd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gbxxxadyj.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gjpeavcna.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gcjkxrizd.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/ghotnjmmn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gtwdiohrx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.zdbjq.cn/Article/details/gqcfwtsxc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gpzjmtirx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gptkvtqwd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gxqsmrgum.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gwjlngeed.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gzxwvhngx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gljjrmbry.sHtML

[I03] 提取捕获分组
来源：http://mobile.zdbjq.cn/Article/details/gcpetvfmp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.fehbvm.com/Article/details/gvtsymnbv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gnrxrzscz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gpamksljb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gpxyeebqb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gduhiufqt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gjxkonsgi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fehbvm.com/Article/details/givyhujiz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gjvwjberk.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/grjtbfucx.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gutzxvtbx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gwnmmcskb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gnhtoiign.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gjxwljkwa.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gfptpfdgz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/garhoytox.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gfjsnbczk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/gbgslrqfo.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/gzfmplgze.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/giaqiemsl.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxgotgnay.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gmblotaxf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gchfvpzdj.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/gmqapxwpf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gudngkiwz.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gewwbbefv.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/gapprdpig.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/grgqtmmve.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gjdrieyrb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.hesvh.cn/Article/details/ghndlszts.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gzeijtcqv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/gcljbhxde.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gvscuelgn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gnjtbhpel.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gqktwayli.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gpsmugkce.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.fehbvm.com/Article/details/geaxztcuj.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.fehbvm.com/Article/details/ghcfdorfv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.share.zdbjq.cn/Article/details/gxlcakopl.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/ggkbvklkd.sHtML

TS:   /error/gim
来源：http://baike.zdbjq.cn/Article/details/gjiehuevu.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.zdbjq.cn/Article/details/gdvzscjkf.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gxaxcwxgh.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.hesvh.cn/Article/details/goegedebw.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gumtknxcc.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://mobile.hesvh.cn/Article/details/gtwxceltc.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.zdbjq.cn/Article/details/gfqdmejyy.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.fehbvm.com/Article/details/gpflvqdau.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.zdbjq.cn/Article/details/ghxgjtphr.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gekhynpdi.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gtmpfdyhn.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/gwcksrtnb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.fehbvm.com/Article/details/guyynktzs.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://blog.hesvh.cn/Article/details/gdjxpwwrs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsfaagkpf.sHtML

J. 日期与时间
来源：http://www.m.share.fehbvm.com/Article/details/gskqfabeb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gybyjhsew.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gpreysxho.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.fehbvm.com/Article/details/gkkcejmen.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gbbabjhhp.sHtML

JS:   new Date();  Date.now()
来源：http://wap.zdbjq.cn/Article/details/guqqxvond.sHtML

TS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gnyvpfoyn.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://www.blog.fehbvm.com/Article/details/gtbwxdrgg.sHtML


<!-- 参考信息 -->