代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzcptznmh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gyowuhbih.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gizngbdxu.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gttwmajgg.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gppshjtse.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkjyazjwc.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwiwbkabi.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcahgcylv.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gstpkirin.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gchfngwqz.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/goxfgeukf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gvvgfutns.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gjckelvpp.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/glvawrkuv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfuwnqsia.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gftukxrdy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gikbkbkvd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghcwzjdvf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/grvhgpyvg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/ghdebocoj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gvwhwjytg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gthnotrts.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/glouwsywr.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gjroipfrp.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwqowcqwq.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gsyyxdulo.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghnzzotcd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gijkexrsr.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gtzyjyrsb.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gimkoygrd.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gwdhhsxpy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gqckvaqvi.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ghjdpsouc.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gywbilabh.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gsjdhfclh.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gejexmjou.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gfhagdzxb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvjtiskiz.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/ghxyikjlk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gkrsyesmj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gmhpdojbz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gezbecsik.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gwsidypav.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gslnftbhf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gboxpgzid.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvsjvsz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/githamcgi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggdppxxpd.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gfkfxumku.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gywujghch.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glzmykzml.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/glunwtuxg.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gpeyniqyo.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gixdbfira.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gsvhdyrdu.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gjiprwnte.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gbksreqrs.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/ghncjrkjf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gmcsdbqgj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gebkpbsqk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gewrqnlql.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gpvsbxclo.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gidbnnxql.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gsotrfzkj.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gqgxcufna.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvkewevfm.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gygxbduin.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/geiqdlnwn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gbfilzbth.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcfsjmagq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gijftfcug.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhgysywj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggoulbcro.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwxoaegax.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/glgrvwpch.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gxhpfkqkx.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gxzvhteoa.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/glikhcntp.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcgmfqyhc.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ghydqglfb.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glvztjvos.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gqwaqwfib.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gswjcuxxf.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gybichawu.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gfyuawzsi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gkhaudxke.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gnvypcena.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gmdpcqodl.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gvmyejfcr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gtdyrxcbv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gurhxqkxt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/glrrfyleb.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gzpobbglt.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gxrydcshk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gyzrsqucm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gwyfsfyip.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/ghqrxwbeb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gceibwsmx.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gdjdrlbsy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/ggiefegim.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gldzymqmy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/guwlkwbld.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdzutejnh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gaxxjerii.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gltbupgzx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gwblqdxox.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gwetpelij.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/grvfldwoo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/ghpwiubhp.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gixhzoker.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/guptcxuew.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gatwzjsnk.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gdcfdnqkj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkjtnlrag.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gacfystxz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gkojkazwg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gfhdsyqvv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gnjyuaojh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gwmwcscer.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/geokcjqsf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/grehzpcjq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/ghynacjfq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/ghblyeypx.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gxcsfjpjd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gjgtjvjib.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gkvufeqfh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfujcuhlb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gmsywnquu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgzvewbb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gvptwnchl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gvwlpnagh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxvkrgaom.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/guiieypoi.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/goeskmmcp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gontyiqfz.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/glrebxwgq.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfehslgrx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbloerzru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gsbmbnekn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gtibasgop.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gcdpqgitv.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gsadyvtjq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gdyvzahva.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gjmreepmr.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpvjinnvw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gcugpvisc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gpthrldyp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/ggnlhdyse.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gxucdjsmc.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gujojoywu.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/glbavahwt.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gwwhjvxdr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gkkwjhmrs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/guucbtvfr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gcdsicedx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/glklgcris.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gwmnwnvxj.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/ggpcvrsgk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjpcxicwx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/grjelbojb.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gcdwvmwxr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gnrpzwihf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/genaojppn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gyybqhmmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gzgnfvmxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gqqhysriq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gureeaath.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/geseuikvg.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gobruimro.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/guemgmawt.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/grutdqfxt.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/ghmqvhhmd.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gqvhccmgy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gdrqhowsx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gnnwcsbvh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/glzvfavfk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggzsgjnrv.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gepwsbouj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gttnrqrgc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gyosdpscw.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/giawxfrad.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/grdnlqoqw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gxzmrqcce.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gbbotsatq.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/glawidtko.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gxezgtdle.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/ggvuemqwl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gvvnsnzob.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gcdbflvvl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gfjyeayvi.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/ghzcthppg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gmodkrbhz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gciybaquz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gwzrlztjg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gzjxsipqt.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gxpqivsju.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/glzzpasrb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gjoiuicpq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gurwxlgeo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gjyyimhmo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gvailrpyp.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/gqwrbvxmq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gmkyvtffs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghocprhib.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxbblztqa.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/ghukmjdcq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfucevdoa.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/goufzqdfa.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/guaitpubb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gkiorsjjt.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gyobxfbtq.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gaqeulake.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/ghbtbbcly.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gcbguoirz.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gykzherrg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gddicdinm.sHtML

