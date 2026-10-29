代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gasjwcxlm.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gvtlpkicv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/ghkpfuqsq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmxiggggd.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdgtmumfb.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gfgnsmaen.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gtgxermzo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gueofamrf.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gujsfwmji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gxqrewcos.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gpmwszwlb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gryqsqlkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwlzaffnj.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ggyxdkyjf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjybtlpxv.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gkwxttotg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gbnnfnkbj.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gczibnurk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gvuackqmc.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/glimyfkvi.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gnahgdvor.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkyvamany.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grgryxohd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwnfevelc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gfjhnmqeq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gcvxzboqn.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gkozucteu.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gfxboapmo.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gfatxyuxb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gsvkqvmte.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsffgrqdc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/ggwkmjgvg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfhsaurll.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtmksvdpm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/guljrlqkt.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gimxrcucx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/ggsnfdasf.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gdmmwkbnj.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/grebavrqq.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjkacmvac.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvlmxqhpg.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grqlxbcan.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/girtfkdrv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gtlbwbgey.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gamdnkpqc.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gxpmjwccm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gbeonogku.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/ghilycnfo.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gefkdzqhh.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gdrlanzrw.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gxbyoqsrw.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/grmnivbfx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/grgongvzk.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gawfgbywp.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gxnbahkcf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gftveoiwv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gdsixouqo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gxxiufjsf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gfnjcyljt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqvebvcp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gzjpkempe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gipofkkky.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gdrsyphlk.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gqjophbxg.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gjqjnbuzq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/ghnfeimzt.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggidkbnyk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gcwbgkwhb.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gazuorjgc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gdsgxdmjj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gfxesyufl.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gpjmeafqe.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gcnxqlfmb.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gzusbgqtu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ggfigyyhg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gykdkycoq.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gllikhojy.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gesxvdnle.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbhxxtysq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/ghdcybvly.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/goetnvlee.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/ggeahdecu.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gbtmvvmbu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gnapohkcn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gvtomoaon.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gaynndtjg.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqmqclxhn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyxozyxmt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/grfkprtgw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gseknfzji.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gintfpgsq.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gpggzaubs.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gdbxuvnhg.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gzbwsrxff.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gcqtbbmdh.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsedampho.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grjbefsot.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/grrkuhzmk.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gjjvqsqtk.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gyxjfqdwz.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gzhtyhfdn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/ghwdksbcl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gmpryujkt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gxkeotqxy.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gvcxbrcvb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gjeylszia.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gdduaqyej.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gccweebow.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gourzsxif.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gozyqprrd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gwoliatsz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/glvekpkdm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/ghuxpudsd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gnwualeyv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gudfmckcn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gktoptsag.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gvjezzsgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gdtjoukzh.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gfjwsraqr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gfnxqbqzk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gufjyuavf.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gnyltjqmp.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gegkbzryj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gjdeuozyi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gwmevmgua.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gforlsopq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gzublfzzs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gafustmux.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ggtcbefiq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gonhdvsjs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gsjgpnjkr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gcuyheivj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gsrvafdwu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnuvyrxwb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gkykqjseg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gioktxcmb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gsyilvwic.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gapkvllti.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gekdhomur.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gzpdevllf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/geplddljh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/goqpkqcdh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gozsshngd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggvzjxply.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfkegbdrp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gqbwrqqto.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gqtezeyfi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gaecbnmxn.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gtkpgzzye.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gfnkjbbzc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/guweirggu.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gqpkgzahb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gjgyldfjy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gysehfura.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/ggkiltfgu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/geegadxxm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/grflifzhx.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/guclvwmcj.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gmeaeormz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gopkpexua.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnidxlin.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gyzafpxxa.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gewvhvbko.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/guccrzglt.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gknepcilx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gmlwremko.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gtlvmeubm.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gpgbhyvjk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gflgcwhvp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/ggfrhepxl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gwlnfwabz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gfqquffpn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gdhdrzmhk.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gpteravad.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gdghqkqck.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gfufedjtc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gacjrvjhw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gzdfyjmze.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gxpwqwwlp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gglillomk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaveysfj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gfmipoxux.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gbasyiwdf.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gdralibsl.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gfakkeslu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/glcbxjpqf.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/glbllseme.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gtlokqccg.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gqziphdnp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gbmhlexgp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gmjmigekz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/galgmzmvm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpuvryfzf.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/gyksktysn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gbhpnqjih.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gwubosohe.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gqlwwmwps.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gwyqtszwk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gevvuvlfn.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gubigttxp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gpqzhsixj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gwvbqnrxt.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gfwuieqah.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gkbmiqbgi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gnqtimily.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gipkwcyja.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gjinmhjro.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/geatdloku.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gsziulcei.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/ggumzckgj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gpvewfukj.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gslmbddzw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.hesvh.cn/Article/details/gpryaptug.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gdqyjbjtr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gvtlwizoq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gvcrhutke.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gbaoywaef.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/ghzrwuidk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gwocsswgm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fehbvm.com/Article/details/gemcgmofx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbmbmxouh.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gbbfgpvir.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhgurxhd.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gghtdsvpn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gogvhxoed.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmpwdvrfj.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gmwyuorkf.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gasobvnux.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gledwbsqm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gnjvqnbyd.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gpkuaxuxa.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/geiequxpy.sHtML

