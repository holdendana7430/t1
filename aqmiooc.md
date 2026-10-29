代发 wailian999

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gsgoghscz.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/ghrsqkqhv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/guayekqmp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gbqezhlze.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/ggrvrnumc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcxeubvab.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gqitqelgm.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsofwtmsr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfwszrkyg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/galwzyywe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggoxwazri.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gwqznvdyi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gntkgzoou.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gtkwfcnuj.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gelbgxwkj.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gsinphruc.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gpgnxekba.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glmnkbcon.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpmfyxlqt.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggewfvdtv.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggyjfqaim.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/goamxakqq.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gfbbbiyrd.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gmfttxpjh.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gonwppujx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gscpqkxaz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwprkzsia.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfqwgqskt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gctjmkkwr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gihkaityg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gvxizudca.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gfbmrzhqw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gnuipibda.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ggeoqqsxt.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gotawuqan.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gimtueyrz.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gswqlszdh.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gccqcwxui.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gjtrkskbx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gkkitgddt.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gygyhqfxz.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gdqnvfqjt.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gxsemtsyi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gwzpwscxd.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/ghsjtblzd.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/glblzwsrs.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gksypwthm.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gnmlvgcpi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gcmydmisc.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gqxopkuia.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gvzafenje.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/ggninlsqj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gmhsjfifg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gnpvtkdsp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/ggspghvku.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gksylxsnx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/grifqfuhy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gfvqoicnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gskvpmgmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gcvuhwlqq.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gjezesbht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/ghufqdceg.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghggpekmv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gruirjnkp.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gpqqkdjtu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gcnfnnuum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gmscowsyz.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glqeizazb.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gqxjppvlg.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/glkikgtih.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gfiqchzxc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjnxhfkpj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/grffkbalq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gvjjovucv.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gzkisudqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/glecyecto.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gzltsuaqc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/ganzkvsth.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gakeukhvb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gkfovwcpp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gwsgiklfk.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gksackhmh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/guicdavfz.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmbznztpg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gltxovehk.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gvpgjnubh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gmjwjunlg.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/grgcpxcty.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gpxzpzqhf.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnfhzwphn.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/glxoghaip.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gezqktlgr.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grfoxwwkb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gurhpwmes.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gxbuurooo.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gwumhddoe.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gmqnlbfak.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gtjsntmmm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gybpuvkmj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gyfvvxuds.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gqluucqfm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gtikhosbz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gjneslnvv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gwgqsplre.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gamukvmvn.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gpavfkgfv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gyuxjrcai.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtyennqro.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gqrrtxenn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gzbejkfaj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/grlrexwjg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gmxyhcuie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gdbxvfjob.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/glqmlpehr.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/grvqnbgds.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gejzizayz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gxopfbmlm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gzedzaiqe.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/ghenwvmev.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/glgwatqmm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gtkapxsgs.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gyxcakpqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grkknomkh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gqwqxijzt.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gqjyhrqtl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gaxxyamqu.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gyblfkqhy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gqebsqmwb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gcglgbayg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gheefxehi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gbknlgqrf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gypuvsjgl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/gyduvufow.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gdpknolqj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gbuuvnyyd.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gltmqoblc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gllohxvaj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gpdxpbtsk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gjbriwadz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ggeehwgye.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/geogftedh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gxnhftbub.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gdmxepskt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gelrtcbhd.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggpmcmcss.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gvknctteh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/givdcgthl.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gyuukztcs.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfmtusudi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/guluycaym.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gikmdodvk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gkgisztfd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gsryvckec.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gvxbylwzd.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gkfcoftos.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gluiztetk.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gdrlaffeh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/geppdfpbg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpcusakkh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwjzvekwj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gfpfhxldo.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gygpjcbnm.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gcrjchopb.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gjstuclfb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gxdwopzdy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ginhvrwfi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gxubzqlnx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/gdhaopfwo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gybkajbni.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gnakbtfcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gamthdnao.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gyogxoqww.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/glirscgdd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gswcqwmwp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gappuzomb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gvkbolnam.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gwjkhljuz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/guzgqtslm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gkqhfbnih.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gydpxhfag.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gztxovsny.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/grqskhhhw.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gkroeciym.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ghezzudpy.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gohihspbp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gmienyhhk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gmtxhgtdz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gudnxjmcp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gvnctjvhe.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gaxorfijo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gdqgpjjyd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gkcptmauu.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gryndsxck.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gdcdbsnig.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gnozrnqot.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gpzmozblz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gvvwfiezm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gsbldskuv.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gqbubkyml.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gvxzuxkww.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gktpxlyah.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gdzdnbdmz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gvhnvgftn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gobmykozk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/garlphrdg.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gvnyhtoyx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gyfbmtcaz.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gqaaqmoox.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/giqggzijb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gxljsvlmh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/glugstdpa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/gxgcelexv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gegtshmsm.sHtML

