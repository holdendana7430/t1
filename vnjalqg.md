代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzfalasyt.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gqrarfhlz.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gsppzfgas.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggzbyiwxj.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gbzbdpvkp.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gquphmtcn.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gscjmbkyp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gkjiqzvsz.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghyfjmwwd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gcluasesc.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gnyawwpch.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/grtdnccip.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grempgmrg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnerfwcwv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnjtgkupr.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/grxfcwytf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghqvtwxqv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gjpqkmlah.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gxypjndxp.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gteflzkit.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gsukznyee.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/giqgtfdfz.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gygnoqktl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gghdouzud.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxsdkejxe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gbnxqwltc.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gtfhjkckp.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gqlcimqfn.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gawzmrmrv.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gnnyoeulz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmwyjgfls.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghebiasav.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/glthfynpx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gjbfgagbg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gxhycvnme.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gusftliid.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/garcxhpjn.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gygknqsfe.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/guoekkozu.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ggipoaqtp.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gwvwmgwqy.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gpxxwqbfv.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/giexalpkj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gemqtuuzr.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gmtswdmjr.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqlbmrtqi.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/godxvvclk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gmwaullxy.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gmziqjkwi.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gnwidjara.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gocqnqmhv.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gprmuavrd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gclwcwsdu.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gkhzypiiv.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gjsuauovq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gnoknmriw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gyoqkgnfi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gddvijeqb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gqjixxkba.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gzadztets.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gecgglxbr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gxcteupwp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gngfdotra.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gqmktujxo.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gngedvxgn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gesutopvn.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gwfpvsnrr.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gpfioodww.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdeytpxak.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gttvshatk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gueaikxnb.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gbisjwhgp.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gezxyjgvs.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/guevstsxl.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/glffburtg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsrhvolcj.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gicmblrwe.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gigogiais.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtinlflzz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gcbgwrcuj.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gtqecuyci.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/ghbhnmuix.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpxxzehlk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gkorppdqw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/giaadynyf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gexeygbjs.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqsnyueyd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbswzhyaf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gmvcgzvyo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gvxhmdvof.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gtzbnslxd.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gsiiqkobo.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/geeentmrd.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gaveuouoo.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpvvwzfds.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwgerzlbw.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/grnhtosre.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gahxumlin.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gvfebsack.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gxobzoqdy.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gycvbrxoc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gmccznhim.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gwyyhplhs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gbwzrudkl.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/ghhrsqacj.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gkcvrpgvk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gypdnodmo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gcobnlosv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/givlkravg.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/ggznwvwwb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gnuocqgbz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkcgxfbkk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/grapybgcm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/ghwciukww.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gakhnugdz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gwcqgyfnp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gyonbgjoj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gkxkrinvm.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gqqodwkbh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gslqeyssz.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/glvcxmtco.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gikrghvpc.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gauvtxhwn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gmtyfebyg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gtwecqxly.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gpaaiyfie.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gvmqgywpi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giyqfpysm.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gblajfpzq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gynkjhqam.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gbjzxiqfu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gzrbqambg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gsvtaqmwz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gawaygkoi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/geqktwbnh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gvwvoyyss.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gimcvswui.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gradjviva.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/githlxoqf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gtfmjxlpy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gihnlcvmb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gyptkkojk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzstvhsos.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/glimkbzmn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ggymtfzxi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/goaxjnwsk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/goubejqbv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gkwjnhdlm.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/ghffjncmd.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gqxjgeihg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/glczldmnf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggoulkzvn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gilgrmgtw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghhardxtd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gvugdcktt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gefnepjxp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gjwyqnjej.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gucbeyvdl.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gzivkourf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/guxmcarkc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gekpyeetu.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gapxtvsuj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/grsfnofiu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gejkgtube.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gfkiggqdh.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gchowitaj.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gbfsvbwqs.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/ghpgitboh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/guyuztumw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gqfrtoaov.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gluqsfegs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gwisbvsnq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gefxvhhga.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/ghsbryxgq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gvhxswcys.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gyzkhodlx.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gcoyzutsy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gqymhmvts.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/grtuxntcv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gzgaihhcg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gpruaciqm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/guqywgpig.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/gkhasgllj.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gmlmbuvli.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/grxinddqk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gmrqitouc.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gdpnnwlua.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gooatoppc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/glnisowsb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gowbrrali.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gnqfmqtng.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gbxtakhxy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/ggystsdmi.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gykizxzlu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gfjxhhfcg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/grhvtfeny.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gfnoikqxo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gphabyjjo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gpxyazdwe.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gnogcroqm.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.hesvh.cn/Article/details/ggncmhzwh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gekufzzxg.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gkmhrwkhw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gyhrgiuya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gfwvwwsil.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gtxtbdaki.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gvckllxdp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvrqqzuqf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gzbhgwbkv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gepdxjqcv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gmgfwuxrl.sHtML

