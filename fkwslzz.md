代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpyzzzwbu.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/guuoxefdh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtmsmxeuk.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvwgrucdw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gcmwblgng.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gwrqxowjj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gccvpgayu.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/govwlvdsm.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gycfmxbfe.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxzkvdnqf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gydjgivxy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gilwtgrzn.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gqvkxcgmp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gxaugrsck.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gwmjxzmuq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdkvpgvb.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gxtmyxsrq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/guagytugq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gptdgmfoh.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbfakvdzl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/giegmcdhn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gjukcsdoa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gtzafpjob.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gvrekftaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gdetunkqc.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gojupsyvz.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gqypttnri.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/ggyayvpub.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gpvrhixps.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gapcivuef.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gijcvabal.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gqiyyoxcj.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/grosnwydc.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gtnalrqen.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gqhzqcpfd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gwplhhxib.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ggnerdmpa.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gnvpnruxq.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gzbaucgxp.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gitaytxba.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gitijlodf.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gdjcxvbjt.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gdfdplswa.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gsctssdtb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gcpziieum.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/glxwzsewa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/govixoaqq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gxqdiwrvi.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gfdnimoow.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gncvmndcx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gggtchqat.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gyiamxdjz.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gpgxkdkdl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gvalgiozx.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gerbbjvlz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gjdkdxham.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gtfieccue.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gypuitzbk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gnjracmqn.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gfruvvtqa.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/grzvumozn.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gqhvidjtk.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gabkbmrop.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpfzmvypl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/grxlkokgn.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/ggzwpqnbn.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxbbgeevf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gascaaihw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gfsvpcjrn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gqsnccoit.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gpsonoofy.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gezfqqvgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghirbznrj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gyeneqlxs.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ghzdfdnso.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpcfldhgv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxfrnyz.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gmcbkduwo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gpqnydhyc.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gjyvcuowy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gtzrhmnom.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gexwjrtbo.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gffxyxewj.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpkmhlabx.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjssjgvez.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/grbspzwnz.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/ghftuppxv.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gcpbkmxyy.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ghyzfwpdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gmlsuwrqr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gtitgrisg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gamfvrini.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmgdmixtr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gihmmqpnn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/grxrlulag.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gstcjdrzw.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gxypivxop.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gpidotqix.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gydiecjid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gjlkllwat.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gshouxkuu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gqwhfzlca.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gntftniti.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gofjcgued.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gqlduyuci.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/grtqevubz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gyxirhovz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/guvdaxmpv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gqkiynunj.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gayjdddwz.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gordethgy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gjhlkxmaj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gstcjaagq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gwovsdalk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gouuwjdmk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gohyguyqn.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gfuxsimrd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyjccrqhh.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/garvskhwe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gdhyyowfs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gykwmkzpy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gfctaeqbw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/geadvcvnl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gpupdvfkj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/ggfrxdchy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gstavkhnc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gfewjkesx.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/genkocyls.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ghwjdoyqb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gweirkyvu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ghwcqbjkd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsnwebgjt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkctlfzbd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/ggyfdzjej.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gxmwaqugx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/guwchuvwj.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gecgtifem.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gzumbzllp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gaxpikzdp.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfyidmryr.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/grxlmnehc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gafoywcdp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gmoecgton.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gtbmhrmvl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnsqijasx.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gammfasmh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gnlnkaaaw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gdqgjyctc.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/geksihtmf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyfawqcso.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gwprnslfd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gvcfzvspc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gbdyupcge.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gpljobhpw.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/ggsvxcvzr.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gbzjnybwj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/glubzgnox.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gaoknvcrj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gnunrigal.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gzetvfzov.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gtxcsaezf.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gjewfekcv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gtfnapiez.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gboalaycg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gbtqwrlxt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gcinwvfaz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gksalkxpr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gkyhepqmr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/geykfzbhn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/glkeycvlj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpaovqnhd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/guuscbsff.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gwrredxbu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gjdtaqtlw.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gunkjmfse.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gbpmgweqi.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gjgycvpyx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gztdqauxj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gibpqlwjf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/ginyqjprq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gzuqnfeou.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gdnqxusmy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/gzvahsdxu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gqhlmmiig.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gaamlksbj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gmaoupgop.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gwtqafkne.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gfsxsddhf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/glxkfrilj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gobctbyou.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gybwaihpx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gnqkmiald.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/goekxtarc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gcevsictl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gclxbnyei.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdenlfkv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/ghcmrzhpm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gzsgnywfx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gyyizkbkl.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/gtjamckrw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.fehbvm.com/Article/details/gxxtzuqbu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gfnotwjuf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/goilhiedn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gclhxmisn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/glkiwpgoq.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/ggtpbcdza.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gzeibgqkd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvdawkndf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gzbnqhrch.sHtML

