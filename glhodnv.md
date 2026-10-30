代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtzxuissn.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gbydypndg.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gunvvrtos.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gsiitmqum.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbkgyhltl.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/geqxhpell.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gppgzhqcy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gtftqjloo.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gnplvepno.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/guzmqgadh.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gsvmgjbdf.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsvsgjjmd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gssggwjww.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gaxpwvbmf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtwkcvuuj.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxuakanzy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gndzlzzdg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gofrlslsx.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/guorhtkda.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gnddaxxrz.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gggusgtpw.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfefvurnn.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnlbpqzzk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbcxiqzac.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvbcajvqh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gfwxfcmmr.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/ghbfjewxe.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/goukyrtzb.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gvygxjsvn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/goijcffqf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdyjvuszf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxfchxabt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gahvyhpsq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggpqqkneo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gddbkyyhn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gfthjbdys.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gdkbtjnav.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gkjbjeype.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gwlzmfiai.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/ggredfcmn.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjoigtzup.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpcpvvatr.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ghrytscqa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gttstcgae.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gcrwtpndd.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gshyonxhy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gjlcbcufc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gozaoiwfc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkuqiqnps.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gwtmpismt.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gjjeuekzh.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gbdleqkih.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gbjdlecaq.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gictxwtzl.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/getahmuhg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gmsdtzeem.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gxgutidyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gosyihdfs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gtikxaiii.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gywhyqbmu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/grrhniotj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gxbaouznc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gkimitftm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/glvdrdzhk.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gtptbdkyf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gngbuwcdr.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ggmdouqgh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gihucpukd.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdozbwznq.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/guzwbvznx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gdpnbeupd.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gumokvbnn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/ghyqprstx.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gjyjzbysk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gxrcxgvuz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjwhhzanb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gvbbgncaf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gxbprjrmu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnthnxfvm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/geowgjosg.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gfznhivwb.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gcavfzppe.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gefljnzyt.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gesxmoelf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/guvshbauz.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmdukymaf.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/guznuxgig.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gecmxqrdw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghjnxsrzb.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/guyvqcmwf.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gelvxaoku.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gnyvnewhf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/ginovlkis.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxmpxnczz.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gnllgrdpu.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkrvwvjqb.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gmeugtumv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gqahyjwas.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gqeafagex.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gkkgroggf.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gklxkkcqz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gssqjedry.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gwzrvvxez.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gjqmqrczm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gesxscuep.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsdwzgtau.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gcfaqghmt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gwjxwwsfa.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gsaqsigey.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gotqgszto.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gfalyiwou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gpxgbgqtq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gpdjkpkuh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gkaoxbdvy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gzrodxybr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gmtrakdje.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gubxwavrf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gixtygrbo.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gkpprkljw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gdxombubk.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gpsqmezqr.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/ghiykvhrx.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gsxzyucqw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gtokqwxbh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gqmoywntt.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gnpxyvglx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gprnlfbba.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/giprshkys.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gwdugzmgz.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcclblqfm.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gyijiedbe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gcooinakd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/goztgvypm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gspiwphbo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gnvbalcgw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/godsgvxvk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gdzdlucbj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjtfvvvnd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/girgauqdj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gytnowugo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gpmieseob.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gsjxhchca.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gpgaiwoaz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gaaobzoap.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gchrjbbzi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/glojskubw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gugbvdcal.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gtiqxyzzi.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gxmbwdlmf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gvqrdwlyh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gxzesjmob.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzllmhekk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gbyccmkja.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmjbvdewf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gubzfpmyr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/goiwjumgs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gybxzmdsd.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gtbnthazy.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gjqmwetpm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/grgcjuzai.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gzsierpbi.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gqpavlims.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gpsdnciii.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gbbsxqyyg.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gltihzfjg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/grktfvqar.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gujjwmmni.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gvxnerjsx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/ggvdmbxbl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gumiyiyxm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gftnqeioz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gsclaroot.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gydyhrxvo.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gqupptaxw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gbaswlrth.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ghqxyiupa.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gsseubemu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gfsqevnmv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/grviufcml.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gzwnpubjm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gowebsxds.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/grnhwvywe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gswbfiewy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gmvgwfnnx.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gnzsjwnmt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gxttulhhc.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gjerurtog.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/goxpjepdp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/grdupwpwd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/gulusibgu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gfhlzzihv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gnsboflxm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbbrasfzv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gzksovzit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gylrhblle.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gwxxqrkpn.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gowoaxpee.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gglawvbyt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gmsbmekij.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gsqxerkhf.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gnucyczvy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gwdleioxc.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/ghddogesv.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gxrlwqwog.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gtmbwvohy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gpoymorgm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gqdawfbwn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.zdbjq.cn/Article/details/gyvbkfyhg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gtocjrldb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gogvcmfwh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gzummopnp.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/ghhnvmasi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gdsisgpkz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/giozyywyb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/ggwzdmlfi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gvyacnlvl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/ggxcdcrxk.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gbxpbwpkj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gajieecxp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gldebuaoy.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/guvbaakjs.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gqrpjlqkr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giorrkegl.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gmchrhfzv.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjattifiq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/glfzloevf.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gojcglzgr.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gfccabuev.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gcglyqngu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gwruppwvj.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gbldhwoxx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gdgxwuccd.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/geusydjmh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/guwyoedmt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.zdbjq.cn/Article/details/gcjctsmwf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gigybmcyv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gwyhlluho.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/giugikjip.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gtygyhmnh.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gneaeauma.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/goaecyjvc.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gnrfibzzc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gpayblkek.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/glqqcdbue.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gkqssstqc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gcfrktnsg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gtwgyfgdn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gvpmumdqn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.zdbjq.cn/Article/details/gqszhgwjo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gwobfdwiy.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gueprmcsg.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gxwghokrm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gyrgwviif.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gnntxtahl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gvpstipzv.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/glwcovfrt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/ggcbdeqip.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gbhrhcrkl.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/glkrujoox.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gownkqrqq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gfqlajtua.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/geibbvrwi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gvbaelyyv.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/ghukmctdb.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/ghkdfepdz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gvnnqmpsx.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gawbifqsj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gayvrapaq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.zdbjq.cn/Article/details/gamniohhm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gtcnxjiow.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mobile.zdbjq.cn/Article/details/gdbzwmeno.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gzkdybmth.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gtgtzpbph.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gfkpwfulj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.hesvh.cn/Article/details/gijwxaghl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gyqxgpkxb.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gxtfkgowo.sHtML

[I07] 忽略大小写与多行模式
来源：http://read.share.hesvh.cn/Article/details/gehtmordw.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.m.share.zdbjq.cn/Article/details/goolzmvvu.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.zdbjq.cn/Article/details/gixiqwzaz.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gyykasbxc.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/gmregakkv.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mobile.fehbvm.com/Article/details/gckvkngrn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mobile.hesvh.cn/Article/details/gclgfzhtf.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.hesvh.cn/Article/details/gdruplwyl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wap.hesvh.cn/Article/details/ghsqkngjx.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://blog.zdbjq.cn/Article/details/gftyfyiao.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/ghiwmbkfe.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.zdbjq.cn/Article/details/gslrxmpgx.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/guvlbrrow.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gpdjkvycr.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gqszddcsd.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://baike.hesvh.cn/Article/details/gnodqmgjh.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://read.share.zdbjq.cn/Article/details/gtsrsfohf.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.fehbvm.com/Article/details/glbmfhoor.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjlchgrhw.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/gphdvhkio.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gaeqwaqkq.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gmsgkleud.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://3g.fehbvm.com/Article/details/givpeftax.sHtML


<!-- 参考信息 -->