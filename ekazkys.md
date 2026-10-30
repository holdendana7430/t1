代发 wailian999

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwrthiskp.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/guuvbxxwx.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gcbvucnvr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gqfjjehew.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/godmvprov.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gdzobnsuc.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gdezdxyom.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gjgkdbmrh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gsgavrije.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdvxjfclu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/ggtianhps.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbcbrcciw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gjnykgnwt.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gokjftkxq.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/geimloiet.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gejrnduwv.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gcjehfzqh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtmqqdlze.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdkzqtrsq.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdgncezre.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmiwttifm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gynpffegz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gijsseyif.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggqpbekht.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gqasbdhru.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gvpuzwpfe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/goidgsfrz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvcmboqep.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzqfiyrxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/galtalclt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gdaehsitg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gzkjhyejz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gduyeumbc.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gzdrynkqf.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gaywpvgje.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gldbskynd.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gnwouqeev.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gvslspnff.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gnqnsekyg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gdqvocanx.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gmqbmsmhj.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gjyayxrdv.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvoellbfw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/ggyjyndxn.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gvvjrfmaz.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gsrynvcdz.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gbelsxcye.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gniyawtla.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gkkiljptc.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gyjvgxthy.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gguzggkxw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gbnjdssnf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gkcmnvjre.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/goydkulhp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gwbkhadfu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gujgrwvwl.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gwvccewha.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gfnuldsrl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gnumnsjof.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjwprlgca.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gttwkoqvi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gmosasyyq.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtcknfpcr.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gwsiwdgne.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/guqwdwbqa.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gcpirmqhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gvegsummx.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghpewrtdo.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/ghzbnpgcy.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gxknzcfod.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/grtwfncax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/giltldtbo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gkclbesix.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gvusxugww.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdblmdeye.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkncpakjx.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/glnizbxqf.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gkqacmsaq.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/ggitrryvf.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqhmubytj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gshrckwki.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glzrovckc.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grvuznhwg.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gvzhexllx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gukhhonlx.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gzzvhaoqc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gdwvkyngm.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gutbgbjmf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gsrglvbgr.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gpxegjgsb.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/goyaxfhfn.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvmjikcxw.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvmvavtxu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gxfkhsnnd.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gvilzzqtg.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gwvsqlzjm.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gjdqenfju.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gzqjnzgai.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gejkcrfej.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/geheuzbtr.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/glcprtbwr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/ggggssqgd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqauauhd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gbupirduu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gzdjjhrix.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grpgbuacj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gmeflbmel.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/grdszviuv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/goxgtmium.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gldjeqola.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gngkhnsac.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gftyevjip.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gjrqmuiod.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/ggtpdfyuu.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwsmzivsk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gemvvnnvp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gcgsbxjfg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gndzwhvsy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gutjgfluu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gdsofdsam.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gbemgcpkq.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gfbmhsfgw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gkfiotwwn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grmmradyf.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gbyqgthoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbyhrkdii.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gwvmbsqel.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gzadpzhvn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gszgzgoam.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gvjtrxxcr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gfcpzpsea.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gpzqfkobo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gbuadxelv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gpsokfzdr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gjbihxiuv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gnmytxzca.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gypylhqoz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnulbzhbp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gjcubciab.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsbfydznb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/glwumgbus.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/giuqkaahb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gkhpjnsjj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gbgbjaoyj.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gmtncervl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gneqipkjm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gteqycwrm.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gyhxrsknw.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gsrwwtvpf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdpwqjhew.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gudvnqjjz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/glwufmyvu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gisuocubt.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gjjbpaapj.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gzlvmbkmx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/goywdekpi.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gscbpxgcf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gvwksqofw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gsdedcokl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gdixqwdfz.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gtlnwpciy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/ggxujeqpx.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gwklozhtq.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gbozilchk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/grwxoiyyu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gplovdhdt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdqmappbr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/geiwfdsvq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gwnexkeic.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gjcbdydwn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/ggbwaaybm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gjwjjdqhj.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/gkcrrbjjj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gitzyjooo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/ggzzaycll.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gqmwriuat.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gqoalstfi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gvrqentmp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gjytnwmea.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gdcqlkvpu.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/ghvsxmmbd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gciyumdkc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ggpzjeowx.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gimamimvf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/glvnwccru.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gxyhoufcc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/giropqpdk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gpdvtskmy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gowubfvhh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gaozljnsx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gcxqnabya.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gsubxrirf.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/guanuvvkb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/guikmtrgq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gnczhjorc.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/ghuravjjw.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gzwpagptz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/goraexhiw.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gvwpboimn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gohckkwcw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/ghlrfvhps.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/ggfzkcgei.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gdygpihal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gckjxgrge.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.hesvh.cn/Article/details/grkwmsvoy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/ggkvvhbir.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gkofgzoan.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/glimwyhcx.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gosdziftb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fehbvm.com/Article/details/gchkiwhqq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gnsodbocs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gqhqsaijt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gzwjysxyu.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gxvoeqkdl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/guledgstg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggydueyxj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/govanmkku.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gteccjawo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjvgvqhlg.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gzuaezskh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwpogobzg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gjizsafnf.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gvxajpkzl.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gljafjrsw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gvjoudkef.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gcjeudipi.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gptwfjdas.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gdowztszi.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfsgqkmid.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gspdxivgq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gsjaiakrf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/girwoyuxb.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gxliosoiv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gvzfhwyoh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxvrtdj.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gobvozcvo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggstvynwn.sHtML