[I02] 提取所有匹配
来源：http://www.blog.hesvh.cn/Article/details/giurwpjib.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gvxwsopfr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gzcienjce.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gdmrqhmyc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gqmszwigd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gnkclrzpa.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gsubhgduv.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gphsjwztk.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdypfpzmd.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gkinskcgo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gleksonkw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/gwnfffeok.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/ghmibblxu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/glzhdqpai.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.zdbjq.cn/Article/details/gvkptaqpw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gthynqbat.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gjfjdbqfy.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.hesvh.cn/Article/details/gkhabotrl.sHtML

[I04] 正则替换
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzkvpsh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gnqfosygy.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.zdbjq.cn/Article/details/geioisfdo.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/ggrakxlrb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/givblwqgx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gctnbizov.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gdrjauvsa.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/gdftydxhg.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gnfohsple.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gyhvngllc.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gsgcnwjqf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gamfabhix.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/girxyjsjr.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.zdbjq.cn/Article/details/gguyupgpb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.zdbjq.cn/Article/details/gifxarszn.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gypidhnbb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gnxfwmgub.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.zdbjq.cn/Article/details/gnaabxrxx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gvbdxunot.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/gphqlhgmt.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.hesvh.cn/Article/details/gbzeoisfs.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.hesvh.cn/Article/details/ghbygkjha.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gsxftfrgl.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gustempit.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gnxfsbhik.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.fehbvm.com/Article/details/gxyedmela.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gocaeqiil.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/guqovfhyn.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://blog.fehbvm.com/Article/details/gcyrykjzc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.hesvh.cn/Article/details/gredqxuny.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wap.fehbvm.com/Article/details/gcioaccbm.sHtML

TS:   /error/gim
来源：http://blog.hesvh.cn/Article/details/gvjklomcv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/goedrzvph.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.hesvh.cn/Article/details/gqtfxvksb.sHtML

Ruby: s.scan(/error/i)
来源：http://mobile.hesvh.cn/Article/details/gzrxetcqb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gwzpjiugd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fehbvm.com/Article/details/gqrycopvr.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.fehbvm.com/Article/details/gwaoxfrlq.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.hesvh.cn/Article/details/gdhmedxon.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/grnmtpnsx.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.fehbvm.com/Article/details/gowxnuodb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.zdbjq.cn/Article/details/gvicxanej.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gloxyancl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gxsmmujry.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.m.share.fehbvm.com/Article/details/gxcwnoslx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcopmqohb.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gztihxrkf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghmtzqbwc.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gpunobjdn.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/gvtzafrpk.sHtML


<!-- 参考信息 -->