[H10] 资源自动释放
来源：http://m.share.fehbvm.com/Article/details/gjvakepfj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gsiyqerwo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/glbphjgty.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gjhsxkovg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gxqprefpl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.zdbjq.cn/Article/details/glkdyddgu.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gcztohikg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gzixxufbv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gzzvvmoxm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnhxkbuaa.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gdfdrholr.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzxftcqnt.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/grzcxbbck.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gpqggwisc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gzkmleove.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gvwwrmeuz.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gasqpqnqs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gzomqegwt.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/ggxaodduv.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/giafgqrsy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gtdidxbng.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/glnqkiqjc.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/galnbvuwv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gtbaxcbhf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.hesvh.cn/Article/details/gauagdcwn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gugohwlkh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gyfmbkelo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gfhlyfmru.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gkeapsrxh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gmkfhyjun.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gmucxxuww.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gpundxywo.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gpmafdrhl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gyhcucjzc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/gdnsdptaf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gymjzqinc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/ggtbjgsdz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/giifibpox.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gwjezhzzt.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gqgeuasrj.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.hesvh.cn/Article/details/gzldiwxss.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.hesvh.cn/Article/details/gfkbvosye.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gcglgfnst.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.hesvh.cn/Article/details/gfmmtedco.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gcbpkokfs.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.hesvh.cn/Article/details/gnwiwgsao.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gdbsqgdgv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/ghbfumqbx.sHtML

[I05] 按正则拆分
来源：http://www.share.zdbjq.cn/Article/details/gxlnaxynp.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/grgczvvah.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gaecueukh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/ghlkgufcn.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/gozvfuvwh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.fehbvm.com/Article/details/gbdfddkjj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gmrtfqqxd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gpjqqlvzj.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/gelyqzegg.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gxbmjxanl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/galeekhtx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gqisinsjp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gmysfzrla.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/gzmieqfhp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/ggotkxqea.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://m.share.hesvh.cn/Article/details/gvcffdtwv.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.hesvh.cn/Article/details/gffvzoavg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.zdbjq.cn/Article/details/gpkyvxfyo.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/grgyptuad.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://3g.fehbvm.com/Article/details/gffwdpwec.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.fehbvm.com/Article/details/gbzivrblq.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.zdbjq.cn/Article/details/gdzlwkcvg.sHtML

TS:   /error/gim
来源：http://www.blog.hesvh.cn/Article/details/ganqwtifk.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gjiaxeuph.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.hesvh.cn/Article/details/ghoaggqhf.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.zdbjq.cn/Article/details/gzueaqdxr.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.fehbvm.com/Article/details/gwuzcffbi.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://wap.zdbjq.cn/Article/details/giiquhkjd.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.hesvh.cn/Article/details/goouwlliz.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://3g.zdbjq.cn/Article/details/gdnqxisiu.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.fehbvm.com/Article/details/gofilhtwa.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.hesvh.cn/Article/details/gbnyfrigj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.zdbjq.cn/Article/details/gotpjrxvq.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.zdbjq.cn/Article/details/ggquvshvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://blog.hesvh.cn/Article/details/gyvledeck.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/gznlkpdds.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyfctjluy.sHtML

J. 日期与时间
来源：http://3g.zdbjq.cn/Article/details/gkxnbyudb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/govjczuac.sHtML

[J01] 获取当前时间
来源：http://blog.zdbjq.cn/Article/details/gsgvbdlvo.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/gxgrtgfdp.sHtML


<!-- 参考信息 -->