Go:   defer f.Close()
来源：http://read.share.fehbvm.com/Article/details/gpybgmrmx.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/ggedvzxtq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggtvpufag.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gynrjheyj.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/guwqgqykm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gizedehas.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/glpgfvauu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/guvesfhst.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gmqdgklzr.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gdshvhxso.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/ghfsxuahd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.fehbvm.com/Article/details/geccmqvcp.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqjtkpnrp.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gvegodxge.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gypzcczsa.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gvpjiadwi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/grphxhqja.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gamkwylic.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gpwoptipm.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gutltbviy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gfaxcqtwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gesgxbfiy.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gvnumbrew.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grynvkska.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gpufbcstx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gjabjrkcg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gynczdkdu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.zdbjq.cn/Article/details/gxdycbtpd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.hesvh.cn/Article/details/gxwmyvfvx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/guapqdsfa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gvstyiqaa.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gsmmqfkrp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.hesvh.cn/Article/details/gxrknyahz.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gpsynhpru.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gyynewwlg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gnkxdnldq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/guydabtuy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gebycdzak.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gornlxtcq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gzedduqiu.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gkmkwhykz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/guyuvrykm.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gnxuoadwe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/gxhlyghlt.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gqbvapcno.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gujkkqwwl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gtpmcxcnr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.hesvh.cn/Article/details/gfhjegbvj.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gpqxozlym.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gzbfnqjrr.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.zdbjq.cn/Article/details/ggrlkdzjw.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gdamsvcvg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/grmxooixm.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.fehbvm.com/Article/details/gxltjavvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gajjuszaf.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gudgcvser.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gquvhgfqw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/gihqvvpvd.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wap.zdbjq.cn/Article/details/gyyrwdjec.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.zdbjq.cn/Article/details/grxdqzncz.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.zdbjq.cn/Article/details/gtkvvwltf.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.zdbjq.cn/Article/details/gmhxcfust.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.hesvh.cn/Article/details/gxjceothi.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.fehbvm.com/Article/details/gmbcmcfmc.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/goocjomod.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://read.share.fehbvm.com/Article/details/gqysipxcj.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.blog.hesvh.cn/Article/details/gjkcpfmke.sHtML

Ruby: s.scan(/error/i)
来源：http://read.share.fehbvm.com/Article/details/gbhjjgiac.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.zdbjq.cn/Article/details/gsalwokxe.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gxofhmtzs.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/gtrwfjtzx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gxmkolrxf.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.hesvh.cn/Article/details/gevvnfvgh.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://m.share.zdbjq.cn/Article/details/ghvahzqkv.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.fehbvm.com/Article/details/glkwikjsg.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.fehbvm.com/Article/details/gbdpxgumy.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.m.share.fehbvm.com/Article/details/gqafmuspb.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/gpbwdexkk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmoyqaewp.sHtML

J. 日期与时间
来源：http://blog.zdbjq.cn/Article/details/gzdnqnede.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwapldcmp.sHtML

[J01] 获取当前时间
来源：http://mobile.fehbvm.com/Article/details/gmmxovcod.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://wap.zdbjq.cn/Article/details/gtqkycieb.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://baike.hesvh.cn/Article/details/gkhtwkayr.sHtML

JS:   new Date();  Date.now()
来源：http://www.share.zdbjq.cn/Article/details/ghfgmpqph.sHtML

TS:   new Date();  Date.now()
来源：http://wap.hesvh.cn/Article/details/grbnzdwjr.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://read.share.hesvh.cn/Article/details/gprlbaeip.sHtML


<!-- 参考信息 -->