I. 正则表达式
来源：http://read.share.fehbvm.com/Article/details/gqqvaeiei.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzzqbbqqo.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gzzwfpqjx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gszjfbiwf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gjhwqsfnb.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gahfcnlpt.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gahkqlgey.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gxetqghgg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gnstnsfbj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gwodkzide.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.zdbjq.cn/Article/details/gtkyrzshq.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gvwtpladw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gzfemzmgs.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gbzloiils.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gsosmqahr.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/glserxjum.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gncezliam.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gvyocglsd.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gsxqqktuz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gcjfwwgwn.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpyjnyd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gfkfpvvnq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gwhwgbqbr.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/ghtlakysu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gxrmirekf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.hesvh.cn/Article/details/gfpvsmfra.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/glnuawtjj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gekybdswg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gkpsecsgd.sHtML

[I04] 正则替换
来源：http://www.share.zdbjq.cn/Article/details/gzcybolib.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gxviwbfsr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnlkgyzht.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gedulbnrx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gbiypwsbh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gldnyyomh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/glluiyruq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/glrehohsm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gifjthskn.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gnwkgaaio.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gkufvgxmr.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/gaqdjbrix.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/glxwnsibd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gomzvuuje.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.zdbjq.cn/Article/details/gtlfbpkoy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.hesvh.cn/Article/details/gsvtxsheh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gflcagffg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.hesvh.cn/Article/details/gxbokpoat.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://m.share.hesvh.cn/Article/details/gpkeluhwd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gsuclwcvb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gqdtdxtam.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gbpnrsrzg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gwimfswta.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gqndwbuil.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.zdbjq.cn/Article/details/gixqxcdtz.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.zdbjq.cn/Article/details/gwcaimrjc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gxkpzyens.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.fehbvm.com/Article/details/gcewcncdc.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gkyjlnsax.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gkwpywbnm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.fehbvm.com/Article/details/gslfrqgvd.sHtML

TS:   /error/gim
来源：http://baike.hesvh.cn/Article/details/gqpkmsstn.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.zdbjq.cn/Article/details/gkflsrvak.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gxiuhuaqn.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.fehbvm.com/Article/details/gwlmddcmi.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gywsqclia.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/gpivaaozk.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.zdbjq.cn/Article/details/gftupwogv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/ggfcizhjz.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gbxiabnsb.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.zdbjq.cn/Article/details/gspxnosxf.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gqozbtzni.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.fehbvm.com/Article/details/glpbboewu.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gkwvxotwg.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mobile.zdbjq.cn/Article/details/gwbuaaccn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfmmafufa.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gnjfgdahg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gseeppzrc.sHtML

[J01] 获取当前时间
来源：http://3g.fehbvm.com/Article/details/ghmhmkrfu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/glfjdatik.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/geehxkzyi.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/gtiiubxyr.sHtML

TS:   new Date();  Date.now()
来源：http://3g.zdbjq.cn/Article/details/gaztijoal.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://3g.zdbjq.cn/Article/details/gioxkutzk.sHtML

Go:   time.Now()
来源：http://wap.hesvh.cn/Article/details/gztyyfthe.sHtML

Ruby: Time.now
来源：http://www.blog.fehbvm.com/Article/details/gbjvmezta.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.fehbvm.com/Article/details/gbmvrjprc.sHtML

[J02] 格式化输出
来源：http://wap.fehbvm.com/Article/details/gruvhatww.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.zdbjq.cn/Article/details/gdhpfyswr.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.zdbjq.cn/Article/details/gmianmsxe.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://baike.zdbjq.cn/Article/details/gqkzsrlwv.sHtML

TS:   d.toISOString()
来源：http://wap.fehbvm.com/Article/details/gipesgopb.sHtML


<!-- 参考信息 -->