[I03] 提取捕获分组
来源：http://www.share.hesvh.cn/Article/details/gkznixtgr.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gxklveurl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gosfugdkk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gpcjehdgo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gqqwcpexr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gnpvhpkic.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gjbfhflat.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/ggozvrdav.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gtnfaftln.sHtML

[I04] 正则替换
来源：http://baike.zdbjq.cn/Article/details/gkghhvizv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.zdbjq.cn/Article/details/gwbqyygot.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gllplcbjk.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gyyqlscke.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gssiqbmus.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gywvcuejx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.fehbvm.com/Article/details/gsesdsynf.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.fehbvm.com/Article/details/gxjwabaly.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gigxbugvh.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gagqdwiey.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.zdbjq.cn/Article/details/gjyyzggbd.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwqbahosi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gdjwbmwsf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/giotezirn.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gvgqbjkyx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gtocsxpwh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gqukpmica.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gkdovozhm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.fehbvm.com/Article/details/gogmbihbn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://baike.fehbvm.com/Article/details/grobtemvw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.hesvh.cn/Article/details/glanudayy.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/grvdknjhv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/govcrvojv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.hesvh.cn/Article/details/giwohcwsy.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gebrlkirs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gpphufgyu.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/gllishnqr.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.fehbvm.com/Article/details/gmhezfkpg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gayhhaavc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/glbfrujfv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.hesvh.cn/Article/details/gtnyvownz.sHtML

TS:   /error/gim
来源：http://wap.fehbvm.com/Article/details/gsoaopnhx.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wap.hesvh.cn/Article/details/gddqxwufn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gxysypwtp.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.zdbjq.cn/Article/details/ghlddbmrb.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gntcdjydt.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gfzelvjrj.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.blog.zdbjq.cn/Article/details/genzfueba.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://blog.zdbjq.cn/Article/details/gmlwwjcye.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfszmjab.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.fehbvm.com/Article/details/gwostgukb.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/ggmlnahpe.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gnyzmsoxw.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.hesvh.cn/Article/details/gwtudbltt.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.share.fehbvm.com/Article/details/gerisrpyb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggeolnpkk.sHtML

J. 日期与时间
来源：http://m.share.fehbvm.com/Article/details/ggasgieyr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gebdwraqj.sHtML

[J01] 获取当前时间
来源：http://3g.hesvh.cn/Article/details/gkqcolmfa.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.blog.hesvh.cn/Article/details/ggijwijsc.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wap.zdbjq.cn/Article/details/gwuqqcvqs.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gwmehwvds.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.fehbvm.com/Article/details/gwvknjntv.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/grobwjols.sHtML


<!-- 参考信息 -->