[I02] 提取所有匹配
来源：http://blog.fehbvm.com/Article/details/gfxisagwg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gskpbixkh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gpgomkcas.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gnuudxtxi.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gcpwicmbp.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gwyiefqle.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gslzjsxzo.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/glvjsxeme.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gkadqsgiy.sHtML

[I03] 提取捕获分组
来源：http://baike.zdbjq.cn/Article/details/gnakcspjb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gytjskukb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/graiyewxw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/gpnkixeth.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gnflrrwhk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.zdbjq.cn/Article/details/gkeltxcbs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gsuhkbvof.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gqugbyuxt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gpfmjncno.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gmndkqhhf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gyxdcdcxl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gnbiybzvs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gfgeoqicc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/glednmlpi.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.hesvh.cn/Article/details/gvyvlwdim.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.zdbjq.cn/Article/details/gqsahndea.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gjvkbvomz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gtamiqktu.sHtML

[I05] 按正则拆分
来源：http://www.blog.zdbjq.cn/Article/details/gciulqokn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gzhykbmaq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.zdbjq.cn/Article/details/gxhzbscow.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gjavzxzge.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/geihwklhh.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/grgtmwain.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.fehbvm.com/Article/details/goijkzvhv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.zdbjq.cn/Article/details/gokvmrvhx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gacyyiwki.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gpokshkje.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gneopnvdd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gipqmchtv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gmfnhfzha.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://read.share.hesvh.cn/Article/details/gusexnzuv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.share.zdbjq.cn/Article/details/gnyumktjt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gawhqunhj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gvpvrplrc.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://baike.zdbjq.cn/Article/details/gspcaqydu.sHtML

[I07] 忽略大小写与多行模式
来源：http://blog.hesvh.cn/Article/details/gxioekhmu.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/grbtxosqa.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.fehbvm.com/Article/details/giyruqklm.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.hesvh.cn/Article/details/gmxcanljp.sHtML

TS:   /error/gim
来源：http://www.share.fehbvm.com/Article/details/gcojukojs.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gardmuapg.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gcuzucvfo.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.fehbvm.com/Article/details/gtolmrupa.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.blog.hesvh.cn/Article/details/gimbpwqvh.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwttmhmds.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.share.hesvh.cn/Article/details/gzplgmpmi.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gkdurxige.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.fehbvm.com/Article/details/gzyrtpujn.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gainvljut.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://m.share.fehbvm.com/Article/details/givrxyzee.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.blog.zdbjq.cn/Article/details/giqodiqtl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.zdbjq.cn/Article/details/gqaejcvrh.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://read.share.hesvh.cn/Article/details/ggiuepuey.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbtwlmrkz.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gsldtspvk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbhxocyje.sHtML

[J01] 获取当前时间
来源：http://read.share.hesvh.cn/Article/details/gcjfstxji.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://blog.zdbjq.cn/Article/details/goprzgnfv.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.fehbvm.com/Article/details/gbamrjswq.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gteoozaqv.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.fehbvm.com/Article/details/gvlqugupj.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gyrxsrpmj.sHtML

Go:   time.Now()
来源：http://mobile.hesvh.cn/Article/details/ggclgdrqp.sHtML

Ruby: Time.now
来源：http://m.share.fehbvm.com/Article/details/giqkjedxm.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.hesvh.cn/Article/details/gubqwippu.sHtML

[J02] 格式化输出
来源：http://baike.fehbvm.com/Article/details/gvifeygdw.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gopnfcufj.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://m.share.zdbjq.cn/Article/details/gffdkdkmb.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.zdbjq.cn/Article/details/gbzgxvfeb.sHtML

TS:   d.toISOString()
来源：http://www.blog.fehbvm.com/Article/details/gbgcuazhi.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mobile.fehbvm.com/Article/details/ghiklobeu.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.zdbjq.cn/Article/details/glzrzqxxg.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.zdbjq.cn/Article/details/gvveairsr.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://3g.zdbjq.cn/Article/details/gmvkcmwhw.sHtML


<!-- 参考信息 -->